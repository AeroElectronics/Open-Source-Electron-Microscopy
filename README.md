Hello!

This is not the first or last attempt at making open source electron microscopy a reality. Many others have attempted this large and difficult task before with varying specialties and contributions. I have learned a great deal from other's work in this area and it is my hope that I can make a contribution too. It is through the collective effort and ability of the open source community that progress on such large and difficult tasks may be realized.

My work so far has focused on the control electronics which can be used to drive electron microscopes. This is an essential first step that can (mostly) preceed the design of the electron optics. I'm hoping that by lowering the barrier to entry, others can work on this exciting task.

Here are several of my designs and their status:

##Deflecion Coil Drivers
Deflection coil drivers are the electronics that push current into the magnetic lenses that raster the electron beam around the sample. A good deflection coil driver is high bandwidth, fast slewing, low noise, low distortion, low drift, and can operate over a large dynamic range. These constraints make practical design considerably more involved than I anticipated.

First, a few notes on deflection coil drivers generally.
Since the magnetic field produced by a deflection coil is proportional to the current through it. This means that a deflection coil driver is essentially a 'transconductance amplifier' which converts a voltage signal from a DAC which indicates the demanded current, to a realized current on the coil.

Existing electron microscopes have used a variety of design approaches. I have designed several deflection coil drivers, shown below.

###Bridge topology howland current pump
The bridge topology howland current pump is essentially two power OpAmps which act to source and sink current to and from load. The load is positioned between the outputs of the two power OpAmps. With this topology the slew rate and maximum achivable voltage doubles as compared to a single ended design where one end of the load is grounded.


###Single ended coil driver
Single ended coil drivers are where you control the voltage on one side of your load, and ground the other side. This is simpler than a bridge topology and easier to work with generally, but it makes the sacrifice of giving up halving the maximum voltage difference you can apply to your load. These designs are comparitively easy to work with and one require one power OpAmp and some supporting electronics.


| Board  | Picture | Notes | Current design status |
| ------------- | ------------- | ------------- | ------------- |
| Bridge topology howland current pump | Content Cell  | Content Cell  | Content Cell  |
| Single ended coil driver  | Content Cell  | Content Cell  | Content Cell  |
| Adjustable load  | Content Cell  | Content Cell  | Content Cell  |
| Backplane | Content Cell  | Content Cell  | Content Cell  |
