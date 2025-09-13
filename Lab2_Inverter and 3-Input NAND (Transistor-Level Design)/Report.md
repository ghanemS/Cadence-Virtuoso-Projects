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

**Average Propagation Delay calculations**   
  
<img width="491" height="173" alt="image" src="https://github.com/user-attachments/assets/3133924b-9658-41f1-8b29-37bd37c0e59b" />   

<img width="522" height="209" alt="image" src="https://github.com/user-attachments/assets/abf8b405-e125-4d2d-bdb6-c194e8d3564d" />   


**Delay and Power Results**

| Circuit   | Wp (nm) | Wn (nm) | tpHL (ps) | tpLH (ps) | Avg. Delay (ps) | Avg. Power (nW) |
|-----------|---------|---------|-----------|-----------|-----------------|-----------------|
| Inverter  | 100     | 100     | 3.44      | 5.05      | 4.24            | 262             |
| Inverter  | 170     | 110     | 3.84      | 3.86      | 3.85            | 316             |
| NAND3     | 100     | 100     | 12.19     | 11.26     | 11.72           | 533             |
| NAND3     | 160     | 180     | 10.09     | 10.01     | 10.05           | 316             |
  
**Conclusion**  
- Both circuits were successfully implemented in **45nm CMOS technology**.  
- By resizing transistors, nearly equal rising and falling delays were achieved, showing how **transistor sizing affects power-performance balance** in digital VLSI design.  
