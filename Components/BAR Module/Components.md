# Components on B+ BAR Module

## Displays:
Brand: Osptek
Type: YDP096B002-V1
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
Brand: Microchip 
Type: MCP23008
Protocol: I2C

[Datasheet](./MCP23008-MCP23S08-Data-Sheet-20001919F.pdf)

## Base connector 1
```
PIN		Description				Destination
1
	2
3
	4
5
	6	I2C Address MSP A2		IC 1 #1
7		
	8	I2C Address MSP A1		IC 1 #2
9		
	10	I2C Address MSP A0		IC 1 #3
11
	12
13
	14
15
	16	Neopixel Data OUT
17		Neopixel Data IN
```