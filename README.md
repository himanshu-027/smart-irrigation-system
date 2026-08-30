# \# Smart Irrigation System

**An Arduino-based smart irrigation system that automatically**

**monitors soil moisture and controls a water pump according**

**to the moisture level.**



### \## Project Overview

* **The Smart Irrigation System is designed to automate the**

&#x20;   **process of plants.**

* **A soil moisture sensor is used to measure the moisture**

&#x20;  **level of the soil.**

* **Arduino UNO reads the sensor value and controls the**

&#x20;   **water pump through a relay module.**

* **A 16x2 I2C LCD displays the current moisture value**

&#x20;  **and pump status.**



### \## Features

&#x09;**-** **Soil moisture monitoring**

&#x09;**- Automatic pump control**

&#x09;**- 16x2 I2C LCD display**

&#x09;**- Relay-based switching**

&#x09;**- Serial Monitor output**

&#x09;**- Automatic irrigation**

&#x09;**- Simple hardware design**

&#x09;**- Low-cost implementation**

&#x09;**- Continuous monitoring**



### \## Components Required

&#x09;**| Component | Quantity |**

&#x09;**|---|---:|**

&#x09;**| Arduino UNO | 1 |**

&#x09;**| Soil Moisture Sensor | 1 |**

&#x09;**| 16x2 I2C LCD | 1 |**

&#x09;**| Relay Module | 1 |**

&#x09;**| DC Water Pump | 1 |**

&#x09;**| External Power Supply | 1 |**

&#x09;**| Jumper Wires | As required |**



### \## Pin Connections

&#x09;**| Component | Pin | Arduino UNO |**

&#x09;**|---|---|---|**

&#x09;**| Soil Moisture Sensor | AO | A0 |**

&#x09;**| Soil Moisture Sensor | VCC | 5V |**

&#x09;**| Soil Moisture Sensor | GND | GND |**

&#x09;**| Relay Module | IN | D8 |**

&#x09;**| Relay Module | VCC | 5V |**

&#x09;**| Relay Module | GND | GND |**

&#x09;**| LCD | SDA | A4 |**

&#x09;**| LCD | SCL | A5 |**

&#x09;**| LCD | VCC | 5V |**

&#x09;**| LCD | GND | GND |**



### \## Software Required

&#x09;**- Arduino IDE**

&#x09;**- Arduino C/C++**

&#x09;**- Wire Library**

&#x09;**- LiquidCrystal\_I2C Library**



### \##System Flow

&#x20;     	       	      **START**

&#x20;     		 	**|**

&#x20;     		 	**v**

&#x09;	**Initialize Serial**

&#x20;      			**|**

&#x20;      			**v**

&#x09;	**Configure Relay**

&#x09;        	**|**

&#x20;     	 		**v**

&#x09;	**Initialize LCD**

&#x20;      			**|**

&#x20;      			**v**

&#x09;	**Read Soil Moisture**

&#x20;      			**|**

&#x20;      			**v**

&#x09;	**Display Moisture**

&#x20;               	**|**

&#x20;               	**v**

&#x09;	**Moisture > 700?**

&#x20;      			**|**

&#x20; 	   **+---------- YES ----------+**

&#x20; 	   **|                         |**

&#x20;	   **v                         v**

&#x20;        **Pump ON                  Pump OFF**

&#x20; 	   **|                         |**

&#x20;   	   **+------------+------------+**

&#x20;                       **|**

&#x20;              		**v**

&#x20;         	  **Wait 1 Second**

&#x20;              		**|**

&#x20;              		**v**

&#x20;            	      **REPEAT**

