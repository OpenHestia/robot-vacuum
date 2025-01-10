# Documentation of Vacuum Construction

## Microcontroller Conenctor 
(Sides were written down from the viewpoint of the robot on it's back)

* J1 power management system (battery, jack, switch)
* J2 left brush
* J3- vacuum power supply
* J4 right side sensor harness
* J5 left side sensor harness
* J6 right brush
* J7 left motor 
* J8 right motor
* J9 it blaster 

## Microcontroller Processor
This appears to be the HC89S105K8, here's the info about it

| Device      | ROM  | RAM     | I/O | Timer  | PWM             | A/D  | INT | PCA | IIC | UART | SPI | WDT | Voltage      | TEMP          | Package |
|-------------|------|---------|-----|--------|-----------------|------|-----|-----|-----|------|-----|-----|--------------|---------------|---------|
| HC89S105C8  | 64K  | 256+2K  | 41  | 16bit*2 | 12bit*3 group | 23*2 | 15  | 2   | 1   | 2    | 1   | 1   | 2.0~5.5V    | -40~+85℃     | LQFP48  |
| HC89S105S8  | 64K  | 256+2K  | 41  | 16bit*2 | 12bit*3 group | 23*2 | 15  | 2   | 1   | 2    | 1   | 1   | 2.0~5.5V    | -40~+85℃     | LQFP44  |
| HC89S105K8  | 64K  | 256+2K  | 29  | 16bit*2 | 12bit*3 group | 17*2 | 13  | 2   | 1   | 2    | 1   | 1   | 2.0~5.5V    | -40~+85℃     | LQFP32  |

The flash memory can be password protected, which might mean this is a non-starter, sadly. I am interested to see if I can flash program it though!

## Motor Controllers?
These appear to be the motor controllers used: http://www.rz-mic.com/uploadfile/fj/201810310720.pdf

## Nice Little Buzzer
https://osoyoo.com/2017/05/05/buzzer-5v-breadboard-friendlytmb12a05/
