# Functional Validation of SRAM Cell Design

## Objective
The objective of this validation was to verify the correct functional behavior of the SRAM cell at the schematic level using Cadence Virtuoso. The focus was on confirming reliable read, write, and hold operations as a baseline before extending the work toward approximate computing and power–accuracy trade-off analysis.

This validation supports the foundational concepts discussed in the associated research paper on approximate SRAM for Edge AI applications.

---

## Write Operation Validation

### Write ‘0’
- Word Line (WL) asserted high
- Bit Line (BL) driven low, Bit Line Bar (BLB) driven high
- Internal storage node Q transitions to logic ‘0’
- Complementary node Q̄ transitions to logic ‘1’

**Observation:**  
The simulation waveform confirms a clean and deterministic state transition, indicating sufficient access transistor strength to override the cross-coupled inverter feedback.

---

### Write ‘1’
- WL asserted
- BL driven high, BLB driven low
- Q transitions to logic ‘1’, Q̄ to logic ‘0’

**Observation:**  
Minimal metastability or signal disturbance is observed, confirming correct writability at the schematic level.

---

## Read Operation Validation

- Both BL and BLB are precharged to VDD
- WL is asserted
- Stored ‘0’ node weakly discharges its corresponding bit line
- Voltage differential appears without disturbing stored data

**Observation:**  
The read waveform shows stable internal nodes (Q and Q̄), indicating absence of read disturb and adequate read Static Noise Margin (SNM) for the baseline design.

---

## Hold Operation Validation

- WL deasserted (logic low)
- Bit lines isolated from the cell
- Cross-coupled inverters retain stored value

**Observation:**  
Q and Q̄ remain stable over time, confirming reliable data retention in hold mode.

---

## Validation Summary

| Operation | Status |
|---------|--------|
| Write 0 / Write 1 | Verified |
| Read stability | Verified |
| Hold stability | Verified |
| Power metrics | Not extracted |
| SNM quantification | Planned extension |

---

## Relation to Research Work
These functional results form the baseline SRAM behavior referenced in the research paper prior to introducing stepwise transistor scaling and approximation for power–accuracy trade-off analysis.

