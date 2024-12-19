# WirelessMotorControl
[Wireless Motor Control System](https://techi-news.com/Projects/Wireless-Motor-Control-System) for turning security cameras, opening gates, blinds or solar panels

Using infrared receivers and a control panel, it is necessary to provide remote control of electrical equipment control functions. 

To ensure convenient control without the need to accurately point the remote control towards the control system, several infrared receivers are installed, with overlapping fields of view.

The system controls both standard electrical equipment in on/off mode and movement/turning (using an electric motor)

## Functions
1. Control of average power (<2 kW AC, <300 W DC) equipment in on/off mode (ventilation, lighting, backlight etc.)
   
   By pressing a button on the remote control, the consumer power relay is turned on. Pressing the same button again turns off the consumer
   
1. Control of a DC motor that opens gates, blinds, rotates CCTV cameras, floodlights or rotates solar panels. Pressing a button on the remote control enables movement in one direction.
   
   The movement continues as long as the button is pressed. The second button provides movement in the opposite direction. Pressing two buttons at the same time will block movement.

   In the extreme position of the rotary mechanism, limit switches (mechanical, capacitive or other type) are installed; they block movement in corresponding direction after reaching the extreme positions.

## System parameters:
* Main controller		– Arduino Uno 
* Processor 			– 16 MGh, ATmega328P
* Controller memory		– 32 KB Flash + 2 kB SRAM + 1kB EEPROM
* IR receiver			– VS1838B
* Working frequency		– 38 KGh (940 µm)
* Maximum range		– 20m
* Viewing Angle: 		– 90 degrees
* Remote control		– 10 digital buttons + 4 control arrows + 3 service buttons
* Motor controller		– L298N
* Max motor power		– up to 48W 
* Motor voltage 			– up to 32V
* Motor current			– up to 1.5A
* Relay power			
    - 2.2 kW AC (220 V, 10A)
    - 300 W DC (30 V, 10A)
* Power supply
    - 9-12V – controller
    - 32V – Motor
    - 30V DC , 220/120V AC – Controlled loads

## Components
* Controller Arduino UNO 
* 2 channel ralay 
* IR-reciever VS1838B – 2 pcs
* IR Remote Control Kit with 17-Key Controller 
* Motor controller L298N
* Limit switches – 2pcs

## Wiring diagram

![Wiring diagram for main components](https://github.com/Brabn/WirelessMotorControl/blob/main/Wiring_diagram/WirelessMotorControl.Wiring_diagram.jpg)

## Further development of the system
* Adding additianl channels (additional motor and up to 10 controlled loads)
* Adding sound effects for feedback
* Connection to Smart home network
* Remote control of system:
    - From mobile devices (by mobile application via Bluetooth)
    - Web interface
    - Control via mobile network (SMS-informing and control commands)

