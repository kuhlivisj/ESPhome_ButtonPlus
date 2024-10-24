# ESPhome_ButtonPlus

*ESPHome documentation and examples to make ESPHome working on the Button+*

## Status

For now, the diplays, the neopixel LED's and the buttons are working. See the examples folder for the first example. Please reffer the ESPHome documentaion for more information on how to build your own menu or ... (?)
> https://esphome.io/components/display/
> https://esphome.io/components/font#display-fonts

Want to help? Pull requests are welcome!

## Button+

The Button+ is a modular control panel designed to work with MQTT. It has a "Main display" and "BAR modules" where the position and amount  can be changed according your needs. You can order it on there [website](https://button.plus).

## TODO:

- [x] Neonleds
	- [x] figure out how to control them individually. [> maybe with Light Partition](https://esphome.io/components/light/partition)
	- [x] find correct [type](https://esphome.io/components/light/neopixelbus.html#configuration-variables)
- [ ] Temperature sensor STS35
- [ ] Documentation
- [ ] More examples
