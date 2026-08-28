USB Security Dongle

Made in EasyEDA

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

Components:

| #  | Part                        | Designators     |           Qty | Unit price |   Extended |
| -- | --------------------------- | --------------- | ------------: | ---------: | ---------: |
| 1  | 2.2 µF                      | C1,C2           |             2 |     $0.030 |     $0.060 |
| 2  | 100 nF                      | C3–C8           |             6 |     $0.005 |     $0.030 |
| 3  | USBLC6-2SC6                 | D1,D2           |             2 |     $0.184 |     $0.368 |
| 4  | SS34                        | D3              |             1 |     $0.036 |     $0.036 |
| 5  | DO2309A                     | Q1              |             1 |     $0.044 |     $0.044 |
| 6  | MMBT3904                    | Q2              |             1 |     $0.010 |     $0.010 |
| 7  | 100 kΩ                      | R1,R10,R16      |             3 |     $0.004 |     $0.012 |
| 8  | 330 Ω                       | R2,R3,R4,R5,R14 |             5 |     $0.004 |     $0.020 |
| 9  | 10 kΩ                       | R6,R13,R17      |             3 |     $0.003 |     $0.009 |
| 10 | 49.9 Ω                      | R7,R8           |             2 |     $0.003 |     $0.006 |
| 11 | 20 mΩ                       | R9              |             1 |     $0.033 |     $0.033 |
| 12 | 6.49 kΩ                     | R11             |             1 |     $0.035 |     $0.035 |
| 13 | 64.9 kΩ                     | R12             |             1 |     $0.058 |     $0.058 |
| 14 | JS203011SCQN                | SW1             |             1 |     $1.279 |     $1.279 |
| 15 | MHPA3528FRGBCT              | U2              |             1 |     $0.080 |     $0.080 |
| 16 | MHPA3528FRGBCT              | U3              |             1 |     $0.080 |     $0.080 |
| 17 | INA199A3DCKR                | U4              |             1 |     $0.475 |     $0.475 |
| 18 | LMV393IDR                   | U5              |             1 |     $0.338 |     $0.338 |
| 19 | TS3USB221ARSER              | U6              |             1 |     $0.261 |     $0.261 |
| 20 | 74LVC139D,118               | U7              |             1 |     $0.460 |     $0.460 |
| 21 | TLV75533PDBVR               | U8              |             1 |     $0.164 |     $0.164 |
| 22 | SN74LVC1G04DBVR             | U9              |             1 |     $0.095 |     $0.095 |
| 23 | SN74LVC1G08DBVR             | U10             |             1 |     $0.052 |     $0.052 |
| 24 | AM180 USB-A male            | USB1            |             1 |     $0.072 |     $0.072 |
| 25 | 11.0 180°CB1.9 USB-A female | USB2            |             1 |     $0.066 |     $0.066 |
|    | **TOTAL**                   |                 | **43 pieces** |            | **$4.143** |


PCB FAB: (its usually not this high, i dont know why its like this, maybe ill try a different provider)


<img width="1313" height="760" alt="image" src="https://github.com/user-attachments/assets/419b2054-2cf7-43c2-b735-b28e7dd7872d" />


PCB Only - 5 USD + Shipping (~23 usd) (Taxes may be more, I am in India)

Some more pics:

<img width="1140" height="421" alt="image" src="https://github.com/user-attachments/assets/b47a03a9-6b09-4c1d-8b6c-7ff79c4e0ab3" />
<img width="1152" height="391" alt="image" src="https://github.com/user-attachments/assets/d349ab9c-479c-4994-8f95-089c5ad420e7" />
<img width="1102" height="392" alt="image" src="https://github.com/user-attachments/assets/daa3eca2-a419-46fd-94b7-c071d1b16ea2" />
<img width="1169" height="827" alt="Schematic_Dongle001_2026-08-28 (1)" src="https://github.com/user-attachments/assets/d03087a6-0b5b-498b-94c3-5d31f505fb3e" />
