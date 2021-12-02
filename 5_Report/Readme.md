# REQUIREMENTS
## Introductions
Third eye for blind is a wearable device that can help the visually impaired people to move by themselves in a indoor environment. This reduces the work on people who are assisting the blind. Furthermore it also provides an opportunity for visually impaired persons to move from one place to another independently. Technology has been developing a lot these days and people are showing interest in them. This device is helpful especially when the person wants to move around a house or some indoor places by themselves. In this device, the distance of the obstacle is determined by using a Ultrasonic module and a Microcontroller. The obstacle distance is measured and informed to the visually impaired person in the form of a buzzer and vibrations. The person can move in other directions and avoid collisions using this. This project used only the microcontroller instead of using a whole  setup, so the size of the device is reduced to a large extent and the cost is also minimized. End results of the work would be a gloves with a wearable band attached to the gloves to which all the components are connected on a PCB, which works with high degree of accuracy and reliability.The objective of this project is to design a product which is very much useful to those people who are visually impaired and those who often have to rely on others. This project is an innovative one which helps the visually impaired people to move around and go from one place to another with speed and confidence by knowing the nearby obstacles using the help of the wearable band which produces the ultrasonic waves which notify them with buzz sound or vibrations. It allows the user those who are visually impaired to walk freely by detecting the obstacles. They only need to wear this device as a band or cloth on their body. Thus the aim of the project is to develop a cheap, affordable and more efficient way to help the blind people to navigate with greater comfort, speed and confidence. This is the wearable technology for the blinds which helps resolve all the problems of the existing technologies Now a days there are so many technologies and smart devices for the visually impaired people for the navigation, but most of them have certain problems for the blind people and the major drawbacks are that those things need a lot of training and efforts to use. One of the main peculiarities of this project is, it is affordable for everyone, the total cost being less than $25 or ~1500 INR. There are no such devices available in the market that can be worn like a cloth and having such a low cost and simplicity. With the use of this improvised device in a large scale, with improvements in the prototype, it will drastically benefit the community of the visually impaired or the blind people. The walking cane is a simple and purely mechanical device dedicated to detect the static or the constant obstacles on the ground, uneven surfaces, holes and steps via simple tactile-force feedback. This device is light, portable but limited to its size and it is not used for dynamic obstacle detection. These devices operate like the radar and the system of the device uses the ultrasonic waves fascicle to identify the direction and the speed of the objects. The distance between the person and the obstacle is measured by the time of the wave travel. However, all the existing systems inform the blind the presence of the object at a specific distance in-front of or near to him. These details help the user or the blind person in detecting the obstacles and thus change the way and walk accordingly. Information about the objects and their place in the way of the walking like an obstacle and their characteristics can create additional knowledge to enhance the space manifestation and memory of the blind or the visually impaired people. To overcome, the above mentioned limitations this work offers a simple, efficient, configurable virtual for the blind. The existing system consists of the devices or the supports like white cane for helping them to detect the obstacles and travel to places, pet dogs, smart devices like vision a torch for blinds. But, there were many limitations and problems in this existing systems like in the white cane, it may easily break or crack. The white cane may get stuck at the pavement cracks of the different objects. Whereas the pet dogs cost is huge and need a lot of training. In the proposed system, the design is based on a special wearable device based on the microcontroller board which can be worn like a cloth for blinds or a band. This device is equipped with ultrasonic sensor.By wearing this device, they can fully avoid the use of the white cane and such other devices. This device will help the blind to navigate without holding a stick which is a bit annoying for them. They can wear the device as a band or like a cloth and it can function very accurately and they only need a very little training to use it as it is quite simple, efficient and easy to operate and wear.As the blind person needs to know that there is an obstacle infront of him, an Ultrasonic sensor module is used to detect the obstacles. It is a transceiver which works on the principle of sonar. It transmits a high frequency sound wave signal for every 10μs. This sound signal hits the obstacle and gets reflected which is called as an echo. The duration for which this echo signal goes high is known through the echo pin of Ultrasonic module which in turn is connected to the microcontroller. The microcontroller used here is ATmega328P which is used to calculate the distance by the duration obtained from the echo pulse. The duration which is known through the echo signal covers the duration from the ultrasonic module to the obstacle and from obstacle to the ultrasonic module. So, it is divided by 2 and multiplied by the speed of the sound waves (340m/s) to get the original distance. Based on the distance, we could see the output. This entire processing is done by the microcontroller used here.

High level signal is sent for 10us using Trigger.
The module sends eight 40 KHz signals automatically, and then detects whether pulse is received or not.
If the signal is received, then it is through high level. The time of high duration is the time gap between sending and receiving the signal.
Defining our System
he module works on the natural phenomenon of ECHO of sound. A pulse is sent for about 10us to trigger the module. After which the module automatically sends 8 cycles of 40 KHz ultrasound signal and checks its echo. The signal after striking with an obstacle returns back and is captured by the receiver. Thus the distance of the obstacle from the sensor is simply calculated by the formula given as
The equation for the distance calculation between the sensor and the object is as follows:
D = (HPTW * SV)/2
Where, D = Distance in cm.
HPTW = High time of pulse width.
SV = Sound velocity in cm/s.
There are 3 output indicators here which are LED, Buzzer and Vibration Motor. These are programmed such that their output depends upon the calculated distance. For example, the buzzer buzzes rapidly when the person moves more closer towards the obstacle and it buzzes less frequently when the person is a bit far from the obstacle. Similar is the case of LED and Vibration motor. LED blinks with more delay when the person is nearer to obstacle and it blinks with less delay when he is moving away from the obstacle in the backwards direction. Distance could be set as per the choice of the user. A limit to the distance is managed after which there won’t be any of the 3 outputs seen. But one should remember that the ultrasonic sensor module used here is 3 cm to 300 cm. A regulator is being used so as to meet the specifications of the components provided in the datasheet. The regulator used is the 7805 regulator to provide 5v constant voltage.

## SWOT Analysis

### Strength
Not affected by color or transparency of objects
Can be used in dark environments
Low-cost option
Not highly affected by dust, dirt, or high-moisture environments
### Weakness
Cannot work in a vacuum
Not designed for underwater use
Sensing accuracy affected by soft materials
### Opportunity
They have greater accuracy than many other methods at measuring thickness and distance to a parallel surface
Their high frequency, sensitivity, and penetrating power make it easy to detect external or deep objects
Our ultrasonic sensors are easy to use and not dangerous during operation to nearby objects, people or equipment.
Our sensors easily interface with microcontrollers or any type of controller.
### Threats
Limited testing distance
Inaccurate readings
Inflexible scanning methods.

## High Level Requirements
RID	DESCRIPTION	STATUS
HLR1	ATMEGA 328	Implemented
HLR2	C language	Implemented
HLR3	Arduino IDE	Implemented

## Low Level Requirements
RID	DESCRIPTION	STATUS
LLR1	Ultrasonic Sensor	Implemented
LLR2	Distance measured	Implemented
LLR3	LCD Display	Implemented

## 4W's and 1'H
#### Why
The main concept of building this project is to easily detect the preset range and generate an output signal.

#### What
This project is all about the alert system towards the independent of target size, material or reflectivity.

#### Where
This project is to calculate the precise distance(s) of an object moving to and from the sensor are measured via time intervals between transmitted and reflected bursts of ultrasonic sound.

#### When
This project is going to be deployed on 2/12/2021.

#### How
With Ultrasonic Sensing’s unique advantages over conventional sensors and the rapidly increasing range of applications, ultrasonic sensors are becoming widely accepted as an industry standard across the board..
## Future Scope
In future with the advancement of quicker response of sensors, like the usage of top notch sensors it can be made lighly useful and also the modules that one needs to wear as a bracelet or on any other part of the body can be transformed into a wearable clothing like a coat, so that it can be made fit for working and there can be more advancement in this device for instance we can use piezeo electric plates in the shoes of the user which can generate sufficient electricity that the modules can run on. 

## DESIGN

## Block Diagram
![pic1 drawio](https://user-images.githubusercontent.com/94293980/144221264-d1876502-a6c3-4242-8b84-9c81e9e496ca.png)

## Structural Diagrams
![image](https://user-images.githubusercontent.com/94293980/144080159-4e3b13be-e388-4e4e-9206-0e41529b227c.png)

## Behavioural Diagrams
![flowchart](https://user-images.githubusercontent.com/94293980/144221697-fdd155cf-626f-4717-a30f-ba11d7842d49.png)

![download](https://user-images.githubusercontent.com/94293980/144234063-c00b5856-d1d9-4b04-8b1c-36eb9519d189.png)

