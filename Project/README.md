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
|LL01     | According to the level of water the sensor shall detect the distance from the water  |
|LL02     | When the water level reaches the maximum value, the motor shall turn off automatically to avoid overflowing|
|LL03     | There shall be two LEDs(Green and Red LEDs prefarebly) to indicate if the water level is full or not. Green shall indicate not full. Red shall indicate full. |

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

![autowatcont](https://user-images.githubusercontent.com/98827063/157041623-2d4f0fa5-e0e8-43ac-81dd-9f361ba988d4.jpg)


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

**APPLICATIONS**
--

1.	 It can be used in water tanks to control water level.
2.	 It can be used in factories, commercial complexes, apartments, homes, etc.
3.	 Oil tank level control.
4.	 Sea level monitoring.
5.	 Irrigation control.

