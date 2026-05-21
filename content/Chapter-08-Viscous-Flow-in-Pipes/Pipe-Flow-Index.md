---
title: "Ch08: Viscous Flow in Pipes — Index"
tags: [physics, fluid-mechanics, pipe-flow, viscous-flow, laminar, turbulent, friction-factor]
类型: directory
#flashcards
---

# Ch08: Viscous Flow in Pipes — Index

> **Core theme:** Pipe flow is everywhere — Alaskan oil pipelines, blood vessels, home plumbing, HVAC ducts. Despite the variety of applications, the underlying fluid mechanics is universal. This chapter applies mass, momentum, and energy conservation to incompressible viscous flow in closed conduits, combining exact analysis (laminar flow) with dimensional analysis + experiment (turbulent flow) to produce the **Moody chart** — one of the most-used engineering tools in existence.

| # | Topic | Description |
|---|-------|-------------|
| 8.1 | [[8.1-General-Characteristics-of-Pipe-Flow\|General Characteristics of Pipe Flow]] | Pipe vs open-channel flow, laminar/transitional/turbulent regimes, Reynolds' dye experiment, $\text{Re}_{\text{crit}} \approx 2100$, entrance region |
| 8.2 | [[8.2-Fully-Developed-Laminar-Flow\|Fully Developed Laminar Flow]] | Exact Navier–Stokes solution → parabolic velocity profile, Hagen–Poiseuille law, $f = 64/\text{Re}$ |
| 8.3 | [[8.3-Fully-Developed-Turbulent-Flow\|Fully Developed Turbulent Flow]] | Time-averaged equations, Reynolds stress, velocity defect law, law of the wall, viscous sublayer, overlap layer |
| 8.4 | [[8.4-Dimensional-Analysis-of-Pipe-Flow\|Dimensional Analysis of Pipe Flow]] | **The Moody Chart**: $f = \phi(\text{Re}, \varepsilon/D)$, Colebrook equation, laminar/smooth/transitional/fully-rough regimes, noncircular ducts and hydraulic diameter |
| 8.5 | [[8.5-Pipe-Flow-Examples\|Pipe Flow Examples]] | Single pipes: energy equation with losses, major vs minor losses, three problem types (Δp given, Q given, D given), pump/turbine inclusion |
| 8.6 | [[8.6-Pipe-Flowrate-Measurement\|Pipe Flowrate Measurement]] | Venturi, orifice plate, nozzle, rotameter, turbine meter — all using Bernoulli + discharge coefficient $C_d$ |

***

## Why This Chapter Matters

> The pipe flow problem started in [[../Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/7.1-Need-for-Dimensional-Analysis\|Ch07 §7.1]] as the motivating example for dimensional analysis. Now we solve it completely.

| Flow Regime | Analysis Method | Result |
|-------------|----------------|--------|
| Laminar ($\text{Re} < 2100$) | Exact (Navier–Stokes) | $f = 64/\text{Re}$, parabolic profile |
| Turbulent ($\text{Re} > 4000$) | Dimensional analysis + experiment | Moody chart, Colebrook formula |
| Transitional ($2100 < \text{Re} < 4000$) | Not predictable | Avoid design in this range |

***

## Interconnections

| Connection | Where |
|-----------|-------|
| **→ Ch07 Dimensional Analysis** | Reynolds number $\text{Re} = \rho V D / \mu$ first appeared in [[../Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/7.1-Need-for-Dimensional-Analysis\|Ch07 §7.1]]; the Moody chart is dimensional analysis in action |
| **→ Ch07 Similitude** | Pipe model testing uses $\text{Re}$ matching for dynamic similarity — see [[../Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/7.5-Similitude-and-Modeling\|Ch07 §7.5]] |
| **→ Ch11 Compressible Flow** | Chapter 8 is incompressible pipe flow; [[../Chapter-11-Compressible-Flow/11.7-Fanno-Rayleigh-Flow\|Ch11 Fanno flow]] extends constant-area duct analysis to compressible + friction effects |
| **→ Ch11 Nozzles** | Converging nozzles in [[../Chapter-11-Compressible-Flow/11.5-Isentropic-Flow-Through-Nozzles\|Ch11 §11.5]] are the compressible analog of pipe/channel geometry effects on flow |

> 📖 Full context → [[../../../Math/刷题仪表盘|Dashboard]]
