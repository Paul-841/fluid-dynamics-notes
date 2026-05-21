---
title: "Ch07: Dimensional Analysis, Similitude, and Modeling — Index"
tags: [physics, fluid-mechanics, dimensional-analysis, similitude, modeling, buckingham-pi]
类型: directory
#flashcards
---

# Ch07: Dimensional Analysis, Similitude, and Modeling — Index

> **Core theme:** Many fluid mechanics problems cannot be solved by analysis alone and rely on experimental data. Dimensional analysis is a **packaging technique** that reduces the number of variables in an experimental program, making results simpler, cheaper, and more general. The **Buckingham pi theorem** tells us how many dimensionless groups replace the original variable list, and **similitude** allows model-test results to predict full-scale behavior.

| # | Topic | Description |
|---|-------|-------------|
| 7.1 | [[7.1-Need-for-Dimensional-Analysis\|The Need for Dimensional Analysis]] | Why experimentation is necessary, the pipe flow example, how dimensionless groups simplify experiments |
| 7.2 | [[7.2-Buckingham-Pi-Theorem\|Buckingham Pi Theorem]] | The fundamental theorem: dimensionally homogeneous eqn with $k$ variables → $k-r$ independent dimensionless products |
| 7.3 | [[7.3-Determination-of-Pi-Terms\|Determination of Pi Terms]] | Systematic methods for finding dimensionless groups from a list of variables |
| 7.4 | [[7.4-Common-Dimensionless-Groups\|Common Dimensionless Groups in Fluid Mechanics]] | Reynolds, Froude, Euler, Mach, Weber numbers — when each matters |
| 7.5 | [[7.5-Similitude-and-Modeling\|Similitude and Modeling]] | Geometric, kinematic, dynamic similarity; scaling laws; distorted models |
| 7.6 | [[7.6-Applications-of-Model-Studies\|Applications of Model Studies]] | Practical examples: pipe flow, drag on bodies, hydraulic structures, pumps/fans |

***

## Key Physical Intuitions

> ⚠️ **Dimensional Analysis — What It Is and Isn't:**
> - ⬜ **It is** a compacting technique — reduces many variables to fewer dimensionless groups
> - ⬜ **It is** a guide for efficient experimental design
> - ⬜ **It is not** a complete solution — the final answer still comes from experiments or numerical methods
> - ⬜ **It is not** a way to find unique functional forms — only the *organization* of variables

> *"Dimensional analysis is like a trash compactor: it reduces volume for easier handling, but doesn't dispose of the trash."*

***

## Key Equations Summary

| Concept | Dimensionless Group | Significance |
|---------|-------------------|--------------|
| Pipe pressure drop | $\frac{D \Delta p_\ell}{\rho V^2} = \phi\!\left(\frac{\rho V D}{\mu}\right)$ | 5 variables → 2 groups |
| Buckingham Pi Theorem | Number of $\Pi$ groups = $k - r$ | $k$ = #variables, $r$ = #reference dimensions |
| Reynolds number | $\text{Re} = \dfrac{\rho V D}{\mu}$ | Viscous effects / turbulence transition |
| Froude number | $\text{Fr} = \dfrac{V}{\sqrt{g L}}$ | Free-surface / gravity effects |
| Euler number | $\text{Eu} = \dfrac{\Delta p}{\rho V^2}$ | Pressure/inertia ratio |
| Mach number | $\text{Ma} = \dfrac{V}{c}$ | Compressibility effects |
| Weber number | $\text{We} = \dfrac{\rho V^2 L}{\sigma}$ | Surface tension effects |

---

## Dimensional Systems

| System | Base Dimensions |
|--------|----------------|
| **MLT** | Mass $M$, Length $L$, Time $T$ |
| **FLT** | Force $F$, Length $L$, Time $T$ (via $F \doteq MLT^{-2}$) |

> Conversion: $F = MLT^{-2}$ → express mass-dimensioned quantities in terms of $F$, $L$, $T$.

---

## Relationship to Other Chapters

- **Ch. 1** — Fundamental dimensions and units
- **Ch. 8** — Pipe flow (application of Reynolds-number-based correlations)
- **Ch. 9** — External flows / drag (drag coefficient is a dimensionless group)
- **Ch. 11 (Compressible Flow)** — Mach number regimes, Reynolds-number effects in compressible flows

> 📖 Full context → [[../../../Math/刷题仪表盘|Dashboard]]
