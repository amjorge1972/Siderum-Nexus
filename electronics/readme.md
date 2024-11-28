# Electronics

Electronics are very simple. The microcontroller is the brain. Drivers are the connection between microcontroller and steppers. And the steppers do the mecanical job. 

The ESP32 MCU (Micro Controller Unit) was chosen because of its capabilities:
- 240MHZ 32 bit dual core processor
- 448kB ROM / 520kB RAM
- 4MB storage
- Native Bluetooth, Wi Fi, PWM, Serial Comm
- 38 pin Dev Board
- popular and affordable

The stepper drivers are a very usual in 3D printers universe. This circuit board can operate with TMC2208, DRV8825, A4908 and any other with the same pinout.
A4808 are the oldest model, louder operation, 16 microsteps per step and medium current.
DRV8825 have a better current capacity, louder operation and 32 microsteps per step.
TMC2208 are very quiet, medium current and 16 microsteps per step. And could reach 256 microsteps per step using software config. But a bit more expensive.

The power supply must be 12 Volts 5 Amps. A L7809CV Voltage Regulator provides 5 Volts 1 Amp power to MCU and drives.

When continous energized, stepper motors can reach high temperatures like 70ºC and burn your skin. So CAUNTION.

Bill Of Material (BOM):
- 1 x ESP32 38 pin Dev Board (U1)
- 2 x TMC2208 Stepper Drives (DRV1, DRV2)
- 4 x 100uF 25V Eletrolictic Capacitors (C1, C2, C5, C6)
- 1 x L7805CV Voltage Regulator (U2)
- 1 x DC005 Power Jack Socket Connector (DC1)
- 2 x 4P4C PCB RJ11 Female Connector (RJ1, RJ2)
- 6 x 2.54mm Pitch Single Row Pin Female Header Socket
- 1 x Siderum Nexus PCB

The Siderum Nexus PCB Gerber file can be found at:
[Here!](https://github.com/amjorge1972/Siderum-Nexus/edit/main/electronics/Siderum-Nexus_PCB_Gerber.zip)


 
