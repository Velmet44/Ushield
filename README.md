# USB Security Dongle

**Made In EasyESA**

A compact hardware USB dongle that lets you physically control whether a connected USB device receives power, data, or nothing at all.

## Modes

| Mode | Power | Data |
|---|---|---|
| OFF | No | No |
| POWER ONLY | Yes | No |
| POWER + DATA | Yes | Yes |

The device works entirely in hardware. No software, drivers, firmware, or companion application are required.

## Features

- 3-position physical mode switch
- USB 2.0 data switching
- USB power switching
- USB ESD protection
- Current sensing and power monitoring
- RGB status indicators
- Compact 2-layer PCB
- No MCU

## How It Works

The USB data lines are routed through a dedicated USB 2.0 switch, allowing the data connection to be disabled while power remains available.

The downstream power path is controlled separately with a P-channel MOSFET. This allows the downstream USB port to be completely disabled in OFF mode.

A low-value shunt resistor and current-sense amplifier measure the current delivered to the connected device. Comparator and logic circuitry process the measured voltage and control the power status indicators.

## Modes

### OFF

- No USB power
- No USB data

### POWER ONLY

- USB power available
- USB data blocked

This can be used to charge a device without providing a USB data connection.

### POWER + DATA

- USB power available
- USB 2.0 data available

The dongle operates like a normal USB connection.

## Hardware

The main components include:

- USB-A male connector
- USB-A female connector
- TS3USB30E USB 2.0 switch
- TLV75533 3.3 V regulator
- DO2309A P-channel MOSFET
- MMBT3904 transistor
- INA199A3 current-sense amplifier
- LMV393 dual comparator
- 74LVC139 logic decoder
- SN74LVC1G04 inverter
- SN74LVC1G08 AND gate
- USBLC6-2 ESD protection
- C&K 3-position switch
- Two RGB LEDs
- Current-sense and threshold resistors
- Decoupling capacitors

## PCB

The PCB is a compact 2-layer board.

The USB data path is kept short, with the USB 2.0 switch and ESD protection placed close to the USB connectors. Power switching and current sensing are separated from the USB data path as much as practical.

## CAD

The repository contains the enclosure and mechanical assembly files, including the complete assembly and source CAD files.

## Bill of Materials

The complete BOM is included in the repository with component quantities, manufacturer and supplier part numbers, footprints, prices, and supplier information.

# Quote

<img width="1816" height="857" alt="image" src="https://github.com/user-attachments/assets/98f586ec-f5e8-4274-9c5b-7c6c34f8b289" />
<img width="1746" height="872" alt="image" src="https://github.com/user-attachments/assets/ec5921fb-076b-42e7-b4bc-18376fa67c95" />

## Project Status

Complete.

The schematic, PCB, manufacturing files, etc are finished.
