\# Smart Irrigation System

An Arduino-based smart irrigation system that automatically

monitors soil moisture and controls a water pump according

to the moisture level.



\## Project Overview

The Smart Irrigation System is designed to automate the

watering process of plants.

A soil moisture sensor is used to measure the moisture

level of the soil.

Arduino UNO reads the sensor value and controls the

water pump through a relay module.

A 16x2 I2C LCD displays the current moisture value

and pump status.



\## Features

\- Soil moisture monitoring

\- Automatic pump control

\- 16x2 I2C LCD display

\- Relay-based switching

\- Serial Monitor output

\- Automatic irrigation

\- Simple hardware design

\- Low-cost implementation

\- Continuous monitoring



\## Components Required

| Component | Quantity |

|---|---:|

| Arduino UNO | 1 |

| Soil Moisture Sensor | 1 |

| 16x2 I2C LCD | 1 |

| Relay Module | 1 |

| DC Water Pump | 1 |

| External Power Supply | 1 |

| Jumper Wires | As required |



\## Pin Connections

| Component | Pin | Arduino UNO |

|---|---|---|

| Soil Moisture Sensor | AO | A0 |

| Soil Moisture Sensor | VCC | 5V |

| Soil Moisture Sensor | GND | GND |

| Relay Module | IN | D8 |

| Relay Module | VCC | 5V |

| Relay Module | GND | GND |

| LCD | SDA | A4 |

| LCD | SCL | A5 |

| LCD | VCC | 5V |

| LCD | GND | GND |



\## Software Required

\- Arduino IDE

\- Arduino C/C++

\- Wire Library

\- LiquidCrystal\_I2C Library



\## System Flow

START

&#x20; ↓

Initialize Serial

&#x20; ↓

Set Relay as OUTPUT

&#x20; ↓

Keep Pump OFF

&#x20; ↓

Initialize LCD

&#x20; ↓

Display "Smart Irrigation"

&#x20; ↓

Clear LCD

&#x20; ↓

Read Soil Moisture

&#x20; ↓

Display Moisture Value

&#x20; ↓

Is Moisture > 700?

&#x20; ↓

&#x20;┌───────────────┐

&#x20;│               │

YES              NO

&#x20;│               │

&#x20;↓               ↓

Pump ON        Pump OFF

&#x20;│               │

&#x20;↓               ↓

Display ON     Display OFF

&#x20;│               │

&#x20;└───────┬───────┘

&#x20;        ↓

&#x20;    Wait 1 Second

&#x20;        ↓

&#x20;      REPEAT



