# samsung-riscv
Task 5
Temperature-Controlled Fan

The Temperature-Controlled Fan project integrates a temperature sensor (LM35) with the CH32V003 RISC-V processor to create an automated fan system. The system monitors ambient temperature in real-time and adjusts the fan's speed accordingly. The LM35 temperature sensor detects the surrounding temperature and sends an analog signal to the CH32V003 processor, which then generates PWM signals to control the fan's speed. This project provides an energy-efficient solution by ensuring the fan operates only when needed and at appropriate speeds.

Components Required
CH32V003 RISC-V processor
LM35 temperature sensor
Small DC fan (5V)
Transistor (e.g., BC547)
Resistors (e.g., 10kΩ, 1kΩ)
Power supply
Breadboard
Jumper wires
Circuit Connection
Connecting the LM35 Sensor:
VCC (Pin 1): Connect to the 3.3V pin of the CH32V003 processor.
OUT (Pin 2): Connect to an ADC pin (e.g., A0) on the processor.
GND (Pin 3): Connect to the ground (GND) of the processor.
Connecting the DC Fan:
Positive Terminal: Connect to the 5V power supply via the transistor (see below).
Negative Terminal: Connect to GND.
Use a BC547 transistor to control the fan's operation:

Base: Connect to a 1kΩ resistor, which is then connected to the PWM pin (e.g., D2) of the CH32V003 processor.
Collector: Connect to the negative terminal of the fan.
Emitter: Connect to GND.
Power Supply:
Provide 3.3V to the CH32V003 processor and 5V for the DC fan.

Component	
CH32V003 - Pin
LM35 - Sensor	
VCC	- 3.3V (VIN)
OUT -	A0 (ADC)
GND	- GND
DC Fan	
Positive Terminal	- 5V Power Supply
Negative Terminal	- Collector (via BC547)
BC547 - Transistor	
Base - D2 (PWM via 1kΩ)
Collector	Fan - Negative Terminal
Emitter -	GND
