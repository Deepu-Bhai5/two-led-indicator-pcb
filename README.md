# Two-LED Indicator PCB

A beginner PCB design project developed in KiCad as an introduction to
the complete PCB design workflow, from schematic capture to
manufacturing file generation.

## Overview

This project is a simple two-channel LED indicator PCB.

Each LED is independently controlled through its own current-limiting
resistor, with a common ground connection.

## Objectives

- Learn the KiCad PCB design workflow
- Create and validate a schematic
- Assign and work with through-hole footprints
- Design a two-layer PCB
- Route signal and ground connections
- Perform PCB Design Rule Checks (DRC)
- Generate Gerber and drill files
- Review the design using a manufacturer's DFM checker

## Circuit

The board uses:

- 1 × 3-pin input connector
- 2 × LEDs
- 2 × 200 Ω current-limiting resistors

### Connections

- J1 Pin 1 → R1 → D1 → GND
- J1 Pin 2 → R2 → D2 → GND
- J1 Pin 3 → GND

## Design

Documentation/schematic.png

### PCB Layout

Documentation/pcb front.png
Documentation/pcb back.png

### 3D View

Documentation/pcb 3D.png

## Design Validation

The PCB was checked using KiCad's Design Rule Checker.

Validation included:

- Connectivity
- Unconnected items
- Track clearances
- Footprint geometry
- PCB outline
- Manufacturing constraints

## Manufacturing

Gerber and drill files were generated using KiCad's manufacturing
output tools.

The design was additionally reviewed using an external PCB
manufacturer's DFM checker.

## Problems Encountered

During development, several issues were identified and corrected,
including:

- Incorrect connector footprint selection
- LED polarity verification
- PCB routing issues
- Ground routing clearance
- PCB outline validation
- Solder-mask expansion requirements identified during DFM review

These issues were resolved through iterative PCB inspection and
validation.

## What I Learned

- KiCad schematic-to-PCB workflow
- Through-hole footprint selection
- PCB component placement
- Copper routing
- Ground routing
- PCB DRC
- Gerber generation
- Basic PCB manufacturing constraints
- DFM-based design iteration

## Future Improvements

- Fabricate and test the PCB
- Add input protection
- Improve silkscreen layout
- Explore a more compact PCB layout
- Develop a more functional LED indicator circuit

## Tools

- KiCad
- PCB manufacturer's DFM checker

## Project Status

**Design:** Complete  
**Electrical validation:** Complete  
**Manufacturing DFM:** Final cleanup in progress  
**Fabrication:** Pending
