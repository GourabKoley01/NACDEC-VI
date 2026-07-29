# AeroIndian eVTOL Air Ambulance — Concept & Preliminary Design
**National Aerospace Concept Design Competition (NACDEC-VI) — Part 1 & Part 2**

## Overview
This repository contains the conceptual sizing, aerodynamic analysis, distributed propulsion engineering, and mission packaging documentation for the **AeroIndian**, a 1300 kg tandem-wing zero-emission eVTOL medical transport aircraft developed for **NACDEC-VI**. 

The design addresses the rapid medical evacuation mission profile by combining high-lift laminar aero-structures, active thrust vectoring via distributed electric propulsion (DEP), and a hybrid hydrogen fuel cell power architecture to minimize acoustic and environmental footprint.

---

## 🚁 Vehicle Specifications & Performance
* **Maximum Takeoff Weight (MTOW):** 1300 kg (600 kg airframe, 170 kg patient/paramedic payload, 180 kg life-support systems, 350 kg energy storage)
* **Wing Configuration:** Tandem Wing Layout
* **Airfoil Selection:** 
  * *Hover & Transition (Part 1):* NACA 6412 (Hover-optimized $L/D$)
  * *Cruise Optimization (Part 2):* NACA 642215 (Laminar flow optimization at cruise velocity of 120 km/h; wing loading 89.47 $\text{kg/m}^2$)
* **Medical Bay Dimensions:** $3.0\text{ m} \times 2.0\text{ m} \times 1.5\text{ m}$ semi-monocoque internal packaging with an integrated electric stretcher-loading system.

---

## ⚡ Distributed Electric Propulsion (DEP) & Energy Architecture
* **Propulsion Layout:** 30× VF-390 Ducted Fans (14 Front / 16 Rear)
* **Thrust Generation:** Engineered to deliver **22,500 N** of total thrust against a critical hover requirement of 22,295 N.
* **Control Philosophy:** Replaced conventional aerodynamic control surfaces with **Active Thrust Vectoring** across the distributed ducted fan array for pitch, roll, and yaw authority.
* **Power Plant:** Hydrogen Fuel Cell + High-Power Battery Hybrid Architecture, providing high specific energy while reducing acoustic noise emissions during urban hospital landing approaches.

---

## 💻 Aerodynamic CFD Analysis
Preliminary and second-iteration computational aerodynamic simulations were executed to evaluate pressure distributions, recirculation zones, and thrust-vectoring efficiency.

### Simulation Setup
* **Software:** Ansys Fluent 2020 R1
* **Solver Type:** Pressure-Based / Compressible Aerodynamics
* **Turbulence Model:** $k-\omega$ SST
* **Inlet Boundary Condition:** 33.33 m/s (Cruise velocity analysis)
* **Key Investigations:**
  * Parasitic, induced, and wave drag quantification.
  * Stagnation point and surface pressure contour mapping.
  * Slipstream interaction between ducted fan outflow and tandem-wing surfaces.

---

## 📁 Repository Structure
* `/part1/` - Conceptual sizing, mass-fraction breakdown, propulsion selection, and preliminary CFD analysis (NACDEC-VI Part 1).
  * `/part1/report/` - Complete design report documentation, CAD layouts, and performance curves.
  * `/part1/results/` - Aerodynamic pressure contours, velocity vectors, and simulation visual exports.
* `/part2/` - Advanced airfoil refinement, hybrid hydrogen energy system sizing, drag build-up, and thrust-vectoring control analysis (NACDEC-VI Part 2).

---

## ⚠️ Repository Notes & Disclaimers
> **File Size Constraints:** Raw Ansys Fluent `.cas`, `.dat`, and `.msh` mesh files have been omitted from this repository due to GitHub's individual file size limits ($>100\text{ MB}$). Complete boundary conditions, mesh refinement metrics, and solver setups are fully documented within the engineering reports in `/part1/report/`.
