# Hydrostatic Balance

The Navier-Stokes equations in three-dimensional Cartesian coordinates for a Newtonian fluid are expressed as follows:

## General Form (Momentum Equation)

$$
\rho \left( \frac{\partial \mathbf{V}}{\partial t} + \mathbf{V} \cdot \nabla \mathbf{V} \right) = -\nabla p + \mu \nabla^2 \mathbf{V} + \mathbf{f}
$$

where:
- $\mathbf{V} = (u, v, w)$ is the velocity vector,
- $\rho$ is the fluid density,
- $p$ is the pressure,
- $\mu$ is the dynamic viscosity,
- $\mathbf{f}$ is the body force per unit volume, such as gravity.

### Assumptions for Hydrostatic Balance

To derive hydrostatic balance:
1. **Steady-state condition:** $\frac{\partial \mathbf{V}}{\partial t} = 0$ (no time-dependent changes).
2. **No motion:** $\mathbf{V} = 0$ (fluid is at rest, so no convective acceleration).
3. **Negligible viscous forces:** $\mu \nabla^2 \mathbf{V} = 0$ (dominance of pressure and body forces over viscous effects).

With these assumptions, the Navier-Stokes equations simplify to:

$$
-\nabla p + \mathbf{f} = 0
$$

### Incorporating Gravitational Force

The dominant body force in many scenarios is gravity, $\mathbf{f} = -\rho g \mathbf{j}$, where $\mathbf{j}$ is the unit vector in the vertical direction ($z$). Substituting:

$$
-\nabla p - \rho g \mathbf{j} = 0
$$

In component form, this becomes:

$$
\frac{\partial p}{\partial x} = 0, \quad \frac{\partial p}{\partial y} = 0, \quad \frac{\partial p}{\partial z} = -\rho g
$$

The pressure only varies in the $z$ direction, leading to:

$$
\frac{\partial p}{\partial z} = -\rho g
$$

This is the equation of hydrostatic balance.

---

## Integration of Hydrostatic Balance

### 1. **Incompressible Fluid (Liquids)**

For an incompressible fluid, $\rho$ is constant. Integrating $\frac{\partial p}{\partial z} = -\rho g$:

$$
p(z) = p_0 - \rho g z
$$

where:
- $p_0$ is the pressure at a reference height $z = 0$.

This is the well-known hydrostatic pressure formula for liquids.

---

### 2. **Compressible Fluid (Atmosphere)**

For a compressible fluid, $\rho$ varies with pressure and temperature. Using the ideal gas law:

$$
\rho = \frac{p}{R T}
$$

where:
- $R$ is the specific gas constant,
- $T$ is the temperature.

Substitute $\rho$ into $\frac{\partial p}{\partial z} = -\rho g$:

$$
\frac{\partial p}{\partial z} = -\frac{p g}{R T}
$$

Assuming isothermal conditions ($T$ is constant), we can integrate:

$$
\frac{1}{p} \frac{\partial p}{\partial z} = -\frac{g}{R T}
$$

Integrating:

$$
\ln p = -\frac{g z}{R T} + \ln p_0
$$

Exponentiate to solve for $p(z)$:

$$
p(z) = p_0 e^{-\frac{g z}{R T}}
$$

where $p_0$ is the pressure at $z = 0$. This is the barometric pressure formula for the atmosphere.

---

## Summary

- For **incompressible fluids**, hydrostatic pressure increases linearly with depth.
- For **compressible fluids**, pressure decreases exponentially with height under isothermal conditions.
These simplifications and integrations illustrate the core principles of hydrostatic balance for different fluid states.
