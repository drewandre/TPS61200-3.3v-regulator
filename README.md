# TPS61200 3.3v regulator with Soft Power Switch

Low-noise TPS61200 3.3v regulator with soft power circuitry.

When user depresses momentary switch, p-mosfet channel is opened and pin 6 of the TPS61200 (EN / enable pin) is pulled HIGH. This turns the regulator on and supplies a steady, low-noise 3.3v output. ***Important:*** Microcontroller needs to write a digital HIGH to the KILL pin upon startup to keep channel open and regulator turned on.

To turn, MCU should write a digital LOW to the KILL pin. This closes the p-channel mosefet and turns off regulator.
