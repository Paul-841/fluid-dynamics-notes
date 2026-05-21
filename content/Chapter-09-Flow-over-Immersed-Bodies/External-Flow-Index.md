---
title: "Ch09: Flow over Immersed Bodies — Index"
tags: [physics, fluid-mechanics, external-flow, boundary-layer, drag, lift, aerodynamics]
类型: directory
#flashcards
---

# Ch09: Flow over Immersed Bodies — Index

> **Core theme:** External flows — objects fully surrounded by fluid — are everywhere: airplanes, cars, buildings, snowflakes, submarines. The key quantities are **lift** and **drag**, which arise from integrated pressure and shear stress distributions over the body surface. Boundary layers determine friction drag and separation (which controls pressure drag), and for lifting bodies, circulation theory explains how wings generate lift. This chapter blends exact boundary-layer theory (Blasius, von Kármán), empirical correlations, and practical drag/lift coefficient data.

| # | Topic | Description |
|---|-------|-------------|
| 9.1 | [[9.1-General-External-Flow-Characteristics\|General External Flow Characteristics]] | Coordinate systems, body classification (2D/axisymmetric/3D, streamlined/blunt), lift & drag defined via stress integrals |
| 9.2 | [[9.2-Boundary-Layer-Characteristics\|Boundary Layer Characteristics]] | Prandtl's boundary layer concept, laminar/turbulent boundary layers, Blasius exact solution, displacement & momentum thickness, von Kármán integral method |
| 9.3 | [[9.3-Drag\|Drag]] | Friction drag vs pressure drag, drag coefficient $C_D$, Reynolds number dependence, drag crisis, streamlining, separation, drag coefficients of common shapes |
| 9.4 | [[9.4-Lift\|Lift]] | Airfoil geometry, lift coefficient $C_L$, pressure distribution, circulation & Kutta-Joukowski theorem, induced drag, stall, lift-to-drag ratio |

***

## Key Physical Intuitions

> ⚠️ **External flows are qualitatively different from pipe flows:**
> - **Boundary layers grow freely** (no confining walls) — the free-stream velocity outside the BL is set by the body shape, not constant
> - **Separation** dramatically changes the flow — a streamlined body can suddenly behave like a blunt one
> - **Lift is mostly pressure, drag is mixed** — in well-streamlined bodies, drag is mostly friction; in blunt bodies, drag is mostly pressure
> - **$C_D$ and $C_L$ are not constants** — they depend strongly on $\text{Re}$ and (for lift) angle of attack

> *"A boundary layer is nature's way of reconciling the no-slip condition with inviscid flow theory."*

***

## Central Equations Summary

| Concept | Equation | Significance |
|---------|----------|-------------|
| Drag from stresses | $\displaystyle \mathcal{D} = \int p\cos\theta\,dA + \int \tau_w\sin\theta\,dA$ | (9.1) — total drag combines pressure + shear |
| Lift from stresses | $\displaystyle \mathcal{L} = -\int p\sin\theta\,dA + \int \tau_w\cos\theta\,dA$ | (9.2) — total lift combines pressure + shear |
| Reynolds number (external) | $\text{Re}_x = \dfrac{U x}{\nu}$ | Distance-based Re for boundary layer growth |
| BL thickness (laminar) | $\delta \approx \dfrac{5.0x}{\sqrt{\text{Re}_x}}$ | Blasius — exact for flat plate |
| Local skin friction (laminar) | $c_f = \dfrac{0.664}{\sqrt{\text{Re}_x}}$ | Blasius wall shear |
| Total drag coeff (laminar) | $C_{D_f} = \dfrac{1.328}{\sqrt{\text{Re}_L}}$ | Blasius, one side |
| BL thickness (turbulent) | $\delta \approx \dfrac{0.37x}{\text{Re}_x^{1/5}}$ | Empirical, $1/7$th power law |
| Local skin friction (turbulent) | $c_f = \dfrac{0.0592}{\text{Re}_x^{1/5}}$ | Empirical ($\text{Re}_x < 10^7$) |
| Total drag coeff (turbulent) | $C_{D_f} = \dfrac{0.074}{\text{Re}_L^{1/5}}$ | Flat plate, both sides |
| Total drag coeff (turbulent, high Re) | $C_{D_f} = \dfrac{0.455}{(\log_{10}\text{Re}_L)^{2.58}}$ | Schlichting correlation |
| Displacement thickness | $\displaystyle \delta^* = \int_0^\infty\!\left(1 - \frac{u}{U}\right)dy$ | Mass deficit measure |
| Momentum thickness | $\displaystyle \theta = \int_0^\infty \frac{u}{U}\!\left(1 - \frac{u}{U}\right)dy$ | Momentum deficit measure |
| Shape factor | $H = \delta^*/\theta$ | Laminar $H \approx 2.6$, turbulent $H \approx 1.4$ |
| Momentum integral eqn | $\dfrac{\tau_w}{\rho U^2} = \dfrac{d\theta}{dx} + \dfrac{(2+H)\theta}{U}\dfrac{dU}{dx}$ | von Kármán — works for any BL |
| Drag coefficient (general) | $C_D = \dfrac{\mathcal{D}}{\frac12 \rho U^2 A}$ | $A$ = frontal or planform area |
| Lift coefficient | $C_L = \dfrac{\mathcal{L}}{\frac12 \rho U^2 A}$ | $A$ = planform area for wings |
| Kutta-Joukowski lift | $\mathcal{L} = \rho U \Gamma$ | $\Gamma$ = circulation around airfoil |

---

## Flow Classification

| Regime | $\text{Re}_x$ Range | Characteristics |
|--------|-------------------|----------------|
| Laminar BL | $\text{Re}_x < 5\times10^5$ (flat plate, smooth) | Smooth, $\delta \propto x^{1/2}$, $\tau_w \propto x^{-1/2}$ |
| Transition | $5\times10^5 \lesssim \text{Re}_x \lesssim 3\times10^6$ | Instability waves (Tollmien–Schlichting), breakdown |
| Turbulent BL | $\text{Re}_x \gtrsim 3\times10^6$ | Chaotic, $\delta \propto x^{4/5}$, fuller velocity profile |

> ⚠️ Transition $\text{Re}$ depends on free-stream turbulence, surface roughness, pressure gradient.

---

## Relationship to Other Chapters

| Connection | Where |
|-----------|-------|
| **→ Ch07 Dimensional Analysis** | Drag coefficient $C_D = \phi(\text{Re})$ comes directly from [[../Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/7.4-Common-Dimensionless-Groups\|Buckingham Pi]] |
| **→ Ch07 Similitude** | Wind-tunnel model testing requires $\text{Re}$ matching — see [[../Chapter-07-Dimensional-Analysis-Similitude-and-Modeling/7.5-Similitude-and-Modeling\|Ch07 §7.5]] |
| **← Ch08 Pipe Flow** | Moody chart friction $f$ is a drag coefficient for pipes; $C_D$ for external bodies is the analog |
| **→ Ch11 Compressible Flow** | At high Mach numbers ($\text{Ma} > 0.3$), $C_D = \phi(\text{Re}, \text{Ma})$ adds compressibility effects |
| **→ Ch03 Bernoulli Eqn** | Surface pressure distribution $p(\theta)$ around airfoils/bluff bodies traces back to Bernoulli along streamlines |

> 📖 Full context → [[../../../Math/刷题仪表盘|Dashboard]]
