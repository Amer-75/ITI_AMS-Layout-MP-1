# VLSI Mini Project 1 – Custom Layout and Parasitic Analysis

This project was completed as part of the ITI Analog Mixed Signal (AMS) and Layout Training Program. It demonstrates full custom layout design and parasitic analysis for core digital cells: INVERTER 2X, NAND 2X, and NAND 4X.
The design includes manual floorplanning, hierarchical parasitic extraction (resistance, capacitance, and delay), and top-level layout integration up to Metal 3, with fully abuttable custom cells.
The project was implemented using the TSMC 65nm PDK, with Cadence Virtuoso for layout and design, and Calibre for physical verification and parasitic extraction (PEX).

---

## 🧩 Floorplanning

In floorplanning, I aimed to minimize track lengths by experimenting with orientations of custom standard cells.  
- All cells support abutment in any direction.  
- Only up to metal layer 3 was used in the entire project.

**Floorplanning Trials:**  
<img src="path/to/floorplanning-trial.jpg" alt="Floorplanning trial" width="600"/>

---

## ⚡ Parasitic Calculations

### CKOUT Signal Resistance
<img src="path/to/ckout-resistance.jpg" alt="CKOUT resistance" width="600"/>
✅ Met the specs

### Total Capacitance of CKIN and CKOUT
<img src="path/to/ckin-ckout-capacitance.jpg" alt="Capacitance" width="600"/>
✅ Met the specs

### Resistance Between QB and D
<img src="path/to/qb-d-resistance.jpg" alt="QB to D resistance" width="600"/>
✅ Met the specs

### Capacitance Calculation
<img src="path/to/capacitance.jpg" alt="Capacitance" width="600"/>
✅ Met the specs

### Div2_gated_SR_latch Internal Nodes
- SB & RB resistance — ❌ Didn't meet specs initially
- Track width changed to 0.14 μm → ✅ Met specs

<img src="path/to/sb-rb-resistance.jpg" alt="SB RB resistance" width="600"/>
<img src="path/to/adjusted-track-width.jpg" alt="Adjusted width" width="600"/>
<img src="path/to/sb-rb-capacitance.jpg" alt="Capacitance SB RB" width="600"/>

### CK Inverter Delay (Worst Case)
<img src="path/to/delay-calculation.jpg" alt="Delay calculation" width="600"/>

### Q to D Resistance (SR Latch Chain)
<img src="path/to/q-to-d-resistance.jpg" alt="Q to D resistance" width="600"/>
✅ Met the specs

---

## 🧱 Final Layouts

### INVERTER 2X  
<img src="path/to/inverter2x.jpg" alt="INVERTER 2X layout" width="600"/>

### NAND 2X  
<img src="path/to/nand2x.jpg" alt="NAND 2X layout" width="600"/>

### NAND 4X  
<img src="path/to/nand4x.jpg" alt="NAND 4X layout" width="600"/>

---

### 🧩 Top-Level Final Layout

**All Layers:**  
<img src="path/to/layout-all-layers.jpg" alt="All layers" width="600"/>

**NW, OD, and PO Together:**  
<img src="path/to/nw-od-po.jpg" alt="NW OD PO" width="600"/>

**Metal Layers:**  
- Metal 1  
  <img src="path/to/metal1.jpg" alt="Metal 1" width="600"/>
- Metal 2  
  <img src="path/to/metal2.jpg" alt="Metal 2" width="600"/>
- Metal 3  
  <img src="path/to/metal3.jpg" alt="Metal 3" width="600"/>

---

## 🧬 Final Hierarchy

<img src="path/to/final-hierarchy.jpg" alt="Final hierarchy" width="600"/>

---

## ✅ Verification

<img src="path/to/verification.jpg" alt="Verification results" width="600"/>
