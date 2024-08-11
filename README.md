# Smart-Agriculture-System
## Introduction
### Current scenario
The current scenario for this project is the growing need for this system in Nepal and other countries that are heavily dependent on agriculture as well as for various food and dairy based industries. This project can be used for different purposes, mainly for agriculture and floriculture. Currently this system is implemented in very few parts of the world, with a few being Japan, Australia, and Canada. Most farmers still use the traditional agricultural practices which has resulted in different problems such as low crop production, poor crop quality and soil degradation.
Our project and project like this are very much needed and are in high demand due to the above-mentioned problems. The reason for coming up with this project is to meet the rising demand for such systems at a lower cost without any compromise in its performance.  This project provides a reliable and accurate way to measure the temperature, humidity and soil moisture which aids farmers to make informed decisions on irrigation, fertilization, and other agricultural practices which results in greater crop yields and higher crop quality.

### Problem Statement and Project as a solution
Farmers face several problems in Agriculture and other similar industries that impacts their productivity. One of the most common problems faced in agriculture industry is reduced crop yield. This can occur due to various factors such as inadequate water supply, poor soil quality and growing plants in environments which are not suitable for their growth. Another significant challenge faced by farmers is the outbreak of diseases and pests in crops or livestock. Various insects and animals such as mouse destroy crops which results in reduced crop yield.
The solution to these problems is temperature and humidity monitoring device. This device uses components such as DHT11 and soil moisture sensor which accurately measures temperature, humidity, and soil moisture. This device is also equipped with an LCD that display all the reading measured by the sensors. By observing the measurements displayed by this device, farmers gain insight on their environments which will help them to decide suitable plant to grow in that environment and therefore result in increase in crop yield. Furthermore, the soil moisture measurements displayed in the device helps farmers to know if the crops are dehydrated which helps farmers to water the crops appropriately. Additionally, the project also has an ultrasonic sensor and a buzzer which are connected. The buzzer emits a sound after ultrasonic sensor senses animals such as mouse, which drives the animals away resulting in crop protection from animals.


## Design Diagrams (Hardware Architecture, Flowchart, Circuit diagram) 
### 	HARDWARE ARCHITECTURE
![Screenshot 2024-08-11 104023](https://github.com/user-attachments/assets/268ef246-cdee-4411-91b8-cb18834e28ca) 
### FLOWCHART OF THE SYSTEM

![Screenshot 2024-08-11 104047](https://github.com/user-attachments/assets/54767e92-5964-451c-a8da-c4de89e7baea)
## CIRCUIT DIAGRAM
![Screenshot 2024-08-11 104059](https://github.com/user-attachments/assets/cba9983e-0009-4169-a868-43bbae3d5400)
 
## 	Development

This section will describe the step-by-step process that we took to build the project. Development provides an overview of the process used to create the system being described. For this development, one development methodology we employed was the Waterfall methodologies. By strictly following this methodology are prompted to only proceed to the next part of the development step after we have completed the one we are working on. We approached the development of our system in phases. The phases are described below,
Phase 1:
- For the initial phase, we started gathering all the necessary materials required for the project. The materials include: ESP32 Wi-Fi module, a DHT11 sensor, a soil moisture sensor, an LCD, a breadboard, an ultrasonic sensor, a buzzer and a USB cable. Given that we were handed an ESP32 Wi-Fi module a microcontroller which we had no prior knowledge of, we spent the remainder of this development phase researching on the parts and their functionalities, especially that of the ESP32 Wi-Fi module. 
Phase 2:
- For this phase, we looked up on the libraries that were needed for the project. The libraries were needed in order to program the equipments in Arduino IDE. We started off by installing the libraries on the Arduino IDE, since we had no knowledge of which libraries we had to install, our module leader provided us with the library ZIP file which we downloaded and installed it to the Arduino IDE directly. Libraries included: “LCD Library”,” DHT11 Library”, “Adafruit Sensor Library”, “ThingSpeak Library”, “Wi-Fi Library”. 
Phase 3:
- In this phase, we connected all the equipments together on a breadboard. We started off by connecting the DHT11 sensor, soil moisture sensor, ESP32 Wi-Fi module and LCD on the breadboard. Afterwards we tested the DHT11 sensor by placing in room temperature and soil moisture sensor by inserting it inside soil and checked if they measured accurate measurements. After verifying that the measurements were accurate, we displayed those measurements on the LCD and subsequently sent it to the ThingSpeak platform in order to view the data remotely. Later, we proceeded to connect ultrasonic sensor and buzzer in the breadboard. 
Phase 4:
- This was our final phase while developing the project. In this phase, we wrote the code for ultrasonic sensor and the buzzer. We programmed it in such a way that when the ultrasonic sensor detects an object, the buzzer emits a high frequency sound.

 
## Results and Findings
After the completion of the project, the system displayed accurate measurements of surrounding temperature, humidity as well as soil moisture in the LCD. The LCD displayed clear and concise readings. Furthermore, the ultrasonic sensor which was equipped in order to detect objects and animals also showed no signs of error and detected objects precisely. The buzzer which was connected to the ultrasonic sensor and programmed to emit a high frequency recurring sound when the ultrasonic sensor detected objects also worked appropriately. All the sensors performed well and sent their measurements to ESP-32 Wi-Fi module. Moreover, with no signs of error the ESP-32 Wi-Fi module collected the data provided by various sensors and using Wi-Fi technology, wirelessly transmitted all the obtained data to ThinkSpeak platform. Using ThingSpeak platform we were able to remotely view all the measurements provided by the sensors in real time as well as collect all those readings for future use. The GSM (Global System for Mobile Communication) module which was supposed to send alert messages to the user’s mobile phone through SMS (Short Message Service) didn’t succeed in doing so because the GSM module failed to fetch the signal from the network as MDMS (Mobile Device Management System) implemented in Nepal.

 
### Test Case:
- Checking soil moisture sensor’s readings when it is not placed at any medium
  
  ![Screenshot 2024-08-11 105448](https://github.com/user-attachments/assets/448f043a-8870-42d8-829b-dfb451ecddfe)
  
       Findings of moisture sensor when it is not placed at any medium
The reading of the moisture of the soil by the soil moisture (FC-28) in LCD display is represented by ‘soil ms’ and the unit of the measurement is in percentage. The soil moisture measures 0% as shown in figure above; since the sensor is not given any medium to operate.
 
- Checking soil moisture sensor’s readings while placing it inside soil.
  
  ![Screenshot 2024-08-11 105503](https://github.com/user-attachments/assets/1d8a7706-3f40-4156-9a27-fe7d85cb5264)
  
        Findings of moisture sensor when placed on a muddy soil.
The reading of the moisture of the soil by the soil moisture (FC-28) in LCD display is represented by ‘soil ms’ and the unit of the measurement is in percentage. The soil moisture measures 51% as shown in figure above; since the sensor is inserted inside the soil.
 
- Checking soil moisture sensor’s reading while placing it inside water.
  
 ![Screenshot 2024-08-11 105512](https://github.com/user-attachments/assets/d8eb45a5-04cb-4c7d-9992-6f6e72c67496)
 
             Findings of moisture sensor when placed on a water.
The reading of the moisture of the soil by the soil moisture (FC-28) in LCD display is represented by ‘soil ms’ and the unit of the measurement is in percentage. The soil moisture measures 59% as shown in figure above; since the sensor is inserted inside water.
 
- Checking the readings of DHT11 sensor on room temperature.
  
![Screenshot 2024-08-11 105521](https://github.com/user-attachments/assets/0b8fde0f-3ba9-4f80-9e69-8c6d91dde4eb)

            Readings of temperature and humidity from DHT-11
The reading of temperature and humidity detected by the DHT11 sensor in LCD display is represented by “T” for temperature and “H” for humidity. The unit of the measurement for temperature is in Celsius (C). The temperature is 23.30-degree celsius and humidity is 50 percent. as shown in figure above when the sensor is placed in room temperature.

- Checking the readings of DHT11 sensor while placing it below Dryer.
  
![Screenshot 2024-08-11 105530](https://github.com/user-attachments/assets/2787b441-def3-42db-858f-8a3db1d1e4b0)

              Test Of DHT 11 Below the dryer
The reading of temperature and humidity detected by the DHT11 sensor in LCD display is represented by “T” for temperature and “H” for humidity. The unit of the measurement for temperature is in Celsius (C). The temperature is 41.20 degree Celsius and humidity is 15.00 percentage as shown in figure above when the sensor is placed below dryer.

- Checking if the buzzer emits sound when ultrasonic sensor detects an object.
  
 ![Screenshot 2024-08-11 105539](https://github.com/user-attachments/assets/c52dcf8d-0315-450a-ba57-e2a066b90dbf)
 
		Figure : Test of Ultrasonic Sensor
When we placed an a box less than  15cm away from the ultrasonic sensor, the buzzer starting emitting sound.
