Firstly, I've decided on a few standards on what connecters i've chosen.

I chose to use the same edge card connector as is used on PCIE X16 to interconnect the boards. This is one of the most common edge card connectors. Its got plenty of pins, decent current carrying capability, and great bandwidth for digital signals. Its also easy to make the backplane standardized with ATX computer cases some day... Obviously these are ***NOT* compatible with your computer** and you should not try ot plug them in.

Because the [backplane](../Backplane/README.md) has no electronics, the ways the boards interact with each other only depends entirely on which boards you are using. I'm hoping this flexability will allow this connector to grow to meet whatever challenges are required.

I've decided to use pheonix MC 1.5 connectors with 3.81mm pitch on all of the boards so they may be externally powered externally and tested. Not all of the boards need all of these connections, and not all of the traces on all of the boards are made to handle much current, so beware.

|Pin #|Purpose|
|-----|-------|
|1|+24|
|2|-24|
|3|+12|
|4|-12|
|5|+5|
|6|GND|

