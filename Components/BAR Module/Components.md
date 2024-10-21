# Components on B+ BAR Module

## Displays:

Brand: Osptek
Type: YDP096B002-V1
Protocol: SPI
Driver IC: ST7735S
Resolution: 160 (h) x 80 (v)

[Specification PDF](../Datasheets/YDP_096_B002_V1_8_P_b6210a13b6.pdf)

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
IC1-14 GP5	IC1-10 GP1				8 CS 		Chip select pin
```

## IC 1

Brand: Microchip 
Type: MCP23008
Protocol: I2C

[Datasheet](../Datasheets/MCP23008-MCP23S08-Data-Sheet-20001919F.pdf)

### IO:

```
GP0		N.C.
GP1		Chip select Display Right
GP2		Button Right
GP3		N.C.
GP4		N.C.
GP5		Chip select Display Left
GP6		Button Left
GP7		N.C.
```

## Neopixels

Neopixels are connected in series and in the folowing order:
1. Base connector #17
2. Neopixel Front Left
3. Neopixel Back Left
4. Neopixel Front Right
5. Neopixel	Back Right
6. Base connector #16

## Buttons

```
Button Left:	IC 1 # 15	GP6
Button Right:	IC 1 # 11	GP2
```

## Base connector 1

```
PIN		Description				Destination
1		GND
	2	+3.3V
3		Reset					IC 1 #4, Display #3
	4	I2C SI					IC 1 #20
5		SPI	SDA					Display #5
	6	I2C SCK					IC 1 #19
7		SPI SCL					Display #6
	8	I2C Address MSP A0		IC 1 #3
9		SPI Register select		Display #4
	10	I2C Address MSP A1		IC 1 #2
11		Backlight anode			Display #1
	12	I2C Address MSP A2		IC 1 #1
13		N.C. ??
	14	N.C. ??
15		N.C. ??
	16	Neopixel Data OUT
17		Neopixel Data IN		
```

