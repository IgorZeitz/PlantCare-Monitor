# PlantCare Monitor 🌱

A compact environmental monitoring and plant-care system based on the ATmega328P microcontroller.
The device monitors:
- temperature,
- air humidity,
- soil moisture,
- gas concentration.
  
 ## Features
The device presents sensors sampled data on a 16x2 LCD display, controlled via a tactile switch. Real time environmental monitoring allows the unit to trigger alarms when high concentration of toxic gas are detected and to start automatic plant watering when soil moisture drops below a defined threshold.

💧🚿 *Watering Logic:*
>
The soil is continuously monitored. If moisture falls below a configured threshold, the transistor switches on the 5 V pump. Water is delivered to the pot through a silicone tube. The pump turns off once soil moisture returns to safe level.

🚨⚠️ *Gas Alarm Logic:*
>
When the gas sensor detects a harmful concentration level, an alarm routine is triggered. A buzzer emits a loud signal, a red LED lights up and an alert message appears on the LCD.

<div align="center">
  <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/schema.png" alt="Schema">
</div>

## PCB

The device Pritned Circuit Board was custom designed and manually etched with termotransfer method with laminate, a laser printer and B327 mixed with water. The board includes routing for all sensors, external connectors for pump and inputs. Additional pads for debug and programming interfaces were added (SPI and UART). The device is powered via USB-C.

| PCB design | PCB etching | Final PCB |
|:----------:|:------------------:|:-----:|
| <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/pcb.png" width="600" height="438"> | <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/wytrawiona.jpeg" width="600" height="435"> | <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/wywiercona.jpeg" width="600" height="433"> |

## Enclosure

The PCB is housed in a custom 3D printed enclosure made from PLA. The design includes slots for used sensors, wiring responsible for the pump and soil moisture sensor probe and a window for the LCD display. Some additional cutouts were added for LEDs and the tact switch.

| 3D model | Device hardware |
|:--------:|:---------------:|
| <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/Case.png" width="480" height="270"> | <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/z%C5%82o%C5%BCony.jpeg" width="480" height="601"> |
| Front cover 3D model | Device front cover |
| <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/CaseTop.png" width="480" height="270"> | <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/obudowa.jpeg" width="480" height="368"> |

## Final Device

| Prototype | Final version|
|:------------------:|:-----:|
| <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/prototypowy-w%C5%82%C4%85czony.jpeg" width="768" height="1024"> | <img src="https://github.com/IgorZeitz/TEST/blob/test2/images/w%20obudowie.jpeg" width="1024" height="768"> |
