---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Solids vs. Fluids

Solids and fluids (liquids and gases) exhibit distinct mechanical behaviors due to differences in their molecular interactions and responses to forces.

## Molecular Structure and Behavior

- **Solids**: Molecules are closely packed in a regular arrangement with strong intermolecular forces. This gives solids a definite shape and volume.  
  - **Elasticity**: Solids resist deformation and tend to return to their original form when forces are removed (Hooke’s Law).  
  - **Shear Stress**: Solids can sustain shear stress without flowing, as intermolecular forces provide resistance.

- **Fluids**: Molecules are loosely arranged and move freely past each other, with weaker intermolecular forces. Fluids take the shape of their container and are classified as:  
  - **Liquids**: Definite volume but no fixed shape. They flow under gravity or other forces and are nearly incompressible.  
  - **Gases**: No definite volume or shape. They expand to fill their container and are highly compressible.  
  - **Shear Stress**: Fluids cannot resist shear stress. Even a small shear force leads to continuous deformation (flow).  

  - **Viscosity**: Fluids resist shear through viscosity, which measures the internal friction between fluid layers.  
  - **Newtonian vs. Non-Newtonian**: Newtonian fluids (e.g., water, air) have constant viscosity, while non-Newtonian fluids (e.g., ketchup, blood) change viscosity depending on the applied stress.

## Response to Forces

- **Solids**: Stress–strain relationships describe how solids deform. Deformation can be elastic (reversible) or plastic (permanent). Solids resist both normal forces (tensile/compressive) and shear forces.  

- **Fluids**: Fluids resist normal forces by changing pressure or volume, but under shear forces they continuously deform. Unlike solids, fluids cannot reach equilibrium under shear; they always flow.

## Flow and Motion

- **Solids**: Deform under force but do not flow. Once forces are removed, they return to their shape (elastic) or remain deformed (plastic).  
- **Fluids**: Flow whenever subjected to shear forces.  
  - **Laminar flow**: Smooth, orderly motion.  
  - **Turbulent flow**: Chaotic, irregular motion.  
  - **Examples**: Water in a pipe (laminar vs. turbulent), glacier ice (slow fluid-like flow despite being solid).

## Continuum Hypothesis

The **continuum hypothesis** assumes fluids can be treated as continuous matter, despite being made of discrete molecules. This allows fluid properties like velocity, pressure, and density to be described as smooth functions of space and time.

### Key Concepts

- **Molecular vs. Macroscopic Scales**  
  At the molecular level, fluids consist of randomly moving particles. At the macroscopic level (scales much larger than molecular dimensions), fluid properties are averaged and treated as continuous.

- **Control Volume**  
  A region of space (fixed or moving) where fluid properties are averaged. Sufficient molecules exist in the volume to define density, velocity, and pressure.  

- **Fluid Element**  
  A differential volume treated as a “point” where fluid properties are defined continuously.

### Validity of the Hypothesis

The hypothesis holds when the **mean free path** $\lambda$ is much smaller than the characteristic system length $L$. This is quantified by the **Knudsen number** ($\text{Kn}$):

$$
\text{Kn} = \frac{\lambda}{L}
$$

- $\text{Kn} < 0.01$: Continuum assumption valid.  
- $0.01 < \text{Kn} < 0.1$: Slip-flow regime (e.g., microfluidics).  
- $0.1 < \text{Kn} < 10$: Transition regime; kinetic theory needed.  
- $\text{Kn} > 10$: Free molecular flow (e.g., rarefied gases in space).  

```{note}
The continuum hypothesis is the cornerstone of fluid mechanics. It enables the use of the Navier–Stokes and continuity equations, simplifying fluid flow analysis for most engineering and natural systems.


## What is Fluid Mechanics?

Fluid mechanics is the branch of physics that studies the behavior of fluids and the forces acting on them.

- **Fluid Statics**: The study of fluids at rest.
- **Fluid Dynamics**: The study of fluids in motion.

Applications span engineering (aerospace, civil, mechanical), environmental sciences (atmosphere, oceans, rivers), and biological systems (blood flow, respiratory dynamics). Plasmas, often treated as fluids with electromagnetic effects, are also part of advanced fluid mechanics.