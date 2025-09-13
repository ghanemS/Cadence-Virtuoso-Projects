# Lab 2: Inverter and 3-Input NAND (Transistor-Level Design)

**Objective**  
- Design and simulate a CMOS inverter and a 3-input NAND gate at the **transistor level** in **Cadence Virtuoso (45nm CMOS)**.  
- Evaluate their propagation delays and power consumption, and optimize transistor widths for balanced rising and falling delays.

**Process**  
- Built transistor-level schematics for the inverter and NAND3 using PMOS and NMOS transistors.  
- Configured testbench with pulse inputs in **Cadence Spectre**.  
- Measured rising (tpLH) and falling (tpHL) propagation delays and average power.  
- Resized transistors (Wp/Wn) to minimize delay mismatch.  

**Results**  
- **Inverter**:  
  - Avg. delay ≈ 4.24 ps, power ≈ 262 nW.  
  - Optimized case: delay ≈ 3.85 ps, power ≈ 316 nW at **Wp=170 nm, Wn=110 nm**.  

- **NAND3**:  
  - Avg. delay ≈ 11.72 ps, power ≈ 533 nW.  
  - Optimized case: delay ≈ 10.05 ps, power ≈ 316 nW at **Wp=160 nm, Wn=180 nm**.  

- Waveforms confirmed correct inverter and NAND3 logic operation.  

**Conclusion**  
- Both circuits were successfully implemented in **45nm CMOS technology**.  
- By resizing transistors, nearly equal rising and falling delays were achieved, showing how **transistor sizing affects power-performance balance** in digital VLSI design.  

