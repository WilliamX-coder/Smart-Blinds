# Roadmap

## Sprint 1

## Repos
- [x] Get 1 inspired repo from Gtihub - Joe  
- [x] Get 1 inspired repo from Github - William

- [Smart-Blinds/brizdotdev](https://github.com/brizdotdev/Smart-Blinds)  
- [automatic-roller-blinds-motor/asafteirobert](https://github.com/asafteirobert/automatic-roller-blinds-motor)

## Hardware
- [x] find out what hardware brizdotdev is using - Joe
- [x] find out what hardware asafteirobert is using - William  
### (Smart-Blinds/brizdotdev)
- Raspberry Pi Model 3
- 4x AA Batteries
- Continuous Rotation Servo (SM-4303r) - (This will spin the wand to open and close the blinds)
- [3D Printed gear](http://www.thingiverse.com/thing:867) - (This is intended for "roller blinds", we will not be using these)

### (automatic-roller-blinds-motor/asafteirobert)
-small remote, web interface or RESTful API
-Arduino pro mini 
- Arduino Pro Mini 3v3
- 28BYJ-48 5V stepper motor
- 0805 1uf SMD capacitor
- 100uF(or higher) 25V SMD type D electrolytic capacitor
- 470uf 6V SMD size C tantalum or type D electrolytic capacitor
- NRF24L01+	SMD module
- A4988 or DRV8825 Stepper Motor Driver module
- 9V power supply (recommended 0.5A multiplied by the number of roller blinds)
- Power supply connector (usually DC2.5/5.5)(optional)
- Wire for connecting power
- Pair of XH 2.54mm 2-pin connectors (optional)
- 3D printed parts found in `3d print` folder. 1x motor adapter and 1x mount(or mount-mirrored)
- PCB
- 2x M2x5 screws
- 2x M3x6 screws
- 2x M3 nuts (optional)
## Software  
- [x] find out what software brizdotdev is using - Joe
- [x] find out what software asafteirobert is using - William

### (Smart-Blinds/brizdotdev)
- [Raspbian](https://www.raspberrypi.org/downloads/raspbian/) - "Your Raspberry Pi needs an operating system to work. This is it. Raspberry Pi OS (previously called Raspbian) is our official supported operating system."


### (automatic-roller-blinds-motor/asafteirobert)
-order the PCB from this link: https://www.pcbway.com/project/shareproject/Automatic_roller_blinds_motor.html-roller -blinds can be controlled wirelessly using a NRF24L01 module. Controlled either by a small remote, web interface or RESTful AP, built around an Arduino pro mini and a cheap stepper motor.
-Arduino Uno

## Errors: 
- [x] Clone, test, and document any setup or issues with brizdotdev's code - Joe
- [x] Clone, test, and document any setup or issues asafteirobert's code - William

(Smart-Blinds/brizdotdev):  
Traceback (most recent call last):  
  File "c:\Users\Joe\Documents\GitHub\Smart-Blinds Insparation\brizdotdevSmart-Blinds\Smart-Blinds\blinds.py", line 4, in <module>  
    import RPi.GPIO as GPIO  
ModuleNotFoundError: No module named 'RPi'

### (automatic-roller-blinds-motor/asafteirobert):
#include <EEPROM.h>
 EEPROM.get(...);
 EEPROM.put(...);
 this Stores the value 123 at EEPROM address 0
 
## Possible Error cause:  
### (Smart-Blinds/brizdotdev) 
It’s trying to import RPi.GPIO, which is only available on Raspberry Pi hardware.

### (automatic-roller-blinds-motor/asafteirobert)
this is trying to include the Arduino EEPROM and load it into an object

## Possible Error fix:  
### (Smart-Blinds/brizdotdev)
import RPi.GPIO as GPIO

### (automatic-roller-blinds-motor/asafteirobert)
Need to upload code to microcontroller like an Arduino Uno

## Sprint 2

## Sprint 3

## Sprint 4
