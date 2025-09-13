# Lab 1: 4-bit Prime Number Detector & 1 Detector  

**Objective**  
- Design and simulate a 4-bit prime number detector in **Cadence Virtuoso (45nm CMOS)** that outputs logic-high for prime inputs (1, 2, 3, 5, 7, 11, 13).

**Process**  
- Constructed truth table and K-map to derive the Boolean equation.  
- Implemented schematic using **5 NOT, 7 AND, and 3 OR gates** (15 total).  
- Configured simulation in **Cadence Spectre** with periodic pulse inputs (1 ns, 2 ns, 4 ns, 8 ns).  
- Ran transient analysis for 16 ns to generate all 16 input combinations.  

**Results**  
- Output went logic-high (≈2.5 V) for prime inputs and logic-low (0 V) otherwise.  
- Simulation waveform matched the expected truth table.  

**Conclusion**    
- The 4-bit prime number detector was successfully implemented and verified in **45nm CMOS technology**.  
- This lab demonstrated schematic entry, simulation setup, and logic verification in Cadence Virtuoso.  

