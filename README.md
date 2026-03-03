# Rapid-Prototyping-Application-of-Additive-Manufacturing

//Transient Thermal & Structural Analysis of FDM-Printed Turbine Blade
### Simulation of Additive Manufacturing Process Using ANSYS

---

## 📌 Project Overview

This project investigates the transient thermal and structural behavior of a miniature turbine blade manufactured using Fused Deposition Modeling (FDM).

A sequentially coupled thermal–structural finite element analysis (FEA) was conducted to simulate the layer-by-layer deposition process and evaluate resulting thermal gradients, deformation, and stress distribution.

The study focuses on understanding how additive manufacturing process parameters influence structural integrity and dimensional stability.

---

## 🎯 Objective

- Simulate the FDM printing process using transient thermal analysis
- Model layer deposition using element birth and death technique
- Import temperature field into static structural analysis
- Evaluate thermal-induced deformation and stress
- Assess structural behavior of ABS turbine geometry during cooling

---

## 🛠 Software & Tools

- CAD Geometry: Design1.x_t (Turbine Blade Geometry)
- Simulation: ANSYS Mechanical 2024
- Analysis Type:
  - Transient Thermal
  - Sequential Coupled Static Structural

---

## 📐 Geometry Description

- 10-fin miniature turbine blade
- Layer-by-layer deposition (10 layers)
- Rectangular glass base plate
- Average blade surface area: ~22.95 mm²
- Mesh:
  - 15,466 elements
  - 68,857 nodes
  - Hexahedral / Tetrahedral elements
  - Element size: 0.5–1.0 mm (heat affected zone)

---

## 🔬 Materials

### Turbine Blade Material: ABS (High Impact)

- Density: 1.03 g/cm³
- Young’s Modulus: 2.2 GPa
- Poisson’s Ratio: 0.35–0.38
- Thermal Conductivity: 0.14–0.21 W/m·K
- Thermal Expansion: 72–108 × 10⁻⁶ /°C
- Melting Temperature: 220–250 °C

### Build Plate Material: Soda-Lime Glass

- Young’s Modulus: 72 GPa
- Thermal Conductivity: 0.7–1.3 W/m·K
- Thermal Expansion: 8.3 × 10⁻⁶ /°C

---

## 🌡 Transient Thermal Simulation Setup
| Initial Temperature| Heat Flow Applied per Layer | Convection Coefficient | Time Step | Total Simulation Time | 
|--------|-------| -------|-------|-------| 
| 22 °C | 1 × 10⁻⁷ W| 1.24 × 10⁻⁶ W/(m²·K)|10 seconds |100 seconds|

- Element Birth and Death used to simulate deposition

### Key Thermal Result

- Maximum Temperature: **30.406 °C**
- Heat concentrated at central hub region
- Gradual outward thermal gradient
- Cooling rate ≈ 1 °C per second in hottest region

---

## 🧱 Structural Analysis (Sequential Coupled)

- Temperature imported from transient thermal analysis
- Reference Temperature: 22 °C
- Fixed support at glass base interface
- Bonded contact between deposited layers
- Large deformation enabled

### Structural Results

| Metric | Value |
|--------|-------|
| Maximum Deformation | 0.00907 mm |
| Maximum Equivalent Strain | 0.002357 mm/mm |
| Maximum von Mises Stress | 3.8377 MPa |

Deformation was primarily observed at blade tips due to thermal expansion gradients.

---

## 🧠 Engineering Insights

- Central hub region retained highest thermal concentration
- Glass base effectively dissipated heat at build interface
- ABS demonstrated stable structural behavior under thermal loading
- Thermal strain remained within acceptable limits
- Layer-by-layer modeling captured realistic additive manufacturing effects

This simulation demonstrates how transient thermal gradients directly influence mechanical response during additive manufacturing.

---

## 🏗 Manufacturing Relevance

This study highlights:

- Process-property relationships in FDM
- Importance of thermal management in additive manufacturing
- Influence of build orientation on structural stability
- Potential for improving print strategies through simulation

---


## 🚀 Key Competencies Demonstrated

- Transient thermal modeling
- Sequentially coupled FEA
- Additive manufacturing simulation
- Contact modeling between layers
- Mesh sensitivity considerations
- Engineering interpretation of results

---

## 📎 Author

Jose Rodriguez  
Mechanical Engineering – University of Texas at Dallas  
Specialization: Simulation-Informed Additive Manufacturing  

📧 jmr180004@utdallas.edu  
🔗 LinkedIn: https://www.linkedin.com/in/jose-m-rodriguez-/
