**HIGH LEVEL TEST PLAN**
======

|Test ID  |Description                     | Input             |Expected Output          |Actual Output    |Pass/Fail |
--------------------                       |---------------    |------------------       |---------------  |----------|-----------
|   01    | Red Led                        | Voltage = 700mV   | Do not glows            | Do not glows    | Pass     |
|   02    | Red Led                        | Voltage = 1.085V  | Glows                   | Glows           | Pass     |
|   03    | Green Led                      | Voltage = 865mV   | Glows                   | Glows           | Pass     |
|   04    | Green Led                      | Voltage = 1.400V  | Do not glows            | Do not glows    | Pass     |
|   05    | Ultrasonic distance sensor     | Voltage = 700mV   | Generate pulses         | Generate pulses | Pass     |
|   06    | Motor                          | Voltage <= 1.000V | Motor dont start        | Motor dont start| Pass     |
|   07    | Motor                          | Voltage > 1.000V  | Motor starts            | Motor starts    | Pass     |
|   08    | Potentiometer                  | 

**LOW LEVEL TEST PLAN**
====
