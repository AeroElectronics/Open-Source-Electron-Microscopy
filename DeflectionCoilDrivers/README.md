# Deflecion Coil Drivers
Deflection coil drivers are the electronics that push current into the magnetic lenses that raster the electron beam around the sample. A good deflection coil driver is high bandwidth, fast slewing, low noise, low distortion, low drift, and can operate over a large dynamic range. These constraints make practical design considerably more involved than I anticipated.

First, a few notes on deflection coil drivers generally. Since the magnetic field produced by a deflection coil is proportional to the current through it. This means that a deflection coil driver is essentially a 'transconductance amplifier' which converts a voltage signal from a DAC which indicates the demanded current, to a realized current on the coil.

Existing electron microscopes have used a variety of design approaches. I have designed several deflection coil drivers, shown below.

## Bridge topology howland current pump
The bridge topology howland current pump is essentially two power OpAmps which act to source and sink current to and from load. The load is positioned between the outputs of the two power OpAmps. With this topology the slew rate and maximum achivable voltage doubles as compared to a single ended design where one end of the load is grounded.

![Image](https://private-user-images.githubusercontent.com/195795163/405115757-e91abee4-31f4-4465-9c82-f694599c4e87)

## Single ended coil driver
Single ended coil drivers are where you control the voltage on one side of your load, and ground the other side. This is simpler than a bridge topology and easier to work with generally, but it makes the sacrifice of giving up halving the maximum voltage difference you can apply to your load. These designs are comparitively easy to work with and one require one power OpAmp and some supporting electronics.

![Image](https://github.com/user-attachments/assets/56e2b2f6-02ce-431a-912b-e7b2cb1aa7a4)
