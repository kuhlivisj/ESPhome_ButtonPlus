# Base module

## Controller
Brand: Espressif
Type: ESP32-S3-WROOM-1

[Datasheet](./esp32-s3-wroom-1_wroom-1u_datasheet_en.pdf)

## Connectors

### Connector J0

```
PIN		Description				Destination
1		
	2	
3		
	4	
5		
	6	I2C Address MSP A2		GND
7		
	8	I2C Address MSP A1		GND
9		
	10	I2C Address MSP A0		GND
11		
	12	
13		
	14	
15		
	16	Neopixel Data OUT		J1 #17
17		Neopixel Data IN		ESP32 #4 GPIO4
```

### Connector J1

```
PIN		Description				Destination
1		
	2	
3		
	4	
5		
	6	I2C Address MSP A2		GND
7		
	8	I2C Address MSP A1		GND
9		
	10	I2C Address MSP A0		3.3V
11		
	12	
13		
	14	
15		
	16	Neopixel Data OUT		J2 #17
17		Neopixel Data IN		J0 #16
```

### Connector J2

```
PIN		Description				Destination
1		
	2	
3		
	4	
5		
	6	I2C Address MSP A2		GND
7		
	8	I2C Address MSP A1		3.3V
9		
	10	I2C Address MSP A0		GND	
11		
	12	
13		
	14	
15		
	16	Neopixel Data OUT		J3 #17
17		Neopixel Data IN		J1 #16
```

### Connector J3

```
PIN		Description				Destination
1		
	2	
3		
	4	
5		
	6	I2C Address MSP A2		GND
7		
	8	I2C Address MSP A1		3.3V
9		
	10	I2C Address MSP A0		3.3V
11		
	12	
13		
	14	
15		
	16	Neopixel Data OUT		Extensionplate #5
17		Neopixel Data IN		J2 #16
```
