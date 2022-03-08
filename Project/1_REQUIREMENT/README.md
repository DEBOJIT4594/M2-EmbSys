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
