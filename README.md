# CH340G USB to UART Converter PCB

USB to UART/TTL converter for programming and debugging microcontrollers.

## Overview
Converts USB protocol to simple serial (TX/RX) communication.
Allows any computer to communicate with UART-based microcontrollers.

## Specifications
- Input: USB Micro-B (5V from host)
- Output: TX, RX, VCC (5V), GND via 4-pin header
- Baud rates: up to 2Mbps
- Crystal: 12MHz for precise timing
- Protection: Polyfuse on VBUS

## Components
- U1: CH340G USB to UART IC (SOIC-16)
- J1: USB Micro-B connector
- J2: 4-pin output header (TX, RX, VCC, GND)
- Y1: 12MHz crystal oscillator
- F1: Polyfuse (500mA) — overcurrent protection
- C1: 10µF decoupling capacitor
- C2, C5: 100nF decoupling capacitors
- C3, C4: 22pF crystal load capacitors

## Pinout (J2 Output Header)
| Pin | Signal |
|-----|--------|
| 1 | TX |
| 2 | RX |
| 3 | VCC (5V) |
| 4 | GND |

## Tools 
- KiCad 9
- JLCPCB design rules
- Mixed SMD and through-hole components

## Notes
- Connect TX of this board to RX of target device
- Connect RX of this board to TX of target device
- Double-sided GND pour for noise reduction

## Files Provided
- /sch - Schematic of the PCB
- /kicad - KiCad project file
- /pcb - PCB view of the file
- /gerbers - Manufacturing files ready to be fabricated
- .png of the 3D representation

## Status
Fourth PCB project. First board with SMD components and USB interface.
