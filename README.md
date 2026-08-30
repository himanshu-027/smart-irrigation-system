# Smart Irrigation System

An Arduino-based smart irrigation system that automatically monitors soil moisture and controls a water pump according to the moisture level.

---

## Project Preview

![Smart Irrigation System](images/project-front.jpg)

---

## Features

- Real-time soil moisture monitoring
- Automatic water pump control
- 16×2 I2C LCD display
- Relay-based pump switching
- Serial Monitor output
- Low-cost and simple hardware
- Automatic irrigation based on soil condition

---

## How It Works

The soil moisture sensor measures the moisture level of the soil.

The Arduino reads the sensor value through analog pin **A0**.

If the moisture value is greater than the defined threshold of **700**, the Arduino activates the relay and turns **ON** the water pump.

If the moisture value is **700 or below**, the pump remains **OFF**.

The current moisture level and pump status are displayed on the **16×2 I2C LCD**.

---

## Hardware Required

| Component | Quantity |
|---|---:|
| Arduino UNO | 1 |
| Soil Moisture Sensor | 1 |
| 16×2 I2C LCD | 1 |
| Relay Module | 1 |
| DC Water Pump | 1 |
| External Power Supply | 1 |
| Jumper Wires | As required |

---

## Pin Connections

| Component | Pin | Arduino UNO |
|---|---|---|
| Soil Moisture Sensor | AO | A0 |
| Relay Module | IN | D8 |
| LCD | SDA | A4 |
| LCD | SCL | A5 |
| LCD | VCC | 5V |
| LCD | GND | GND |

---

## Circuit Diagram

![Circuit Diagram](circuit/circuit-diagram.png)

---

## Software

- Arduino IDE
- Arduino C/C++
- Wire Library
- LiquidCrystal_I2C Library

---

## Working Logic

```text
             START
               ↓
      Read Soil Moisture
               ↓
       Display Moisture
               ↓
      Is Moisture > 700?
          ↙           ↘
        YES            NO
         ↓              ↓
      Pump ON        Pump OFF
         ↓              ↓
         └──────┬───────┘
                ↓
             Repeat