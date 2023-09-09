# IOT-Based-Smart-Energy-Meter-BEC
## ABSRACT
In this project, prevention of power theft can be achieved through an IoT based smart electricity energy meter using ESP32 and real time monitor data on the Blynk application. With existing technology, the user needs to go to the energy-meter reading room and take down the readings. Thus, monitoring and keeping track records of the electricity consumption is a tedious task. This can be automated, thus saving time and money by automating remote data collection.
Efficient energy utilization plays a very vital role for the development of smart grid in power systems. Therefore, proper monitoring and controlling of energy consumption is a chief priority of the smart grid. The existing energy meter system has many problems associated to it and one of the key problems is that there is no full duplex communication. To solve this problem, a smart energy meter is proposed based on the Internet of Things (IoT). The proposed smart energy meter controls and calculates the energy consumption using ESP32, a Wi-Fi module and uploads it to the cloud from where the consumer or producer can view the reading. Therefore, energy analysis by the consumer becomes much easier and controllable. 

## Problem Statement:
With a technical view, “power theft” is a non-ignorable crying that is highly prevalent, and at the same time, it directly affects the economy of a nation. Detecting and preventing such crimes with the help of the developing scientific field is the need of the hour.

## INTRODUCTION
The Internet of Things (IoT) describes the network of physical objects – “things” – that are embedded with sensors, software, and other technologies for the purpose of connecting and exchanging data with other devices and systems over the internet. These devices range from ordinary household objects to sophisticated industrial tools.  With more than 7 billion connected IoT devices today, it is expected that this number will grow up-to 22 billion in coming years.

An Energy meter is a device, which is used for measuring the energy utilized by the electric load. This energy is basically the total power consumed by the load at a particular interval of time. It is used in domestic and industrial AC circuits for measuring power consumption. 
In this project, a smart electricity energy meter using ESP32 Wi-Fi module is made, which can monitor the energy usage anytime, and from anywhere in the world. This will help the use to detect any kind of energy loss as soon as possible and also, make the whole system more controllable. 

Electricity thefts are increasing every year across domestic as well as industrial domains which affect the economic status of the country. Various wireless communication systems are available to detect the power theft, but lacks the required infrastructure needed to employ them. The project's aim is to design a system to monitor the power consumed by load and to detect and eliminate the power theft in energy meters. 

## DESCRIPTION OF PROJECT
![image](https://github.com/Abhirambs-08/IOT-Based-Smart-Energy-Meter-BEC/assets/119886477/ff3c1b06-750b-42e4-84bf-63f301ae012c)

## Components used:
- ESP32 Development Board
- ZMPT101B AC Single Phase Voltage Sensor
- SCT-013 Current Sensor
- 10k Ω Resistors
- 100Ω Resistor
- 10F Capacitor
- Bread Board
- Jumper Wires
- Bulb
- 3-pin plug

## Working-
1.	First, include the necessary libraries for ESP32 Board. EmonLib handles the retrieval of data from both sensors as well as the calculation for the RMS and power values. BlynkSimpleEsp32 integrates the program to the Blynk Mobile app.
   
3.	The EnergyMonitor object emon is created &calibration factors are defined. The Blynk timer object is then created to handle the sending of data to the Blynk mobile app.
4.	Then define the SSID & Password on our local WIFI network & insert the authentication code from the Blynk.
5.	The milli & kWh values have to be initialized. The kWh starts at 0 and will slowly go up as time goes on.
6.	The values from the sensors are being retrieved & calculated. Using emon.calcVI(20, 2000), the real power, apparent power, power factor, Vrms, and Irms are being calculated.
7.	Then use Blynk.virtualWrite to send the data to Blynk based on the virtual pins set.
8.	Under the setup function, initialize the Serial baud rate and set the current and voltage sensor analog pin as GPIO34 & GPIO35. Then set the timer to 5000L for an update time of 5 seconds.
9.	Inside the loop function run the timer and Blynk.

## RESULTS AND DISCUSSION

- When the device is offline, the readings will be set at 0.
![image](https://github.com/Abhirambs-08/IOT-Based-Smart-Energy-Meter-BEC/assets/119886477/2a88d32a-383a-4c35-9594-87251ad69038)

- Once the device is made online, the energy meter data is uploaded to Blynk Application after the interval of every 5 seconds. The data can be observed on Serial Monitor as well as Blynk Application.
![image](https://github.com/Abhirambs-08/IOT-Based-Smart-Energy-Meter-BEC/assets/119886477/c16bd92d-cc29-4f79-8c65-cd4501976bd0)

- The data is sent to the Blynk Application in real time.
![image](https://github.com/Abhirambs-08/IOT-Based-Smart-Energy-Meter-BEC/assets/119886477/9eede34f-81b2-420e-90cb-6aa9568e142e)


Energy Monitoring using IOT is an application of internet of things developed to control home appliances remotely over the cloud from anywhere in the world. In the proposed project current sensor and voltage sensor are used to sense the current and voltage and display it on internet using IoT. The system updates the information in every 5 seconds on the internet using BLYNK app. In the present system, energy load consumption is accessed using Wi-Fi and it will help consumers to avoid unwanted use of electricity. 

![image](https://github.com/Abhirambs-08/IOT-Based-Smart-Energy-Meter-BEC/assets/119886477/1b0c2730-dfce-48f3-9472-b4eb1c39fa3f)


IoT system where a user can monitor energy consumption and pay the bill Online can be made. Also, a system where a user can receive SMS, when he/she crosses threshold of electricity usage slab can be equipped. A system can be made which can send SMS to the concerned meter reading man of that area when theft is detected at consumer end. Also using cloud analytics, future predictions of energy consumptions can be made.

## CONCLUSION

This chapter projects the analysis and discussion of results and findings during and after the implementation of design. It describes in detail the final design perspective as well as highlighting the probable defects engulfing the project. 
A preview to the entirety of this project establishes the essence and need for embedded systems towards technological advancement.

The IOT based Smart Energy Meter is the anti-theft detection system. Even if theft is caught, the victim cannot get back their valuable belongings. That is why it is clear that ‘prevention is better than cure’. It is easier to stop something happening in the first place than to repair the damage after it has happened. By using this technique, crime of stealing power may be brought to an end and thereby a new bloom may be expected in the economy of our motherland and also there will be less scarcity for power utilization. 
