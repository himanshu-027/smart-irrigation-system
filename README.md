# Smart Irrigation System





**An Arduino-based smart irrigation system that automatically monitors soil moisture and controls a water pump according to the moisture level.**





## Project Overview





* **The Smart Irrigation System is designed to automate the watering process of plants.**
* **A soil moisture sensor is used to measure the moisture level of the soil.**
* **Arduino UNO reads the sensor value and controls the water pump through a relay module.**
* **A 16x2 I2C LCD displays the current moisture value and pump status.**



## Features





&#x09;**-** **Soil moisture monitoring**

&#x09;**- Automatic pump control**

&#x09;**- 16x2 I2C LCD display**

&#x09;**- Relay-based switching**

&#x09;**- Serial Monitor output**

&#x09;**- Automatic irrigation**

&#x09;**- Simple hardware design**

&#x09;**- Low-cost implementation**

&#x09;**- Continuous monitoring**



## Components Required





|**Component**|**Quantity**|
|-|-|
|**Arduino UNO**|1|
|**Soil Moisture Sensor**|1|
|**16x2 I2C LCD**|1|
|**Relay Module**|1|
|**DC Water Pump**|1|
|**External Power Supply**|1|
|**Jumper Wires**|As per required|



## Pin Connections





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

## Software Required





**- Arduino IDE**

**- Arduino C/C++**

**- Wire Library**

**- LiquidCrystal\_I2C Library**



## System Flow





|                      **start<br />**      		 	**v<br />**		**Initialize Serial<br />**       			**\|<br />**       			**v<br />**		**Configure Relay<br />**	        	**\|<br />**      	 		**v<br />**		**Initialize LCD<br />**       			**\|<br />**       			**v<br />**		**Read Soil Moisture<br />**       			**\|<br />**       			**v<br />**		**Display Moisture<br />**                	**\|<br />**                	**v<br />**		**Moisture > 700?<br />**       			**\|<br />**  	   **+---------- YES ----------+<br />**  	   **\|                         \|<br />** 	   **v                         v<br />**         **Pump ON                  Pump OFF<br />**  	   **\|                         \|<br />**    	   **+------------+------------+<br />**                        **\|<br />**               		**v<br />**          	  **Wait 1 Second<br />**               		**\|<br />**               		**v<br />**             	      **REPEAT**|
|-|

## 

## Results





**The developed system successfully demonstrates automatic irrigation based on soil moisture readings.**

**The Arduino continuously monitors the soil moisture and controls the pump according to the programmed threshold.**

**The LCD provides real-time information about the moisture value and pump status.**



## **Advantages**





1. **Automatic irrigation**
2. **Saves water**
3. **Reduces manual effort**
4. **Simple circuit**
5. **Low-cost components**
6. **Easy to understand and modify**
7. **Suitable for small-scale applications**
8. **Real-time monitoring**



## **Future Scope**





**The project can be further improved by adding advanced features such as:**

**📱 Mobile application for monitoring**

**🌐 IoT-based remote monitoring**

**📡 ESP32/ESP8266 integration**

**☁️ Cloud-based data storage**

**💧 Water tank level monitoring**

**🌦️ Weather-based irrigation**

**🔔 Mobile notifications**

**🎛️ Remote pump control**

**📊 Moisture data graphs**

**🤖 AI/ML-based irrigation prediction**

**🔋 Solar-powered operation**

&#x20;

## **Applications**





1. **The system can be used in:**
2. **Home gardens**
3. **Agricultural fields**
4. **Greenhouses**
5. **Plant nurseries**
6. **Smart farming systems**
7. **Automatic gardening systems**
8. **Small-scale irrigation systems**



## **Conclusion**





**The Smart Irrigation System successfully demonstrates an automatic method of controlling irrigation based on soil moisture.**

**The Arduino reads the moisture sensor, processes the sensor value, and controls the water pump through a relay.**

**The LCD and Serial Monitor provide real-time information about the moisture level and pump status.**

**This project provides a simple foundation for developing more advanced IoT-based and AI-powered smart agriculture systems.**



## **Acknowledgement**





**I would like to express my sincere gratitude to everyone who supported and guided me during the development of this project.**



## **Author**





**Himanshu Prajapati**



## **License**





**This project is created for educational and learning purposes.**

