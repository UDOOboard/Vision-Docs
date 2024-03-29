The embedded Arduino Leonardo-compatible input/output (I/O) pins operates at **5V**, with a maximum **40 mA** DC current per pin. They are located on the inner columns of the dual headers.

<a href="../img/udoo_vision_arduino_pinout.png" target="\_blank"><img style="width:400px; " src="../img/udoo_vision_arduino_pinout.png" alt="UDOO VISION Arduino pinout"></a>

Make sure to check this image to know where are the corresponding Pins  

## Technical specs

From the Arduino Leonardo page:

| | |
|-|-|
| Microcontroller |	ATmega32u4 |
| Operating Voltage	| 5V |
| Digital I/O Pins |	20 |
| PWM Channels |	7 |
| Analog Input Channels |	12 |
| DC Current per I/O Pin |	40 mA |
| DC Current for 3.3V Pin |	50 mA |
| Flash Memory |	32 KB (ATmega32u4) of which 4 KB used by bootloader |
| SRAM |	2.5 KB (ATmega32u4) |
| EEPROM |	1 KB (ATmega32u4) |
| Clock Speed |	16 MHz |


Each of the 20 digital i/o pins on the Leonardo can be used as an input or output, using pinMode(), digitalWrite(), and digitalRead() functions. They operate at 5 volts. Each pin can provide or receive a maximum of 40 mA and has an internal pull-up resistor (disconnected by default) of 20-50 kOhms.
There are six analog input pins at 10-bit resolution, providing a range of 1024 values between ground and 3.3 V. The number of inputs and resolution can be increased if required, by using an external ADC module.  

The Leonardo has 12 analog inputs, labeled A0 through A11, and all can also be used as digital i/o. Pins A0-A5 appear in the same locations as on the Uno; inputs A6-A11 are on digital i/o pins 4, 6, 8, 9, 10, and 12 respectively. Each analog input provides 10 bits of resolution (i.e. 1024 different values). By default the analog inputs measure from ground to 5 volts, though it’s possible to change the upper end of their range using the AREF pin and the [analogReference()](https://www.arduino.cc/reference/en/language/functions/analog-io/analogreference/) function.

There is a built-in LED connected to digital pin 13. When the pin is HIGH value, the LED is on, when the pin is LOW, it's off.

Analog output is simulated using pulse width modulation (PWM) on digital pins 3, 5, 6, 8, 10, 11 and 13. For an explanation of PWM, refer to the following [Arduino tutorial](https://www.arduino.cc/en/Tutorial/PWM)

The pins 3 (interrupt 0), 2 (interrupt 1), 0 (interrupt 2), 1 (interrupt 3) and 7 (interrupt 4) can be configured to trigger an interrupt on a low value, a rising or falling edge, or a change in value. See the [attachInterrupt()](https://www.arduino.cc/reference/en/language/functions/external-interrupts/attachinterrupt/) function for details.
