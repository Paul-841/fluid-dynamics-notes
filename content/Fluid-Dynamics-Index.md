---
title: "Fluid Dynamics — Index"
tags: [physics, fluid-mechanics, fluid-dynamics]
类型: directory
#flashcards
---

# Fluid Dynamics — Index

> **Core theme:** Fluid dynamics connects the mathematics of continuum mechanics to real-world fluid behavior — from incompressible pipe flows to compressible gas dynamics with shock waves.

## Chapters

| Chapter | Topic | Status |
|---------|-------|--------|
| **Ch07** | [[Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/Dimensional-Analysis-Index\|Dimensional Analysis, Similitude, and Modeling]] | ✅ Complete |
| **Ch08** | [[Chapter-08-Viscous-Flow-in-Pipes/Pipe-Flow-Index\|Viscous Flow in Pipes]] | ✅ Complete |
| **Ch09** | [[Chapter-09-Flow-over-Immersed-Bodies/External-Flow-Index\|Flow over Immersed Bodies]] | ✅ Complete |
| **Ch11** | [[Chapter-11-Compressible-Flow/Compressible-Flow-Index\|Compressible Flow (Gas Dynamics)]] | ✅ Complete |

***

## Knowledge Flow

```
Ch07: Dimensional Analysis
   │  (provides the tools: Re, Eu, Fr, Ma — and the method for creating them)
   │
   ├──→ Ch08: Viscous Pipe Flow (incompressible)
   │     uses Re + ε/D to build the Moody chart
   │     [Ch10 future: Open-Channel Flow uses Fr + Re]
   │
   ├──→ Ch09: Flow over Immersed Bodies (external flow)
   │     uses boundary layer theory + Re to predict drag and lift
   │     Separation physics ← BL state; Lift ← circulation + Kutta condition
   │
   └──→ Ch11: Compressible Flow
         uses Ma + isentropic relations
         Ch11 §11.7 Fanno flow extends pipe friction to compressible ducts
```

## Key Cross-Chapter Links

| From | To | Connection |
|------|----|------------|
| Ch08 §8.1 | Ch07 §7.1 | Reynolds number first introduced via pipe flow example |
| Ch08 §8.4 | Ch07 §7.2 | Moody chart = Buckingham Pi applied to pipes |
| Ch08 §8.4 | Ch07 §7.5 | Pipe model testing uses Re matching |
| Ch08 §8.2 | Ch11 §11.7 | Laminar pipe flow → Fanno flow (compressible counterpart) |
| Ch08 §8.5 | Ch11 §11.5 | Pipe energy equation ↔ nozzle isentropic relations (both are 1D conduit flows) |
| Ch09 §9.1 | Ch07 §7.4 | $C_D = \phi(\text{Re})$ comes from Buckingham Pi: drag coefficient is a dimensionless group |
| Ch09 §9.2 | Ch08 §8.2 | Contrast: external BL grows unbounded vs pipe BL fills duct entirely |
| Ch09 §9.4 | Ch11 §11.2 | Prandtl-Glauert compressibility correction when $\text{Ma} > 0.3$ |
| Ch09 §9.3 | Ch09 §9.4 | Lift and drag are two components of the same integrated stress tensor |

> 📖 Full context → [[../../Math/刷题仪表盘|Dashboard]]
