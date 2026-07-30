# LDO Voltage Regulator - 6V with 1.2V Reference Switch

## Overview

This project represents the design and implementation of a Low Drop-Out (LDO) voltage regulator capable of providing a stable 6V output together with a selectable 1.2V reference voltage.

The project includes:
- LTSpice schematic and simulations
- Breadboard implementation
- PCB design in EasyEDA
- Hardware measurements and testing

The regulator was implemented mainly using THT components available in the laboratory. The pass element of the regulator was implemented using PNP bipolar transistors instead of MOS transistors.

---

## Design Specifications

| Parameter | Value |
|---|---|
| Output Voltage | 6V |
| Reference Voltage | 1.2V |
| Dropout Voltage @100mA | 400mV |
| Current Limit | 250mA |
| Load Regulation | 10mV |
| Line Regulation | 10mV |

Additional functionality:
- Reference voltage switching using NMOS transistor
- Stable operation under variable load conditions

---

## Tools Used

### LTSpice
Used for:
- Schematic implementation
- Circuit simulations
- Parameter optimization
- Electrical analysis

### EasyEDA
Used for:
- PCB schematic recreation
- PCB layout design
- Gerber generation

---

## Circuit Description

The regulator consists of:
- 1.2V voltage reference
- Feedback network
- PNP transistor pass stage
- NMOS switching stage
- Input and output filtering capacitors

The switching stage allows selecting between:
- 6V regulated output
- 1.2V reference voltage

Several simulations were performed to validate:
- Output voltage stability
- Dropout voltage
- Load regulation
- Line regulation

---

## PCB Design

Main PCB characteristics:
- 2-layer PCB
- 1.6mm board thickness
- Mixed THT and SMD implementation
- Separate power and signal routing
- Optimized trace widths
- Test points for measurements

The PCB was designed in EasyEDA following standard routing and manufacturing constraints.

---

## Testing

The circuit was tested using:
- Breadboard measurements
- PCB measurements
- Automated tester validation

Measured parameters:
- Output voltage
- Dropout voltage
- Current consumption
- Load regulation
- Maximum output current

Several hardware issues discovered during testing were corrected during debugging and validation.
