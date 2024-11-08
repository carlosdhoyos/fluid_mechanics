# Derivation of the Pressure Gradient Force

To understand the **pressure gradient force** acting on a small fluid element, let's start by examining the forces exerted by pressure differences across this element.

## Step 1: Consider a Small Fluid Parcel

1. Let’s take a **small rectangular parcel** of fluid with dimensions $dx$, $dy$, and $dz$ in the $x$, $y$, and $z$ directions, respectively.
2. Assume the fluid has a pressure field $p$ that varies in space, meaning $p = p(x, y, z)$.
3. The parcel will experience different pressures on opposite faces due to spatial changes in pressure (pressure gradient).

## Step 2: Calculate Pressure Forces on Opposite Faces

To derive the pressure force, we consider the pressure acting on opposite faces in the $x$ direction.

- **Pressure on the left face (at $x$)**: The pressure on the left face is $p(x, y, z)$, acting over an area $dy \cdot dz$.
    - The force due to pressure on the left face is therefore:
    
      $$
      F_{\text{left}} = p(x, y, z) \cdot dy \cdot dz
      $$
  
- **Pressure on the right face (at $x + dx$)**: The pressure on the right face is slightly different due to the pressure gradient in the $x$ direction. Using a Taylor series expansion:

    $$
    p(x + dx, y, z) \approx p(x, y, z) + \frac{\partial p}{\partial x} \cdot dx
    $$

    - The force on the right face is:
    
      $$
      F_{\text{right}} = \left( p(x, y, z) + \frac{\partial p}{\partial x} \cdot dx \right) \cdot dy \cdot dz
      $$

## Step 3: Calculate Net Pressure Force in the $x$ Direction

The net pressure force in the $x$ direction, $F_x$, is the difference between the force on the right face and the force on the left face:

$$
F_x = F_{\text{right}} - F_{\text{left}}
$$

Substituting the expressions from above:

$$
F_x = \left( p(x, y, z) + \frac{\partial p}{\partial x} \cdot dx \right) \cdot dy \cdot dz - p(x, y, z) \cdot dy \cdot dz
$$

Simplifying by canceling terms:

$$
F_x = \frac{\partial p}{\partial x} \cdot dx \cdot dy \cdot dz
$$

Similarly, we can calculate the net pressure forces in the $y$ and $z$ directions:

$$
F_y = \frac{\partial p}{\partial y} \cdot dx \cdot dy \cdot dz
$$

$$
F_z = \frac{\partial p}{\partial z} \cdot dx \cdot dy \cdot dz
$$

## Step 4: Write the Total Pressure Gradient Force

The total pressure force acting on the fluid parcel in all three directions can now be written as a vector:

$$
\mathbf{F}_{\text{pressure}} = - \left( \frac{\partial p}{\partial x} \hat{i} + \frac{\partial p}{\partial y} \hat{j} + \frac{\partial p}{\partial z} \hat{k} \right) \cdot dx \, dy \, dz
$$

Or, using the **gradient operator** $ \nabla $:

$$
\mathbf{F}_{\text{pressure}} = - (\nabla p) \, dx \, dy \, dz
$$

## Step 5: Express the Pressure Gradient Force per Unit Volume

For a small fluid parcel, the **volume** $V$ is $dx \cdot dy \cdot dz$. The **pressure gradient force per unit volume** (which we use in the Navier-Stokes equations) is therefore:

$$
\mathbf{f}_{\text{pressure}} = -\nabla p
$$

## Summary

The pressure gradient force per unit volume is $ -\nabla p $. This force results from spatial changes in pressure within the fluid and acts from regions of higher pressure to regions of lower pressure. It is a key component in the Navier-Stokes equations, influencing the motion of fluid by accelerating it in the direction of lower pressure.
