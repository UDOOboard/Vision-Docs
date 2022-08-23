The **GPIO** (*General-Purpose Input/Output*) peripheral provides dedicated general-purpose pins that can be configured as either inputs or outputs.
When configured as an output, it is possible to write to an internal register to control the state driven on the output pin. When configured as an input, it is possible to detect the state of the input by reading the state of an internal register. In addition, the GPIO peripheral can produce CORE interrupts.

**UDOO Vision** features a total of **20** GPIOs available on the external Pinout connectors.
Those GPIOs are available in the internal Arduino Pinout columns manageable from the Microchip ATmega32U4 processor of the Arduino Leonardo embedded. These Pins are *5V only compliant*.

In the following image you can see 20 GPIOs manageable from the main ATmega32U4(Arduino Leonardo-compatible embedded) and their functions.

**TODO: add correct image**

Refer to the [Arduino Leonardo (ATmega32U4)](!/Arduino_Leonardo-compatible(ATmega32U4)/Overview) section to manage the Arduino GPIOs. You will be able to use the internal row pinout exactly like you do with an Arduino Leonardo.