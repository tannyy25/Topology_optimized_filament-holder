# Topology Optimization of a 3D-Printable Filament Holder

## Overview

This project focuses on designing and topology-optimizing a lightweight filament holder using Autodesk Fusion 360.

The original component was optimized to reduce material usage while maintaining structural stiffness. The optimized geometry was then validated using static stress finite element analysis (FEA) under a 100 N downward load.

The final geometry was prepared for additive manufacturing.

---

## Objective

- Reduce the mass of the original component.
- Maximize structural stiffness through topology optimization.
- Validate the optimized geometry using static stress FEA.
- Develop a geometry suitable for 3D printing.

---

## Design Workflow

Original CAD Model
→ Topology Optimization
→ Optimized Geometry
→ CAD Reconstruction
→ Static Stress FEA
→ Final 3D-Printable Design

---

## Topology Optimization

The topology optimization was performed in Autodesk Fusion 360.

### Optimization Parameters

| Parameter | Value |
|---|---|
| Optimization Objective | Maximize Stiffness |
| Target Mass | ≤ 30% |
| Loading | 100 N downward force |
| Constraints | Two fixed mounting regions |
| Preserved Regions | 3 |

---

## Static Stress FEA

The final optimized CAD geometry was evaluated using a Static Stress study in Autodesk Fusion 360.

### Analysis Setup

- **Load:** 100 N downward force
- **Constraints:** Fixed mounting regions
- **Simulation Material:** Steel
- **Mesh Size:** 10 mm
- **Minimum Safety Factor:** 90.45

The 10 mm mesh was used for the reported solved result.

---

## Results

### Mass Reduction

| Parameter | Original | Final Optimized |
|---|---:|---:|
| Mass | 3.627 kg | 1.192 kg |
| Mass Reduction | — | **67.1%** |

The final optimized design achieved approximately **67.1% mass reduction** compared with the original model.

### Calculation

```text
Mass Reduction =
((Original Mass - Final Mass) / Original Mass) × 100

= ((3.627 - 1.192) / 3.627) × 100

≈ 67.1%
```

---

## FEA Validation

The optimized geometry was subjected to a 100 N downward load to evaluate its structural response.

The minimum reported safety factor was **90.45** for the Steel material used in the simulation.

> **Note:** The FEA material is Steel as an assumed simulation material. The actual filament/material used for 3D printing may have different mechanical properties. Therefore, the reported FEA safety factor should not be interpreted as the safety factor of the final printed component.

---

## Tools Used

- Autodesk Fusion 360
- Topology Optimization
- Finite Element Analysis (FEA)
- Static Stress Analysis
- CAD Modeling
- STL / Additive Manufacturing

---

## Repository Structure

```text
topology-optimized-filament-holder/
│
├── CAD/
│   ├── filament_holder_original.f3d
│   ├── filament_holder_final.f3d
│   └── filament_holder_final.stl
│
├── Optimization/
│   ├── optimization_setup.png
│   ├── boundary_conditions.png
│   ├── topology_optimization_result.png
│   └── original_vs_optimized.png
│
├── FEA/
│   ├── static_stress_setup.png
│   ├── safety_factor.png
│   ├── stress.png
│   ├── displacement.png
│   └── static_stress_report.html
│
└── Results/
    └── results.md
```

---

## Key Outcomes

- **67.1% reduction in component mass**
- Topology optimized for **maximum stiffness**
- Validated using **100 N static loading**
- Final geometry reconstructed as a CAD solid
- Final design exported as **STL for additive manufacturing**

---

## Author

**Tanishq Yadav**  
B.Tech Mechanical Engineering  
Indian Institute of Technology Guwahati
