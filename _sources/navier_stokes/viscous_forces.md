# Derivation of Friction (Viscous) Forces in Fluid Mechanics

In fluid mechanics, **viscous forces** (or frictional forces) arise from the internal friction within a fluid as layers of fluid move relative to one another. These forces depend on the **viscosity** of the fluid and the velocity gradient between fluid layers. Let’s derive the expression for the viscous forces acting on a small fluid element.

## Step 1: Consider a Small Fluid Parcel

1. We start by examining a small rectangular fluid element (parcel) with dimensions $dx$, $dy$, and $dz$.
2. Assume the fluid has a viscosity $\mu$, which is a measure of the fluid’s resistance to deformation (its "stickiness").

## Step 2: Define Shear Stress Due to Viscosity

In a viscous fluid, as one layer of fluid moves past another, a **shear stress** is exerted due to the viscosity of the fluid. For a fluid moving in the $x$ direction with velocity $u$, this shear stress $\tau_{xy}$ is proportional to the rate of change of velocity in the $y$ direction, which we can express as a partial derivative:

$$
\tau_{xy} = \mu \frac{\partial u}{\partial y}
$$

where:
- $\tau_{xy}$ is the shear stress acting on the $x$ face in the $y$ direction,
- $\mu$ is the dynamic viscosity of the fluid,
- $\frac{\partial u}{\partial y}$ represents the velocity gradient in the $y$ direction.

This relationship, called **Newton's Law of Viscosity**, assumes a **Newtonian fluid** where the shear stress is linearly proportional to the velocity gradient.

### Shear Stresses in Other Directions

Similarly, we can define shear stresses for velocity changes in other directions:
- $\tau_{yx} = \mu \frac{\partial v}{\partial x}$, where $v$ is the velocity in the $y$ direction.
- $\tau_{zx} = \mu \frac{\partial w}{\partial x}$, where $w$ is the velocity in the $z$ direction.

In general, we define the **shear stress tensor** for a fluid as:
$$
\tau_{ij} = \mu \frac{\partial u_i}{\partial x_j}
$$

where $u_i$ is the velocity in the $i$ direction and $x_j$ is the spatial coordinate in the $j$ direction.

## Step 3: Calculate the Net Viscous Force on the Fluid Parcel

Let’s calculate the viscous forces acting on the fluid parcel in the $x$ direction. For simplicity, we’ll start with shear stresses acting on the faces perpendicular to the $x$ axis.

### Viscous Force in the $x$ Direction

1. **Shear Stress on the Left Face ($x$)**:
   - The shear stress on the left face (at position $x$) in the $x$ direction is $\tau_{xx} = \mu \frac{\partial u}{\partial x}$.
   - The force due to shear stress on this face, acting over an area $dy \cdot dz$, is:
     $$
     F_{\text{left}} = \tau_{xx} \cdot dy \cdot dz = \mu \frac{\partial u}{\partial x} \cdot dy \cdot dz
     $$

2. **Shear Stress on the Right Face ($x + dx$)**:
   - The shear stress on the right face (at $x + dx$) is:
     $$
     \tau_{xx}(x + dx) = \tau_{xx} + \frac{\partial \tau_{xx}}{\partial x} \cdot dx
     $$
   - The force on the right face is then:
     $$
     F_{\text{right}} = \left( \tau_{xx} + \frac{\partial \tau_{xx}}{\partial x} \cdot dx \right) \cdot dy \cdot dz
     $$

3. **Net Viscous Force in the $x$ Direction**:
   - The net viscous force in the $x$ direction is:
     $$
     F_x = F_{\text{right}} - F_{\text{left}} = \frac{\partial \tau_{xx}}{\partial x} \cdot dx \cdot dy \cdot dz
     $$
   - Substituting $\tau_{xx} = \mu \frac{\partial u}{\partial x}$, we get:
     $$
     F_x = \frac{\partial}{\partial x} \left( \mu \frac{\partial u}{\partial x} \right) \cdot dx \cdot dy \cdot dz
     $$

### Viscous Forces in the $y$ and $z$ Directions

Similarly, we can derive the viscous forces in the $y$ and $z$ directions:

$$
F_y = \frac{\partial}{\partial y} \left( \mu \frac{\partial v}{\partial y} \right) \cdot dx \cdot dy \cdot dz
$$

$$
F_z = \frac{\partial}{\partial z} \left( \mu \frac{\partial w}{\partial z} \right) \cdot dx \cdot dy \cdot dz
$$

## Step 4: Write the Total Viscous Force per Unit Volume

The total viscous force per unit volume, $\mathbf{f}_{\text{viscous}}$, can be expressed by combining these components:

$$
\mathbf{f}_{\text{viscous}} = \nabla \cdot \left( \mu \nabla \mathbf{u} \right)
$$

where $\nabla \mathbf{u}$ is the velocity gradient tensor. This term appears in the Navier-Stokes equation as the **viscous force per unit volume** and describes the internal frictional forces in a fluid due to viscosity.


## Summary

The viscous force per unit volume, $\mathbf{f}_{\text{viscous}} = \nabla \cdot \left( \mu \nabla \mathbf{u} \right)$, represents the frictional resistance within the fluid. This force is crucial in fluid mechanics because it captures how fluids resist deformation due to internal friction, affecting the velocity field and energy dissipation within the fluid.


---

## Table of Stresses in Fluid Mechanics

In fluid mechanics, stresses within a fluid are categorized as either **normal stresses** or **shear stresses**. Normal stresses act perpendicular to a surface and include both compressive and tensile stresses, while shear stresses act tangentially to a surface and arise from viscosity as layers of fluid slide past one another.

The notation for stresses uses two subscripts:
- The first subscript indicates the **direction normal to the surface** on which the stress acts.
- The second subscript indicates the **direction in which the stress acts**.

Below is a table summarizing the notation for all normal and shear stresses in a fluid, with the direction each stress acts on and the associated expression.

| Type of Stress | Notation | Acts on Surface Normal to | Acts in Direction | Expression                       |
|----------------|----------|---------------------------|-------------------|----------------------------------|
| **Normal Stresses**       |          |                           |                   |                                  |
| Compressive or tensile in $x$ | $\tau_{xx}$ | $x$                       | $x$               | $-\frac{\partial p}{\partial x} + \mu \frac{\partial u}{\partial x}$ |
| Compressive or tensile in $y$ | $\tau_{yy}$ | $y$                       | $y$               | $-\frac{\partial p}{\partial y} + \mu \frac{\partial v}{\partial y}$ |
| Compressive or tensile in $z$ | $\tau_{zz}$ | $z$                       | $z$               | $-\frac{\partial p}{\partial z} + \mu \frac{\partial w}{\partial z}$ |
| **Shear Stresses**       |          |                           |                   |                                  |
| Shear in $y$ direction on $x$ face | $\tau_{xy}$ | $x$                       | $y$               | $\mu \frac{\partial u}{\partial y}$ |
| Shear in $z$ direction on $x$ face | $\tau_{xz}$ | $x$                       | $z$               | $\mu \frac{\partial u}{\partial z}$ |
| Shear in $x$ direction on $y$ face | $\tau_{yx}$ | $y$                       | $x$               | $\mu \frac{\partial v}{\partial x}$ |
| Shear in $z$ direction on $y$ face | $\tau_{yz}$ | $y$                       | $z$               | $\mu \frac{\partial v}{\partial z}$ |
| Shear in $x$ direction on $z$ face | $\tau_{zx}$ | $z$                       | $x$               | $\mu \frac{\partial w}{\partial x}$ |
| Shear in $y$ direction on $z$ face | $\tau_{zy}$ | $z$                       | $y$               | $\mu \frac{\partial w}{\partial y}$ |

### Notes:
- **Normal stresses** include contributions from both **pressure** (compressive forces) and **viscous effects**.
- **Shear stresses** are purely viscous in nature and arise from the relative motion (velocity gradient) between layers of fluid.
- In cases where the fluid is **Newtonian** (i.e., stress is proportional to the rate of strain), the dynamic viscosity $ \mu $ is a constant.
- The **stress tensor** is symmetric, so $ \tau_{xy} = \tau_{yx} $, $ \tau_{xz} = \tau_{zx} $, and $ \tau_{yz} = \tau_{zy} $.

This table provides a concise reference for understanding how each stress acts within a fluid element, assisting in the formulation and analysis of the Navier-Stokes equations.

