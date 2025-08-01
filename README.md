# 2-to-4 Decoder using CMOS in Microwind

## Project Overview

This project implements a **2-to-4 Decoder** using CMOS logic in the **Microwind VLSI layout tool**. The decoder takes 2 input signals (A and B) and activates only one of the 4 outputs (D1 to D4) based on the binary combination of inputs.

---

## Truth Table

| A | B | D1 | D2 | D3 | D4 |
|---|---|----|----|----|----|
| 0 | 0 |  1 |  0 |  0 |  0 |
| 0 | 1 |  0 |  1 |  0 |  0 |
| 1 | 0 |  0 |  0 |  1 |  0 |
| 1 | 1 |  0 |  0 |  0 |  1 |

---

## Optimized Boolean Equations

- D1 = (A + B)'
- D2 = (A + B')'
- D3 = (A' + B)'
- D4 = (A' + B')'

---

## Implementation Steps

1. **Boolean Logic Simplification**
2. **Gate-Level Schematic Design**
3. **CMOS Transistor-Level Design**
4. **Stick Diagram Drawing**
5. **Layout Design using Microwind**
6. **Simulation for all input combinations**

---

## Simulation Results

- **Rise Time:** 9 ps  
- **Fall Time:** 4 ps  
- **Propagation Delay:** 6.5 ps  
- **VOH (Output High Voltage):** 1.2 V  
- **VOL (Output Low Voltage):** 0.02 V  
- **VIH (Input High Voltage):** 0.62 V  
- **VIL (Input Low Voltage):** 0.4 V  

---

## Output Resistance

- **LOW output (NMOS ON):** ~20 KΩ  
- **HIGH output (PMOS ON):** ~40 KΩ  

---

## Tools Used

- **Microwind** (for CMOS layout and simulation)

---

## Conclusion

The CMOS 2-to-4 decoder offers a compact and power-efficient digital logic solution. Its low propagation delay and well-defined logic levels make it suitable for high-speed and low-power applications in VLSI systems.
