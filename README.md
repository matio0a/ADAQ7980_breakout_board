# ADAQ7980_breakout_board
A KiCad project of a breakout board design for ADAQ7980 - 16-bit 1 MSPS Analog-to-Digital converter.
The project contains the necessary symbols and footprints, as well as the schematics and PCB layout of a breakout board that can be used for rapid prototyping with ADAQ7980. 
The board features the bypass capacitors for both power rails, as well as the gain-setting resistors, and a feedback capacitor for the input driver.
The driver in the design is configured as a unity-gain buffer, and the feedback capacitor is omitted. Other values of resistors can be used to create a non-unity gain configuration, and the placeholder for the feedback capacitor is present on the board.
The pads of the bypass capacitor connected to the negative power rail should be shorted if a single-supply configuration is used (V- should be connected to GND).

Licensed under CERN-OHL-P v2.
