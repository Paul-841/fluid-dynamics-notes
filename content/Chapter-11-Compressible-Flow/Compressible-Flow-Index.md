---
title: "Compressible Flow — Index"
tags: [physics, fluid-mechanics, compressible-flow, gas-dynamics]
类型: directory
#flashcards
---

# Compressible Flow — Index

> **Core theme:** When a fluid moves fast enough that density changes become non-negligible, incompressible flow assumptions break down. Compressible flow introduces the **speed of sound** as a reference velocity (Mach number), **isentropic relations** connecting pressure/density/temperature, and exotic phenomena — choking, shock waves, friction-driven acceleration, heating-driven temperature drop.

| #     | Topic                                                                      | Description                                                                                                                                                                                                                      |
| ----- | -------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 11.1  | [[11.1-Ideal-Gas-Thermodynamics\|Ideal Gas Thermodynamics]]                | Equation of state, internal energy, enthalpy, specific heats, entropy, isentropic process                                                                                                                                        |
| 11.2  | [[11.2-Speed-of-Sound-Mach-Number\|Speed of Sound & Mach Number]]          | **Full step-by-step CV derivation** of $c = \sqrt{(\partial p/\partial \rho)_s}$, wave-frame transformation, isentropic justification, ideal gas $c = \sqrt{kRT}$, Mach regimes, disturbance propagation, Mach cone              |
| 11.3  | [[11.3-Categories-of-Compressible-Flow\|Categories of Compressible Flow]]  | Incompressible vs compressible criterion, subsonic/transonic/supersonic/hypersonic, stagnation conditions                                                                                                                        |
| 11.4  | [[11.4-Isentropic-Flow\|Isentropic Flow of an Ideal Gas]]                  | Isentropic relations $p/\rho^k$, $T/\rho^{k-1}$, critical conditions, effect of area change                                                                                                                                      |
| 11.5  | [[11.5-Isentropic-Flow-Through-Nozzles\|Isentropic Flow Through Nozzles]]  | Converging nozzles, converging-diverging (C-D) nozzles, choking, mass flow rate                                                                                                                                                  |
| 11.6  | [[11.6-Normal-Shocks\|Normal Shocks]]                                      | Governing equations (Rankine-Hugoniot), **full step-by-step derivations** of $p_2/p_1$, $T_2/T_1$, $& \text{Ma}_2$, Prandtl relation, property jumps, stagnation pressure loss, shock strength, moving shocks, numerical example |
| 11.6a | [[11.6a-Transonic-Flow-Condensation-Clouds\|Transonic Flow & Vapor Cones]] | Prandtl-Glauert singularity, local supersonic bubbles, condensation cloud physics, temperature drop → dew point, CFD visualization, misconceptions corrected                                                                     |
| 11.7  | [[11.7-Fanno-Rayleigh-Flow\|Duct Flow with Friction & Heat Transfer]]      | Fanno flow (constant area + friction), Rayleigh flow (constant area + heating), operational limits                                                                                                                               |

***

## Key Physical Intuitions

> ⚠️ **Compressible flow is full of counter-intuitive phenomena:**
> - **Friction can accelerate flow** (in subsonic, friction slows flow; in supersonic, friction accelerates it!)
> - **A converging duct can decelerate flow** (in supersonic flow, area decrease → velocity decrease)
> - **Heating can decrease temperature** (in supersonic Rayleigh flow)
> - **Abrupt discontinuities** (shock waves) can form across which pressure, density, and temperature jump almost instantly

***

## Central Equations Summary

| Concept | Equation | Eq. # |
|---------|----------|-------|
| Ideal gas law | $\rho = p / (RT)$ | (11.1) |
| Speed of sound | $c = \sqrt{kRT}$ | (11.26) |
| Mach number | $\text{Ma} = V / c$ | (11.27) |
| Isentropic $p$-$T$ | $p_2/p_1 = (T_2/T_1)^{k/(k-1)}$ | (11.34) |
| Isentropic $p$-$T$ (stagnation) | $p_0/p = (1 + \frac{k-1}{2}\text{Ma}^2)^{k/(k-1)}$ | (11.41) |
| Isentropic $\rho$-$T$ | $\rho_0/\rho = (1 + \frac{k-1}{2}\text{Ma}^2)^{1/(k-1)}$ | (11.42) |
| Isentropic $T$ (stagnation) | $T_0/T = 1 + \frac{k-1}{2}\text{Ma}^2$ | (11.40) |
| Critical area ratio | $A/A^* = \frac{1}{\text{Ma}}\bigl[\frac{2}{k+1}(1+\frac{k-1}{2}\text{Ma}^2)\bigr]^{(k+1)/[2(k-1)]}$ | (11.59) |
| Normal shock $p_2/p_1$ | $p_2/p_1 = 1 + \frac{2k}{k+1}(\text{Ma}_1^2 - 1)$ | (11.67) |
| Normal shock $\text{Ma}_2$ | $\text{Ma}_2^2 = \frac{(k-1)\text{Ma}_1^2 + 2}{2k\text{Ma}_1^2 - (k-1)}$ | (11.68) |
| Fanno flow | $\frac{4fL}{D} = \frac{1 - \text{Ma}^2}{k \text{Ma}^2} + \frac{k+1}{2k}\ln\bigl[\frac{(k+1)\text{Ma}^2}{2(1+\frac{k-1}{2}\text{Ma}^2)}\bigr]$ | (11.84) |
| Rayleigh flow | $T_0/T_0^* = \frac{2(k+1)\text{Ma}^2(1+\frac{k-1}{2}\text{Ma}^2)}{(1+k\text{Ma}^2)^2}$ | (11.98) |

> **Where to find values:** For common gases ($k$ = 1.4 for air), tabulated **isentropic flow tables**, **normal shock tables**, **Fanno flow tables**, and **Rayleigh flow tables** provide numerical values for the above dimensionless ratios.

---

## Relationship to Other Areas

- **Thermodynamics** — compressible flow is where fluid mechanics and thermodynamics meet; you need the energy equation and equation of state
- **Gas turbine & aeronautical engineering** — primary application domain
- **Open-channel flow** — mathematically analogous (Froude number ~ Mach number, hydraulic jump ~ shock wave)

> 📖 Full context → [[../../../Math/刷题仪表盘|Dashboard]]
