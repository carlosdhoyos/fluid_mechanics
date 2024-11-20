# Force Calculations on Flat and Curved Surfaces

In fluid mechanics, the force exerted by a fluid on a surface depends on the surface's orientation, shape, and pressure distribution. Here, we derive methods for calculating forces on flat surfaces (general orientation) and curved surfaces, with an emphasis on clarity and practical applications.

---

## 1. **Force on Flat Surfaces (General Orientation)**

A flat surface submerged in a fluid can be oriented at any angle $\theta$ with respect to the horizontal. The pressure distribution on the surface is governed by hydrostatic principles.

### a. Pressure Distribution

The pressure at any point on the surface is:

$$
p = p_0 + \rho g h,
$$

where $h$ is the vertical depth of the point below the fluid surface. For a plane inclined at an angle $\theta$, the depth $h$ is expressed as:

$$
h = z \sin \theta,
$$

where $z$ is the distance along the inclined surface. This relationship forms the basis for pressure integration over the surface.

### b. Resultant Force

The total force on the surface is obtained by integrating the pressure over the area:

$$
F = \int_A p \, dA.
$$

For a flat surface of area $A$, uniform density $\rho$, and a centroid at depth $\bar{h}$, the resultant force simplifies to:

$$
F = \rho g \bar{h} A,
$$

where:
- $\bar{h}$ is the vertical depth of the surface's centroid,
- $A$ is the total area of the surface.

### c. Line of Action

The line of action passes through the center of pressure. For an inclined surface, the center of pressure depth $h_{\text{cp}}$ is:

$$
h_{\text{cp}} = \bar{h} + \frac{I_G}{\bar{h} A},
$$

where $I_G$ is the second moment of area about the horizontal axis through the centroid.

### d. Practical Example

**Example 1: Flat Inclined Surface**  
Consider a flat plate of area $A = 4 \, \text{m}^2$, inclined at $\theta = 30^\circ$ to the horizontal, with centroid depth $\bar{h} = 2 \, \text{m}$.

**Resultant Force:**
$$
F = \rho g \bar{h} A = (1000)(9.81)(2)(4) = 78,480 \, \text{N}.
$$

**Horizontal and Vertical Components:**
$$
F_x = F \cos \theta = 78,480 \cos(30^\circ) = 67,973 \, \text{N},
$$

$$
F_y = F \sin \theta = 78,480 \sin(30^\circ) = 39,240 \, \text{N}.
$$

---

## 2. **Horizontal and Vertical Components**

For an inclined surface, the resultant force can be resolved into horizontal ($F_x$) and vertical ($F_y$) components.

### Horizontal Component:

The horizontal force corresponds to the force on the vertical projection:

$$
F_x = \rho g \bar{h}_x A_x,
$$

where $A_x$ is the vertical projection area, and $\bar{h}_x$ is the depth of its centroid.

### Vertical Component:

The vertical force arises from the weight of the fluid directly above the surface:

$$
F_y = \rho g \bar{h}_y A_y,
$$

where $A_y$ is the horizontal projection area, and $\bar{h}_y$ is the depth of its centroid.

---

## 3. **Force on Curved Surfaces**

For curved surfaces, the force calculation involves resolving the force into horizontal and vertical components.

### a. Horizontal Force

The horizontal component equals the force exerted on the vertical projection of the curved surface:

$$
F_x = \rho g \bar{h}_x A_{\text{proj, vertical}}.
$$

### b. Vertical Force

The vertical component equals the weight of the fluid above the surface:

$$
F_y = \rho g V_{\text{fluid}},
$$

where $V_{\text{fluid}}$ is the volume of fluid above the curved surface.

### c. Resultant Force and Direction

The magnitude of the resultant force is:

$$
F_R = \sqrt{F_x^2 + F_y^2},
$$

and its direction:

$$
\theta = \tan^{-1} \left( \frac{F_y}{F_x} \right).
$$

---

## 4. **Example: Curved Surface**

**Example 2: Hemispherical Dome**  
A hemispherical dome of radius $r = 2 \, \text{m}$ is submerged under a fluid.

- **Horizontal Force ($F_x$):**
  The vertical projection area is:
  $$
  A_{\text{proj}} = \pi r^2 = 12.57 \, \text{m}^2.
  $$
  Thus,
  $$
  F_x = \rho g \bar{h} A_{\text{proj}} = (1000)(9.81)(1)(12.57) = 123,290 \, \text{N}.
  $$

- **Vertical Force ($F_y$):**
  The fluid volume above the hemisphere is:
  $$
  V_{\text{fluid}} = \frac{2}{3} \pi r^3 = 16.76 \, \text{m}^3.
  $$
  Therefore,
  $$
  F_y = \rho g V_{\text{fluid}} = (1000)(9.81)(16.76) = 164,440 \, \text{N}.
  $$

---

## 5. **Dimensionless Parameters**

Dimensionless parameters, such as the Froude number or Reynolds number, are essential in real-world fluid mechanics applications, guiding interpretations of force impacts and flow regimes.

---

## 6. **Conclusion**

The methods outlined here are vital for designing safe and efficient fluid systems, including dams, submarine hulls, and fluid storage structures. Understanding the decomposition of forces into horizontal and vertical components simplifies analyses for both flat and curved surfaces.

### Key Takeaways:
- Flat surface force calculations rely on hydrostatic principles and centroid depths.
- Curved surface forces often require projections and volumetric considerations.
- Practical applications and diagrams enhance comprehension.

---

## Additional Exercises

1. Calculate the force on a rectangular plate $A = 3 \, \text{m}^2$, inclined at $45^\circ$, with $\bar{h} = 1.5 \, \text{m}$.
2. Determine the force components on a quarter-spherical dome with radius $r = 1.5 \, \text{m}$ submerged in water.

**Figures:**  
- Inclined flat surface showing pressure distribution and centroid.
- Hemispherical dome illustrating projection and fluid volume.

These examples highlight the applicability of hydrostatics to engineering problems.
