
Instrumentation amplifiers for load cells (standard Wheatstone bridge 4-wire load cells)

There are two versions of the amplifier - one which is intended to be connected to an external ADC or microcontroller, eg. an Arduino, with a 5V ADC reference.
The second version has an integrated 12-bit ADC (a Microchip MCP3202, of which channel 0 is the active output channel), which is interfaced back to the microcontroller over
an SPI interface. This latter version is a slightly more complicated circuit, but it will have better resolution, less noise and better performance.

The nominal voltage output from the instrumentation amplifier on the analog-output board will be 2.5 V (half of Vcc) and it will go either up (towards 5 V) or down
(towards 0V) depending on the direction of the strain on the strain gauge, and depending on how the bridge is wired up to the board. On the digital-output board, the nominal
digital output will be 2048 (half of the maximum of 4095, from the 12-bit ADC) and it will either go up or down.

Here's an example of a readily available, low-cost load cell which may be used: http://www.seeedstudio.com/depot/weight-sensor-load-cell-0500g-p-525.html

If you need something designed for greater force, or a more robust load cell designed for industrial conditions, any standard industrial load cell, from Omega for example,
may be used.

