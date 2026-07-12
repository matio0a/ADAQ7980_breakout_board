# ADAQ7980_breakout_board
A KiCad project of a breakout board design for ADAQ7980 - 16-bit 1 MSPS Analog-to-Digital converter.
The project contains the necessary symbols and footprints, as well as the schematics and PCB layout of a breakout board that can be used for rapid prototyping with ADAQ7980. 

**Board description:**
  - ADAQ7980 pins are accessible through the external pin headers.
  - The IN+ pin is additionally accessible through the on-board SMA-connector. The input pin is 50 Ohm-terminated.
  - A 4.096 V precision voltage reference (ADR4540) is used to fix the ADC range.
  - The input amplifier is configured as a unity-gain buffer. Footprints for gain-setting resistors as well as for a feedbac capacitor are present. The unity-gain setting is achieved by soldering a 0-Ohm SMD resistor instead of R2.
  - A 47k resistor is soldered between VIO and SDO pins to create an additional "Busy" signal on the SDO line. This feature can be turned off by tying the SDO line to VIO directly.
  - A green LED is present to indicate the power on condition.
  - SDI line is accessible through the dedicated pin header. Place a jumper between SDI and VIO to operate in a 3-wire SPI mode.
  - V- line is accessible through the dedicaed pin header. Place a jumper between V- and GND pins to operate in a single-supply mode.

**To do:**
  - Redo the board layout.
  - Create production files.

Licensed under CERN-OHL-P v2.
