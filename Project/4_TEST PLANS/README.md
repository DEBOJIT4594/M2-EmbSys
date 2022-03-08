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
