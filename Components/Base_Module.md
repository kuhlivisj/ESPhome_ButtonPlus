# Base module

## Controller
Brand: Espressif
Type: ESP32-S3-WROOM-1
Driver IC: ST7735S (ESPHome compatible)

[Datasheet](../Datasheets/esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)

## Connectors

### Connector J0

```
MCP I2C address: 0x20

PIN		Description						Destination
1		GND
	2	+3.3V
3		Reset							ESP32 #3 EN
	4	I2C SI							ESP32 #24 IO47
5		SPI MOSI						ESP32 #28 IO35
	6	I2C SCK							ESP32 #25 IO48
7		SPI SCK							ESP32 #29 IO36
	8	I2C Address MSP A0				GND
9		SPI Register select				ESP32 #30 IO37
	10	I2C Address MSP A1				GND
11		Mini Display Backlight anode	ESP32 #16 IO46 (via transistor)
	12	I2C Address MSP A2				GND
13		Extensionplate...
	14	Connected with J1,2,3
15		Main Display Backlight anode	ESP32 #15 IO3 (via transistor)
	16	Neopixel Data OUT				J1 #17
17		Neopixel Data IN				ESP32 #4 IO4
```

### Connector J1

```
MCP I2C address: 0x21

PIN		Description						Destination
1		GND
	2	+3.3V
3		Reset							ESP32 #3 EN
	4	I2C SI							ESP32 #24 IO47
5		SPI MOSI						ESP32 #28 IO35
	6	I2C SCK							ESP32 #25 IO48
7		SPI SCK							ESP32 #29 IO36
	8	I2C Address MSP A0				3.3V
9		SPI Register select				ESP32 #30 IO37
	10	I2C Address MSP A1				GND
11		Mini Display Backlight anode	ESP32 #16 IO46 (via transistor)
	12	I2C Address MSP A2				GND
13		Extensionplate...
	14	Connected with J0,2,3
15		Main Display Backlight anode	ESP32 #15 IO3 (via transistor)
	16	Neopixel Data OUT				J2 #17
17		Neopixel Data IN				J0 #16
```

### Connector J2

```
MCP I2C address: 0x22

PIN		Description						Destination
1		GND
	2	+3.3V
3		Reset							ESP32 #3 EN
	4	I2C SI							ESP32 #24 IO47
5		SPI MOSI						ESP32 #28 IO35
	6	I2C SCK							ESP32 #25 IO48
7		SPI SCK							ESP32 #29 IO36
	8	I2C Address MSP A0				GND
9		SPI Register select				ESP32 #30 IO37
	10	I2C Address MSP A1				3.3V
11		Mini Display Backlight anode	ESP32 #16 IO46 (via transistor)
	12	I2C Address MSP A2				GND
13		Extensionplate...
	14	Connected with J0,1,3
15		Main Display Backlight anode	ESP32 #15 IO3 (via transistor)
	16	Neopixel Data OUT				J3 #17
17		Neopixel Data IN				J1 #16
```

### Connector J3

```
MCP I2C address: 0x23

PIN		Description						Destination
1		GND
	2	+3.3V
3		Reset							ESP32 #3 EN
	4	I2C SI							ESP32 #24 IO47
5		SPI MOSI						ESP32 #28 IO35
	6	I2C SCK							ESP32 #25 IO48
7		SPI SCL							ESP32 #29 IO36
	8	I2C Address MSP A0				3.3V
9		SPI Register select				ESP32 #30 IO37
	10	I2C Address MSP A1				3.3V
11		Mini Display Backlight anode	ESP32 #16 IO46 (via transistor)
	12	I2C Address MSP A2				GND
13		Extensionplate...
	14	Connected with J0,1,2
15		Main Display Backlight anode	ESP32 #15 IO3 (via transistor)
	16	Neopixel Data OUT				Extensionplate #5
17		Neopixel Data IN				J2 #16
```
