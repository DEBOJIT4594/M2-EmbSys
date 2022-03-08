[![Codacy Badge](https://app.codacy.com/project/badge/Grade/97ae6d8938854ce68211f9ae1d962b79)](https://www.codacy.com/gh/DEBOJIT4594/M2-EmbSys/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=DEBOJIT4594/M2-EmbSys&amp;utm_campaign=Badge_Grade)

**AUTOMATIC WATER CONTROLLER** 
====================

**ABSTRACT**
--
Water is very precious for living beings and scarcity of the same is gradually increasing. Most of the cities in the country and that of the world are facing this problem. Hence, it is of utmost importance to preserve and save water. In many houses there exists unnecessary wastage of water due to overflow from overhead tanks etc. **Automatic Water Level Controller** can provide a solution to this problem.


**INTRODUCTION**
--
The **Automatic Water Level Controller** is a solution to the problem of water scarcity. In this project a microcontroller is used and it is an **Arduino Uno**. The project also consist of various components such as LEDs to indicate if the water is has reached a fix point or not. A servo motor has been used in the project .  An ultrasonic distance sensor has been used here to measure the distance and a potentiometer has been used to give analog input to the sensor.

**FEATURES**
--

1) It is easy to install
2) It easy to use 
3) Low maintenance required
4) It functions automatically
5) It saves energy by automatically turning off the motor when the tank is full.


**REQUIREMENTS**
--

**HIGH LEVEL REQUIREMENT**

|Test ID  |    Description  |  
-------------|-----------------------------------
|HL01     |    There shall be a  ultrasonic distance sensor  | 
|HL02     |    There shall be a motor        |
|HL03     |    There shall be LEDs to indicate the water level   |
|HL04     |    There shall be a potentiometer to use as analog input for sensor  |

**LOW LEVEL REQUIREMENT**

|Test ID   |  Description | 
------------------|-------------------
|LL01     | According to the level of water the sensor shall detect the distance from the water and send it to the microcontroller.  |
|LL02     | When the water level reaches the maximum fix point, the motor shall turn off automatically and when the water level is below the fix point, motor starts.|
|LL03     | The two LEDs(Green & Red) shall indicate if the water level is has cross the maximum fix point or not. |
|LL04     | The potentiometer that has been used in place of water, should send the signal to the sensor. |


**SWOT ANALYSIS**
--

__STRENGTHS__

- This system can be used to save and preserve water.

**WEAKNESSES**

- It has limited uses only.  

**OPPORTUNITIES**

- The components are easily available and easy to install. The system can be used in any household whenever needed. 

**THREATS**

- Development in this field is slow.


**5W's & 1H**
--

**WHO**

- People will use this system. 
 
**WHAT**
 
- It is a system which saves and preserve water.
 
**WHEN**
 
- Whenever the water level drops below a certain level, the Automatic Water Controller switch the motor on and shuts the motor off when rises well above a fixed level.
 
 **WHERE**
 
 - It can be install in homes, hotels, hospitals, public places, etc.

**WHY**

- To save and preserve water.

**HOW**

- This is a system which automatically control a motor to ensure a constant reserve of water.


**ARCHITECTURE**
--
**BEHAVIOURAL DIAGRAM**

![FLOWCHAT_AWC](https://user-images.githubusercontent.com/98827063/157051954-bcc73cb9-d051-4472-9b29-1d4ab4597233.jpg)


**STRUCTURAL DIAGRAM**

![STRUCTURAL_DIAGRAM](https://user-images.githubusercontent.com/98827063/157078746-f88b922f-0cc4-4e95-81b0-658a4081147e.jpg)


**BLOCK DIAGRAM**

![block diagram](https://user-images.githubusercontent.com/98827063/157061684-89b58c73-e15f-46a7-adb8-5c5a8990cf88.jpg)


**CIRCUIT DESIGN**

![autowatcont](https://user-images.githubusercontent.com/98827063/157216742-c088bc45-83c9-4b49-b40b-2a7f7f3bfc59.jpg)



**COMPONENTS**
--

**1.	MICROCONTROLLER**

_A microcontroller is needed to perform all the important operations so that the projector works fine._


**2.	SERVO MOTOR**

_It is use to control the flow of water._


**3.	ULTRASONIC DISTANCE SENSOR**

_It is used to sense the distance between itself and the surface of water._


**4.	LEDs**

_LEDs are used to indicate the water level. If the water has crossed the upper limit, green LED will glow. If the water goes below the lower limit, red light will glow.  ._


**5.	POTENTIOMETER**

_It is used in place of water to give the sensor the analog input by adjusting it_


**6.	VOLTAGE SOURCE**

_It is used to give power to the motor and potentiometer._

**7.	GROUND**

_Grounding is used to protect the equipments._

**HIGH LEVEL TEST PLAN**
======

|Test ID  |Description                                 | Input                         |Expected Output          |Actual Output    |Pass/Fail |
--------------------                                   |---------------                |------------------       |---------------  |----------|-----------
|   01    | Ultrasonic distance sensor                 | Voltage from potentiometer    | Generate pulses         | Generate pulses | Pass     |
|   02    | Motor should start                         | PWM Signal                    | Motor starts            | Motor starts    | Pass     |
|   03    | Red Led                                    | Current from microfontroller  | Do not glows            | Do not glows    | Pass     |
|   04    | Green Led                                  | Current from microcontroller  | Glows                   | Glows           | Pass     |
|   05    | Potentiometer                              |  5V                           | 1.100V                  | 1.100V          | Pass     |


**LOW LEVEL TEST PLAN** 
====

|Test ID  |Description                                                                   | Input                              |Expected Output     |Actual Output    |Pass/Fail |
--------------------                                                                     |---------------                     |------------------  |---------------  |--------- |-
|   01    | Ultrasonic distance sensor below fix point                                   | Voltage from potentiometer = 700mV | Generate pulses    | Generate pulses | Pass     |
|   02    | Ultrasonic distance sensor above fix point                                   | Voltage from potentiometer = 1.085V| Generate pulses    | Generate pulses | Pass     |
|   03    | Motor above fix point when potentiometer output is 1.085V                    | PWM Signal                         | Motor starts       | Motor starts    | Pass     |
|   04    | Motor below fix point when potentiometer output is 865mV                     | PWM Signal                         | Motor stops        | Motor stops     | Pass     |
|   05    | Red Led should not glow below fix point when potentiometer output is 700mV   | Current from microcontroller       | Do not glows       | Do not glows    | Pass     |
|   06    | Red Led should glow above fix point when potentiometer output is 1.100V      | Current from microcontroller       | Glows              | Glows           | Pass     |
|   07    | Green Led should not glow above fix point when potentiometer output is 1.100V| Current from microcontroller       | Do not glows       | Do not glows    | Pass     |
|   08    | Green Led should glow below fix point when potentiometer output is 865mV     | Current from microcontroller       | Glows              | Glows           | Pass     |
|   09    | Potentiometer                                                                |  5V                                | 1.100V             | 1.100V          | Pass     |
|   10    | Potentiometer                                                                |  5V                                | 680mV              | 680mV           | Pass     |


**RESULTS**
---

**WHEN V<=1.000V, GREEN LED GLOWS**

![below limit](https://user-images.githubusercontent.com/98827063/157216440-c6a54892-0dd2-43d3-8678-e9e8117464a8.jpg)

**WHEN V>1.000V, RED LED GLOWS**

![ABOVE LIMIT](https://user-images.githubusercontent.com/98827063/157216627-a508d114-1c6d-41ab-9d9f-30d2b7f92e43.jpg)




**APPLICATIONS**
--

1.	 It can be used in water tanks to control water level.
2.	 It can be used in factories, commercial complexes, apartments, homes, etc.
3.	 Oil tank level control.
4.	 Sea level monitoring.
5.	 Irrigation control.

