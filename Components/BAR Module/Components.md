# Components on B+ BAR Module

## Displays:
Osptek YDP096B002-V1
Protocol: SPI

[Specification PDF](./YDP_096_B002_V1_8_P_b6210a13b6.pdf)

### Pinout:

```
Left		Right		Common		PIN SYMBOL	FUNCTION
									1 LEDA 		Backlight anode
									2 GND 		Ground
									3 RESET 	Chip reset signal
									4 RS 		Register select signal. 0:index register; 1:data register
									5 SDA 		Serial data input pin in serial interface operation
									6 SCL 		Serial interface clock
									7 VCC(2.8V)	Analog Power Supply for LCM(2.8V)
IC1-14 GP5							8 CS 		Chip select pin
```

## IC 1
Microchip MCP23008

