# Components on B+ Display Module

## Display:

Brand: Shenzen Surenoo
Type: YT280S030 (STP0280B2-240320)
Protocol: SPI
Driver IC: ST7789V
Resolution: 320 (h) x 240 (v)

[Datasheet](../Datasheets/STP0280B2-240320.pdf)

## IC 1

Brand: Microchip 
Type: MCP23008
Protocol: I2C

[Datasheet](../Datasheets/MCP23008-MCP23S08-Data-Sheet-20001919F.pdf)

### IO:

```
GP0		Display Backlight Cathode	Display	#11,12,13,14
GP1		Display Backlight Cathode	Display	#11,12,13,14
GP2		Button Right
GP3		N.C.
GP4		N.C.
GP5		Display Chip Select		Display #5
GP6		Button Left
GP7		Display Backlight Cathode	Display	#11,12,13,14
```
## Base Connectors

### CN0

```
PIN		Description
1		N.C.
	2	N.C.
3		N.C.
	4	N.C.
5		N.C.
	6	N.C.
7		N.C.
	8	N.C.
9		N.C.
	10	N.C.
11		N.C.
	12	N.C.
13		N.C.
	14	N.C.
15		N.C.
	16	Neopixel Data OUT > directly to pin 17
17		Neopixel Data IN  > directly to pin 16
```

### CN1

```
PIN		Description
1		N.C.
	2	N.C.
3		N.C.
	4	N.C.
5		N.C.
	6	N.C.
7		N.C.
	8	N.C.
9		N.C.
	10	N.C.
11		N.C.
	12	N.C.
13		N.C.
	14	N.C.
15		N.C.
	16	Neopixel Data OUT > directly to pin 17
17		Neopixel Data IN  > directly to pin 16
```

### CN2

```
PIN		Description			Destination
1		GND				GND
	2	+3.3V				+3.3V
3		Reset				IC 1 #4, Display #2
	4	I2C SI				IC 1 #20
5		SPI	MOSI			Display #6
	6	I2C SCL				IC 1 #19
7		SPI SCK				Display #3
	8	I2C Address MSP A0		IC 1 #3
9		SPI Register select		Display #4
	10	I2C Address MSP A1		IC 1 #2
11		Backlight anode			Display #1
	12	I2C Address MSP A2		IC 1 #1
13		Extensionplate...		-
	14	Connected with J0,2,3		-
15		Main Display Backlight anode	-
	16	Neopixel Data OUT		-
17		Neopixel Data IN		-
```
