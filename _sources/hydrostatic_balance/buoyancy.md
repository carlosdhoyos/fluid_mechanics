# Buoyancy Force on a Submerged Object

The buoyancy force arises from variations in hydrostatic pressure acting on the surfaces of a submerged object. This section derives **Archimedes' Principle** from the fundamental hydrostatic equation and explains its implications.

---

## 1. **Relating Buoyancy to the Hydrostatic Equation**

The pressure in a static fluid varies with depth according to the **hydrostatic equation**:

$$
\frac{dp}{dz} = -\rho_f g,
$$

where:
- $p$ is the pressure,
- $z$ is the vertical coordinate (positive upward),
- $\rho_f$ is the fluid density,
- $g$ is the gravitational acceleration.

Integrating this equation from the surface of the fluid ($z = 0$) to a depth $z$, with surface pressure $p_0$:

$$
p = p_0 + \rho_f g z.
$$

This pressure variation generates a net upward force on submerged objects, leading to the buoyancy force.

---

## 2. **Derivation of Archimedes' Principle**

Consider a submerged object of arbitrary shape fully surrounded by a fluid. The object experiences pressure forces acting on its surface.

### a. Net Vertical Force

The pressure on the bottom surface is greater than on the top surface due to the increase in pressure with depth. Let the object displace a volume of fluid $V_d$.

- **Force on the top surface:**  
  At depth $z_{\text{top}}$, pressure is:

  $$
  p_{\text{top}} = p_0 + \rho_f g z_{\text{top}}.
  $$

  The force on the top surface (area $A_{\text{top}}$):
  
  $$
  F_{\text{top}} = p_{\text{top}} A_{\text{top}}.
  $$

- **Force on the bottom surface:**  
  At depth $z_{\text{bottom}}$, pressure is:

  $$
  p_{\text{bottom}} = p_0 + \rho_f g z_{\text{bottom}}.
  $$
  
  The force on the bottom surface (area $A_{\text{bottom}}$):
  
  $$
  F_{\text{bottom}} = p_{\text{bottom}} A_{\text{bottom}}.
  $$

- **Net upward force:**  
  Subtracting the forces:
  
  $$
  F_B = F_{\text{bottom}} - F_{\text{top}} = \rho_f g (z_{\text{bottom}} - z_{\text{top}}) A_{\text{projected}},
  $$
  
  where $A_{\text{projected}}$ is the projected cross-sectional area.

### b. Displaced Fluid Volume

The product $(z_{\text{bottom}} - z_{\text{top}}) A_{\text{projected}}$ equals the volume of displaced fluid, $V_d$. Thus, the buoyant force becomes:

$$
F_B = \rho_f g V_d.
$$

### c. Archimedes' Principle

This result states that the **buoyant force equals the weight of the displaced fluid**:

$$
F_B = \text{Weight of Displaced Fluid}.
$$

---

## 3. **Physical Interpretation of Buoyancy**

The buoyancy force acts upward because the fluid pressure increases with depth, creating a net upward pressure difference on the object. The magnitude of this force depends only on the volume of displaced fluid and the fluid's density, not the properties of the object.

---

## 4. **Conditions for Buoyancy**

### a. Floating Objects

If the object's weight, $W$, is less than the buoyant force, it floats. The equilibrium condition is:

$$
F_B = W \quad \text{or} \quad \rho_f g V_d = m_o g,
$$

where $m_o$ is the object's mass.

### b. Submerged Objects

For fully submerged objects, the displaced fluid volume equals the object's volume, $V_o$. The net force determines whether the object sinks or remains neutrally buoyant:

$$
F_{\text{net}} = F_B - W.
$$

---

## 5. **Example Derivation**

**Example: Submerged Cube**  
A cube with side length $L = 0.5 \, \text{m}$ is submerged in water ($\rho_f = 1000 \, \text{kg/m}^3$). Find the buoyant force.

### Solution:

1. **Volume of Displaced Fluid:**

   $$
   V_d = L^3 = (0.5)^3 = 0.125 \, \text{m}^3.
   $$

2. **Buoyant Force:**

   $$
   F_B = \rho_f g V_d = (1000)(9.81)(0.125) = 1226.25 \, \text{N}.
   $$

---

## 6. **Applications of Buoyancy**

### a. Ship Design
Ships float because their hulls displace enough water to create a buoyant force equal to their weight.

### b. Submarines
Submarines adjust their buoyancy by altering ballast water, controlling their submerged depth.

### c. Hot Air Balloons
In gases, the buoyant force depends on the displaced air's weight, enabling lift.

---

## 7. **Key Takeaways**

- The buoyant force arises due to hydrostatic pressure variations in a fluid.
- Archimedes' Principle states that the buoyant force equals the weight of the displaced fluid.
- Understanding buoyancy is critical in engineering applications like shipbuilding, underwater exploration, and aeronautics.
