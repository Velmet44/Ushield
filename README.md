USB Security Dongle

A compact hardware USB dongle that lets you physically control whether a connected USB device receives power, data, or nothing at all.

It has three modes:

Mode	Power	Data
OFF	No	No
POWER ONLY	Yes	No
POWER + DATA	Yes	Yes

The entire device works in hardware, with no software, drivers, or companion application required.

Features
3-position physical mode switch
USB 2.0 data switching
USB power switching
USB ESD protection
Current sensing and power monitoring
RGB status indicators
Compact 4-layer PCB
No MCU required
How It Works

The USB data lines pass through a dedicated USB 2.0 switch, allowing them to be disconnected while leaving power available.

The power path is controlled separately using a P-channel MOSFET. This makes it possible to completely disable the downstream USB port when the switch is in the OFF position.

The current flowing to the connected device is measured using a low-value shunt resistor and current-sense amplifier. Comparator and logic circuitry are used to process the power-monitoring signals and control the status indicators.

Modes
OFF

The downstream USB port is completely disabled.

No USB power
No USB data
POWER ONLY

The connected device can receive power, but the USB data lines remain disconnected.

This is useful for charging a device without allowing USB data communication.

POWER + DATA

The dongle behaves like a normal USB connection, with both power and USB 2.0 data available.

Hardware

The design includes:

USB-A male connector
USB-A female connector
TS3USB221A USB data switch
TLV75533 3.3 V regulator
P-channel MOSFET power switching
INA199 current-sense amplifier
LMV393 comparators
74LVC139 logic
SN74LVC1G04 inverter
SN74LVC1G08 AND gate
MMBT3904 transistor
USBLC6-2 ESD protection
RGB LEDs
3-position switch
Current-sense and threshold resistors
Decoupling capacitors
Design Goals

The main goals of the project were to make a USB security tool that is:

Fully hardware based
Easy to use
Small enough to carry around
Useful without installing anything
Capable of completely disabling USB access when required
PCB

The board uses a 4-layer design with separate attention given to the USB differential pair, power routing, and analog sensing circuitry.

The USB data path is kept short and routed separately from the more noisy power and control circuitry.

CAD

The enclosure and mechanical assembly files are included in the repository along with the PCB source and manufacturing files.

The complete BOM, including quantities, supplier links, component prices, and shipping costs, is included in the repository.

Project Status

The project is complete, including the schematic, PCB, firmware-free hardware design, enclosure, and manufacturing files.

License

See the repository for the license and individual component/library licensing information.
