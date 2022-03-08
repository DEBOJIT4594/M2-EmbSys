**HIGH LEVEL TEST PLAN**
======

|Test ID  |Description                                 | Input             |Expected Output          |Actual Output    |Pass/Fail |
--------------------                                   |---------------    |------------------       |---------------  |----------|-----------
|   01    | Ultrasonic distance sensor                 | Voltage = 700mV   | Generate pulses         | Generate pulses | Pass     |
|   02    | Motor should start above 1.001V            | Voltage = 1.085V  | Motor starts            | Motor starts    | Pass     |
|   03    | Red Led should not glow on or below 1.000V | Voltage = 700mV   | Do not glows            | Do not glows    | Pass     |
|   04    | Green Led should glow on or below 1.000V   | Voltage = 865mV   | Glows                   | Glows           | Pass     |
|   05    | Potentiometer                              |  5V               | 1.100V                  | 1.100V          | Pass     |


**LOW LEVEL TEST PLAN** 
====

|Test ID  |Description                                 | Input             |Expected Output          |Actual Output    |Pass/Fail |
--------------------                                   |---------------    |------------------       |---------------  |----------|-----------
|   01    | Ultrasonic distance sensor below fix point | Voltage = 700mV   | Generate pulses         | Generate pulses | Pass     |
|   02    | Ultrasonic distance sensor above fix point | Voltage = 1.085V  | Generate pulses         | Generate pulses | Pass     |
|   03    | Motor above fix point                      | Voltage = 1.085V  | Motor starts            | Motor starts    | Pass     |
|   04    | Motor below fix point                      | Voltage = 865mV   | Motor stops             | Motor stops     | Pass     |
|   05    | Red Led should not glow below fix point    | Voltage = 700mV   | Do not glows            | Do not glows    | Pass     |
|   06    | Red Led should glow above fix point        | Voltage = 1.100V  | Glows                   | Glows           | Pass     |
|   07    | Green Led should not glow above fix point  | Voltage = 1.100V  | Do not glows            | Do not glows    | Pass     |
|   08    | Green Led should glow below fix point      | Voltage = 865mV   | Glows                   | Glows           | Pass     |
|   09    | Potentiometer                              |  5V               | 1.100V                  | 1.100V          | Pass     |
|   10    | Potentiometer                              |  5V               | 680mV                   | 680mV           | Pass     |
