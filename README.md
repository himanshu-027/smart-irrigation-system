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

|**Component**|**Quantity**|
|-|-|
|**Arduino UNO**|1|
|**Soil Moisture Sensor**|1|
|**16x2 I2C LCD**|1|
|**Relay Module**|1|
|**DC Water Pump**|1|
|**External Power Supply**|1|
|**Jumper Wires**|As per required|



### \## Pin Connections

|**Component**|**Pin**|**Arduino UNO**|
|-|-|-|
|**Soil Moisture Sensor**|**A0**|**A0**|
|**Soil Moisture Sensor**|**VCC**|**3.3V**|
|**Soil Moisture Sensor**|**GND**|**GND**|
|**Relay Module**|**IN**|**D8**|
|**Relay Module**|**VCC**|**5V**|
|**Relay Module**|**GND**|**GND**|
|**LCD**|**SDA**|**A4**|
|**LCD**|**SCL**|**A5**|
|**LCD**|**VCC**|**5V**|
|**LCD**|**GND**|**GND**|



### \## Software Required

&#x09;**- Arduino IDE**

&#x09;**- Arduino C/C++**

&#x09;**- Wire Library**

&#x09;**- LiquidCrystal\_I2C Library**



### \##System Flow

|**start<br />**      		 	**v<br />**		**Initialize Serial<br />**       			**\|<br />**       			**v<br />**		**Configure Relay<br />**	        	**\|<br />**      	 		**v<br />**		**Initialize LCD<br />**       			**\|<br />**       			**v<br />**		**Read Soil Moisture<br />**       			**\|<br />**       			**v<br />**		**Display Moisture<br />**                	**\|<br />**                	**v<br />**		**Moisture > 700?<br />**       			**\|<br />**  	   **+---------- YES ----------+<br />**  	   **\|                         \|<br />** 	   **v                         v<br />**         **Pump ON                  Pump OFF<br />**  	   **\|                         \|<br />**    	   **+------------+------------+<br />**                        **\|<br />**               		**v<br />**          	  **Wait 1 Second<br />**               		**\|<br />**               		**v<br />**             	      **REPEAT**|
|-|



&#x20;

