# Properties of Fluids

## What is Fluid Mechanics?

Fluid mechanics is the branch of physics that studies the behavior of fluids (liquids, gases, and plasmas) and the forces acting on them. The subject is divided into two major categories:

- **Fluid Statics**: The study of fluids at rest.
- **Fluid Dynamics**: The study of fluids in motion.

## Properties of Fluids

Understanding the physical properties of fluids is essential for analyzing fluid flow. The key properties include:

- **Density** ($\rho$): The mass per unit volume of a fluid.
- 
- 
- **Viscosity** ($\mu$): The fluid's resistance to deformation or flow.
  
  $$ \tau = \mu \frac{du}{dy} $$

- **Surface Tension** ($\sigma$): The cohesive force at the surface of a fluid.
  
  $$ F = \sigma L $$


## What is Density?

**Density** is a fundamental property of fluids that measures the amount of mass contained in a unit volume of a substance. It is a key parameter in fluid mechanics, as it influences various aspects of fluid behavior, including pressure, buoyancy, and flow dynamics. Density is denoted by the symbol $\rho$ and is mathematically expressed as:

$$
\rho = \frac{m}{V}
$$

Where:
- $\rho$ is the density (in units of $kg/m^3$ in SI),
- $m$ is the mass of the fluid (in kilograms, kg),
- $V$ is the volume of the fluid (in cubic meters, $m^3$).

### Importance of Density in Fluid Mechanics

Density plays a crucial role in several fluid mechanics applications:
- **Buoyancy**: Objects float or sink in a fluid depending on their density relative to the fluid. For instance, a boat floats because its average density is less than the density of water.
- **Pressure in a Fluid Column**: The pressure at a given depth in a fluid is directly proportional to its density (hydrostatic pressure equation: $P = \rho gh$, where $g$ is the acceleration due to gravity and $h$ is the depth).
- **Flow Behavior**: In compressible flows (e.g., gases), density changes significantly and must be accounted for. In incompressible flows (e.g., liquids), density is generally constant.

### Examples of Density

1. **Water**: The density of water at standard temperature and pressure (STP) is approximately $1000 \, kg/m^3$. This property is commonly used as a reference for other fluids.
2. **Air**: The density of air at sea level and room temperature is about $1.225 \, kg/m^3$. This value decreases with altitude.
3. **Mercury**: Mercury has a very high density of approximately $13,600 \, kg/m^3$, which is why it is commonly used in barometers to measure atmospheric pressure.

### Typical Densities of Fluids

The following table lists the typical densities of common fluids in both **SI units** and **British Gravitational (BG) units**.

| Fluid          | Density ($kg/m^3$) | Density ($lb/ft^3$) | Remarks               |
|----------------|-------------------:|--------------------:|-----------------------|
| Air (STP)      | 1.225              | 0.0765              | At sea level           |
| Water (STP)    | 1000               | 62.4                | Standard temperature   |
| Seawater       | 1025               | 64                  | Higher than fresh water due to salts |
| Mercury        | 13,600             | 847                 | Extremely dense liquid |
| Ethanol        | 789                | 49.3                | Common alcohol         |
| Glycerin       | 1260               | 78.6                | Viscous liquid         |
| Gasoline       | 680                | 42.5                | Common fuel            |

### Units of Density

- **SI Units**: In the International System of Units (SI), density is measured in **kilograms per cubic meter** ($kg/m^3$). This unit reflects the mass contained in one cubic meter of a substance.
  
- **BG Units**: In the British Gravitational (BG) system, density is measured in **pounds per cubic foot** ($lb/ft^3$), which represents the weight of the fluid per unit volume in cubic feet.

### Practical Example: Buoyancy

Consider an object submerged in water. If the object's density is less than that of water ($\rho_{\text{object}} < \rho_{\text{water}}$), it will float. For example, a wooden block with a density of $600 \, kg/m^3$ will float in water because its density is significantly lower than water's density of $1000 \, kg/m^3$.

On the other hand, if an object is denser than water (e.g., iron with $\rho \approx 7,870 \, kg/m^3$), it will sink because its density is much greater than the surrounding fluid.

### Conclusion

Density is a fundamental property in fluid mechanics that directly affects fluid behavior under various conditions. From determining whether objects float or sink to influencing pressure in fluid columns, understanding and calculating density is essential for solving fluid mechanics problems.


```{note}

# Slugs vs. Pounds in the British Gravitational (BG) System

In the **British Gravitational (BG) system**, there are two common ways to express mass-related quantities in fluid mechanics: **slugs** and **pounds**. These units represent different concepts and are often used in different contexts within fluid mechanics.

### 1. Mass Density vs. Weight Density

1. **Slugs per cubic foot ($\text{slug/ft}^3$)**:
   - This is a measure of **mass density** in the BG system. It corresponds to the **mass per unit volume** of a fluid, similar to how **kg/m³** is used in the SI system.
   
2. **Pounds per cubic foot ($\text{lb/ft}^3$)**:
   - This is a measure of **weight density** (also called specific weight), which represents the **weight of the fluid per unit volume**. This unit incorporates the force of gravity because it measures the fluid's weight in pounds.

### 2. Key Difference Between Slug and Pound Units

- **Slug ($\text{slug}$)**: 
   - A **slug** is a unit of **mass** in the BG system.
   - The relationship between mass and weight in the BG system is defined by:
     
     $$
     W = mg
     $$
     
     Where:
     - $W$ is the weight (in pounds, $\text{lb}$),
     - $m$ is the mass (in slugs, $\text{slug}$),
     - $g$ is the acceleration due to gravity (typically $32.174 \, \text{ft/s}^2$).

   - One **slug** is the amount of mass that, under standard Earth gravity, weighs **1 pound-force per unit of acceleration**.

- **Pound ($\text{lb}$)**:
   - A **pound** is a unit of **force (weight)** in the BG system.
   - When we use **$\text{lb/ft}^3$**, we are expressing **weight density** (the weight per unit volume). This value includes the force due to gravity.

### 3. Conversion Between Slug and Pound

To convert between **weight density** ($\text{lb/ft}^3$) and **mass density** ($\text{slug/ft}^3$), you need to account for the acceleration due to gravity ($g$):

$$
\rho_{\text{mass}} (\text{slug/ft}^3) = \frac{\rho_{\text{weight}} (\text{lb/ft}^3)}{g}
$$

For example, the weight density of water is approximately $62.4 \, \text{lb/ft}^3$. To convert this to mass density in slugs per cubic foot:

$$
\rho = \frac{62.4 \, \text{lb/ft}^3}{32.174 \, \text{ft/s}^2} \approx 1.94 \, \text{slug/ft}^3
$$

### 4. When Slugs are Used

In fluid mechanics, **slugs/ft³** is often used when dealing with **mass density** because it simplifies calculations involving dynamics. By using slugs, you can apply Newton’s second law ($F = ma$) directly without introducing a conversion factor for gravity, as slugs are already based on the relationship between mass and weight under standard gravity.

### 5. Common Mistake: Mixing Slugs and Pounds

It's easy to confuse **mass density** and **weight density** in the BG system because both use units related to mass and force. Keep in mind:
- **$\text{lb/ft}^3$** refers to **weight density**, which measures the weight of the fluid in pounds per cubic foot. 
- **$\text{slug/ft}^3$** is the correct unit for **mass density** in the BG system. 

Always convert between the two by dividing or multiplying by the acceleration due to gravity ($g = 32.174 \, \text{ft/s}^2$).

### 6. Summary of Differences

| Quantity        | Symbol           | Definition                         | Units in BG System       | Units in SI System        |
|-----------------|------------------|------------------------------------|--------------------------|---------------------------|
| **Mass Density**| $\rho_{\text{mass}}$ | Mass per unit volume               | $\text{slug/ft}^3$        | $\text{kg/m}^3$           |
| **Weight Density**| $\rho_{\text{weight}}$| Weight per unit volume (includes gravity) | $\text{lb/ft}^3$ | $\text{N/m}^3$            |

- **Mass Density**: Refers to the mass contained in a given volume, and in the BG system, it is measured in **slugs/ft³**.
- **Weight Density**: Refers to the weight of the fluid per unit volume, typically measured in **lb/ft³**, and incorporates the effect of gravity.

### Practical Example: Calculating Density

Let’s calculate the mass density of air using its typical weight density at sea level ($\approx 0.0765 \, \text{lb/ft}^3$):

$$
\rho_{\text{mass}} = \frac{0.0765 \, \text{lb/ft}^3}{32.174 \, \text{ft/s}^2} \approx 0.00238 \, \text{slug/ft}^3
$$

In this case, the mass density of air is about $0.00238 \, \text{slug/ft}^3$, while its weight density remains $0.0765 \, \text{lb/ft}^3$.

```





## Types of Fluid Flow

Fluids exhibit different types of flow depending on various factors like velocity, pressure, and external forces. The major types of fluid flow are:

1. **Laminar Flow**: Flow where fluid moves in smooth paths or layers.
2. **Turbulent Flow**: Flow where the fluid undergoes irregular fluctuations and mixing.
3. **Steady Flow**: The fluid properties at any point remain constant over time.
4. **Unsteady Flow**: The fluid properties change over time.