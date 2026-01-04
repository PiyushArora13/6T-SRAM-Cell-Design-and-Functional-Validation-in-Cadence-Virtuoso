# 6T-SRAM-Cell-Design-and-Functional-Validation-in-Cadence-Virtuoso

## Overview
This project presents the design and functional validation of a 6-Transistor (6T) SRAM cell at the transistor level using Cadence Virtuoso. The objective was to understand SRAM cell operation, read/write behavior, and stability using an industry-standard VLSI design environment.

The project was performed as part of hands-on learning in VLSI design and memory circuits.

---

## Objectives
- Design a transistor-level 6T SRAM cell
- Validate read and write operations using transient simulations
- Understand memory cell behavior, stability, and access mechanisms
- Gain practical experience with Cadence Virtuoso schematic and simulation tools

---

## SRAM Cell Architecture
The standard 6T SRAM cell consists of:
- Two cross-coupled inverters
- Two access transistors controlled by the word line
- Bitlines for read/write operations

The design was implemented at the transistor level using CMOS devices.

---

## Simulation and Validation

### Write Operation
- Verified successful write of logic ‘0’ and ‘1’
- Observed bitline behavior during write cycle

### Read Operation
- Verified correct data retention during read
- Observed voltage stability of storage nodes

Simulation results were validated using waveform analysis.

---

## Results
- Functional read and write operations were successfully verified
- The SRAM cell demonstrated correct bistable behavior
- Basic memory functionality was confirmed

---

## Research Context
This work was initially intended as part of a study on power–accuracy trade-offs in SRAM design. However, due to time and scope constraints, the work was limited to functional validation of the SRAM cell.

---

## Tools Used
- Cadence Virtuoso
- CMOS device models
- Transient simulation environment

---

## Limitations
- No power consumption analysis performed
- No SNM or stability sweep conducted
- No process-voltage-temperature (PVT) analysis

---

## Future Work
- Static Noise Margin (SNM) analysis
- Power and delay characterization
- Power–accuracy trade-off study
- Transistor sizing optimization
- PVT corner simulations

---

## Note
Only simulation screenshots are included due to licensing and environment constraints. This repository focuses on design intent, validation, and learning outcomes.
