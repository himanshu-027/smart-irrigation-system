##Smart Irrigation System An Arduino-based automatic irrigation system that monitors soil moisture and controls a water pump according to the moisture level.

Project Overview
The Smart Irrigation System is designed to automate the watering process by monitoring the moisture level of soil. A soil moisture sensor continuously measures the soil condition. The Arduino UNO processes the sensor reading and automatically controls a water pump through a relay module. The current moisture level and pump status are displayed on a 16×2 I2C LCD.

Features
🌱 Real-time soil moisture monitoring
💧 Automatic water pump control
📟 16×2 I2C LCD display
🔌 Relay-based pump switching
🖥️ Serial Monitor output
⚡ Simple and low-cost implementation
🔄 Continuous automatic monitoring
Working Principle
The system works in the following sequence:

The soil moisture sensor measures the moisture level.
Arduino UNO reads the sensor value through analog pin A0.
The moisture value is displayed on the LCD.
Arduino compares the moisture value with the threshold value 700.
If the moisture value is greater than 700, the relay is activated and the pump turns ON.
If the moisture value is 700 or below, the pump remains OFF.
The process repeats continuously.
System Flow
             ┌──────────────┐
             │    START     │
             └──────┬───────┘
                    │
                    ▼
         ┌────────────────────┐
         │ Read Soil Moisture │
         └─────────┬──────────┘
                   │
                   ▼
         ┌────────────────────┐
         │ Display Moisture   │
         │ Value on LCD       │
         └─────────┬──────────┘
                   │
                   ▼
          ┌─────────────────┐
          │ Moisture > 700? │
          └───────┬─────────┘
             YES  │  NO
              ▼   │   ▼
        ┌────────┐ │ ┌─────────┐
        │Pump ON │ │ │ Pump OFF│
        └────┬───┘ │ └────┬────┘
             │     │      │
             └─────┴──────┘
                   │
                   ▼
             ┌───────────┐
             │   Repeat  │
             └───────────┘
