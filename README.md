# OneWireIO
Communicates with the linux [1-Wire protocol](https://en.wikipedia.org/wiki/1-Wire) device driver in order to read sensor data. Can be extended to write data.

OneWireIO uses the Raspberry Pi [1-WIRE bus interface](https://pinout.xyz/pinout/1_wire#). You need to enable the interface by adding the following line to Raspberry Pi `/boot/config.txt` file, before rebooting your Pi: 

`dtoverlay=w1-gpio,gpiopin=x`

, where `x` is is GPIO number used to connect the sensors.