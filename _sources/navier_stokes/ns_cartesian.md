# Navier-Stokes Equations in Cartesian Coordinates

In three-dimensional Cartesian coordinates ($x$, $y$, and $z$), the Navier-Stokes equations can be expressed separately for each direction. For a Newtonian, incompressible fluid, the conservation of momentum in each direction includes contributions from pressure, viscous, and external forces.

Let’s assume:
- $ \mathbf{V} = (u, v, w) $, where $ u $, $ v $, and $ w $ are the velocity components in the $ x $, $ y $, and $ z $ directions, respectively.
- $ \rho $ is the fluid density, and $ \mu $ is the dynamic viscosity.

The Navier-Stokes equations in each direction are as follows:

## 1. $ x $-Direction

The Navier-Stokes equation in the $ x $ direction is:

$$
\rho \left( \frac{\partial u}{\partial t} + u \frac{\partial u}{\partial x} + v \frac{\partial u}{\partial y} + w \frac{\partial u}{\partial z} \right) = -\frac{\partial p}{\partial x} + \mu \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2} \right) + f_x
$$

where:
- $ \frac{\partial u}{\partial t} $ is the local acceleration in the $ x $ direction,
- $ u \frac{\partial u}{\partial x} + v \frac{\partial u}{\partial y} + w \frac{\partial u}{\partial z} $ represents convective acceleration,
- $ -\frac{\partial p}{\partial x} $ is the pressure gradient in the $ x $ direction,
- $ \mu \left( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2} \right) $ is the viscous term (Laplacian of $ u $),
- $ f_x $ is any external body force in the $ x $ direction.

## 2. $ y $-Direction

The Navier-Stokes equation in the $ y $ direction is:

$$
\rho \left( \frac{\partial v}{\partial t} + u \frac{\partial v}{\partial x} + v \frac{\partial v}{\partial y} + w \frac{\partial v}{\partial z} \right) = -\frac{\partial p}{\partial y} + \mu \left( \frac{\partial^2 v}{\partial x^2} + \frac{\partial^2 v}{\partial y^2} + \frac{\partial^2 v}{\partial z^2} \right) + f_y
$$

where:
- $ \frac{\partial v}{\partial t} $ is the local acceleration in the $ y $ direction,
- $ u \frac{\partial v}{\partial x} + v \frac{\partial v}{\partial y} + w \frac{\partial v}{\partial z} $ represents convective acceleration,
- $ -\frac{\partial p}{\partial y} $ is the pressure gradient in the $ y $ direction,
- $ \mu \left( \frac{\partial^2 v}{\partial x^2} + \frac{\partial^2 v}{\partial y^2} + \frac{\partial^2 v}{\partial z^2} \right) $ is the viscous term (Laplacian of $ v $),
- $ f_y $ is any external body force in the $ y $ direction.

## 3. $ z $-Direction

The Navier-Stokes equation in the $ z $ direction is:

$$
\rho \left( \frac{\partial w}{\partial t} + u \frac{\partial w}{\partial x} + v \frac{\partial w}{\partial y} + w \frac{\partial w}{\partial z} \right) = -\frac{\partial p}{\partial z} + \mu \left( \frac{\partial^2 w}{\partial x^2} + \frac{\partial^2 w}{\partial y^2} + \frac{\partial^2 w}{\partial z^2} \right) + f_z
$$

where:
- $ \frac{\partial w}{\partial t} $ is the local acceleration in the $ z $ direction,
- $ u \frac{\partial w}{\partial x} + v \frac{\partial w}{\partial y} + w \frac{\partial w}{\partial z} $ represents convective acceleration,
- $ -\frac{\partial p}{\partial z} $ is the pressure gradient in the $ z $ direction,
- $ \mu \left( \frac{\partial^2 w}{\partial x^2} + \frac{\partial^2 w}{\partial y^2} + \frac{\partial^2 w}{\partial z^2} \right) $ is the viscous term (Laplacian of $ w $),
- $ f_z $ is any external body force in the $ z $ direction.

---

## Summary

The Navier-Stokes equations in Cartesian coordinates provide a breakdown of the momentum equations in each spatial direction, highlighting how forces (pressure, viscous, and external) contribute to acceleration in the $ x $, $ y $, and $ z $ directions. These component forms are particularly useful for solving problems in specific geometries, where each direction can be analyzed separately.
