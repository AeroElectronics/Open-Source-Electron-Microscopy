![Image](https://github.com/user-attachments/assets/91a5353a-9b69-4ae1-80f6-5a9f07e55637)

This board serves a few purposes:
1. Adding an additional series or parrallel load to the scan coil. Sometimes additional load resistance (or capacitance, will make another board soon...) can help the coil driver perform.
2. Can be used as an adjustable load with varied resistance or capacitance to test the coil over a range of inductances and resistances.
3. Can be used as an adjustable shunt resistor, which may be useful for changing magnification ranges.

When designing deflection coil drivers for open source use it is difficult to know what sort of coil inductances they may be tasked with driving. It is necessary to evaluate their performance over a large range of inductive and resistive loads. For this purpose, a board was designed which allows resistors or inductors to be switched in and out of series so that a load with varied inductance and resistance may be created. Further, in some cases it may be useful to add resistance (or capacitance, which will be covered in another board) to the coil driver’s load. 

**This is a recent design, and has not yet been tested. Please see the [status page](../Documentation/Design_Status.md).**

This board can be controlled digitally or using DIP switches when powered. When unpowered, there are solder jumpers can can be used to selectively short some loads. Beware using serious inductive loads on this board. It has not yet been tested, and large inductors can generate serious voltages if not treated properly. User beware.

Finally, also beware that it is not intended for the relays to be switched while under load. This may be possible, but the relays may be underspeced for switching under major (or possibly typical) currents. It is reccommended to turn off the load before testing.
