# Syllabus
**Course Duration**: 16 Weeks

## Course Description
This course introduces the fundamental principles of fluid mechanics, focusing on the behavior of incompressible fluids. Topics include fluid statics, kinematics, and dynamics, with an emphasis on differential analysis, including the Navier-Stokes equations and Bernoulli's equation. Students will apply these principles to solve practical engineering problems.

## Week-by-Week Outline
### **Weeks 1-2: Introduction to Fluid Mechanics and Properties**
- <span style="color: black;">Prerequisites: Math and physics</span>
- <span style="color: black;">Definition of fluids and distinction between solids and fluids.</span>
- <span style="color: black;">Continuum hypothesis: fluid as a continuum.</span>
- <span style="color: black;">Common physical quantities and units.</span>
- <span style="color: black;">Fluid properties: density, viscosity, surface tension.</span>
- <span style="color: black;">Ideal gas law</span>
- <span style="color: black;">No-slip condition</span>
- <span style="color: black;">Types of flows: laminar and turbulent</span>
- Flow classification: laminar vs. turbulent, steady vs. unsteady, uniform vs. non-uniform

**Lab**: Measurement of basic fluid properties (density, viscosity, surface tension).

---

### **Week 3: Fluid Kinematics**
- <span style="color: black;">Lagrangian vs. Eulerian descriptions of fluid motion.</span>
- <span style="color: black;">Velocity and acceleration fields.</span>
- <span style="color: black;">Concept of vorticity and circulation.</span>
- <span style="color: black;">Streamlines, streaklines, and pathlines.</span>
- <span style="color: black;">Velocity potential and stream function.</span>
- <span style="color: black;">Flow classification: rotational vs. irrotational, incompressible vs. compressible.</span>

---

### **Week 4: Fluid Statics**
- <span style="color: black;">Hydrostatic equation: $\frac{dp}{dz} = -\rho g$.</span>  
- <span style="color: black;">Gauge vs. absolute pressure, vacuum pressure, and pressure head.</span>  
- <span style="color: black;">Pressure variation in incompressible and compressible static fluids.</span>  
- <span style="color: black;">Barometers, piezometers, and manometers.</span>  
- <span style="color: black;">Hydrostatic pressure forces on plane surfaces: resultant force and center of pressure.</span>  
- <span style="color: black;">Hydrostatic pressure on curved surfaces: decomposition into horizontal and vertical components.</span>  
- <span style="color: black;">Applications: pressure forces on submerged surfaces, dams, and gates.</span>  
- <span style="color: black;">Buoyancy force and Archimedes’ principle.</span>  
- <span style="color: black;">Stability of floating and submerged bodies: metacentric height and applications (ships, submarines).</span>  
- <span style="color: black;">Manometry errors: capillary effects and density variation.</span>  

**Optional Enrichment:**  
- Hydrostatics in rotating fluids (free surface of a rotating liquid, paraboloid shape).  
- Applications to engineering systems (hydraulic presses, storage tanks, ship stability).  

**Midterm**

---


### **Week 5: Navier–Stokes Equations**
- <span style="color: black;">Review of Newton’s second law and its application to fluids.</span>
- <span style="color: black;">Forces in fluid flow: pressure, body forces, and viscous forces.</span>
- <span style="color: black;">Derivation of the **Navier–Stokes equations** for incompressible flow.</span>

---

### **Week 6: Bernoulli’s Equation and Energy Conservation**
- Derivation of **Bernoulli’s equation** from the Euler equations for steady, incompressible, inviscid flow.
- Physical interpretation of Bernoulli’s equation as energy conservation.
- Practical applications of Bernoulli’s equation (nozzles, flow meters, venturi tubes).
- Limitations and conditions for Bernoulli’s equation.

---

### **Weeks 7-8: Control Volume Analysis and Integral Conservation Laws**
- <span style="color: black;">Introduction to the **Reynolds Transport Theorem (RTT)** as the bridge between system and control volume approaches.</span>
- <span style="color: black;">Application of RTT to derive the **integral conservation equations**:</span>  
  - **Continuity equation** (conservation of mass).  
  - **Momentum equation** (linear and angular momentum).  
  - **Energy equation** (first law of thermodynamics for control volumes).  
- <span style="color: black;">Assumptions and simplifications: steady flow, uniform flow, one-dimensional approximations.</span>
- <span style="color: black;">Applications of integral analysis to engineering systems:</span>  
  - Jet propulsion and rocket thrust.  
  - Forces on bends and nozzles in piping systems.  
  - Turbines and pumps (energy transfer).  
  - Flow over control surfaces and aerodynamic forces.  

**Midterm**


---

### **Weeks 9-10: Dimensional Analysis and Similarity**
- <span style="color: black;">Concept of dimensional homogeneity and the importance of nondimensionalization in fluid mechanics.</span>  
- <span style="color: black;">The **Buckingham Pi theorem**: procedure to identify dimensionless groups.</span>  
- <span style="color: black;">Key dimensionless numbers in fluid mechanics:</span>  
  - Reynolds number (inertia vs. viscous forces).  
  - Froude number (inertia vs. gravity forces).  
  - Mach number (inertia vs. compressibility effects).  
  - Weber number (inertia vs. surface tension).  
  - Strouhal number (unsteady vs. convective inertia).  
- <span style="color: black;">Modeling and similarity:</span> geometric, kinematic, and dynamic similarity.  
- <span style="color: black;">Applications in wind tunnel testing, hydraulic modeling, and prototype scaling.</span>  

---

### **Weeks 11-12: Differential Analysis of Fluid Flow**
- <span style="color: black;">Conservation of mass: **continuity equation** in differential form.</span>
- <span style="color: black;">Conservation of momentum: revisiting the **Navier–Stokes equations** for incompressible flow.</span>
- <span style="color: black;">Application of differential equations to simple 1D and 2D flows.</span>
- <span style="color: black;">Exact solutions of Navier–Stokes for simple cases: Couette flow, Poiseuille flow, stagnation flow.</span>
- <span style="color: black;">Concept of boundary conditions for viscous flows (no-slip, symmetry, far-field).</span>
- Velocity potential and stream function.

**Lab**: Computational exploration of Couette and Poiseuille flows using Python.

**Midterm**

---

### **Weeks 13-14: Viscous Flow and Internal Flow in Pipes**
- <span style="color: black;">Laminar vs. turbulent flow: **Hagen–Poiseuille equation** for laminar flow, transition criteria (Reynolds number).</span>  
- <span style="color: black;">Head loss in pipes: **Darcy–Weisbach equation** and empirical correlations.</span>  
- <span style="color: black;">Use of the **Moody chart** and friction factor correlations (Blasius, Colebrook–White equation).</span>  
- <span style="color: black;">Minor losses: fittings, bends, valves, expansions, and contractions.</span>  
- <span style="color: black;">Energy equation for pipe systems: combining major and minor losses.</span>  
- <span style="color: black;">Pipe networks:</span>  
  - Series and parallel pipe systems.  
  - Conservation of mass and energy at junctions (Hardy Cross method).  
  - Iterative and numerical methods for solving complex pipe networks.  
  - Use of computational tools for large networks.  

---

### **Week 15: Boundary Layers and External Flow**
- <span style="color: black;">Introduction to boundary layer concept: definition and physical significance.</span>  
- <span style="color: black;">Laminar vs. turbulent boundary layers.</span>  
- <span style="color: black;">Blasius solution (flat plate) and order-of-magnitude estimates.</span>  
- <span style="color: black;">Boundary layer thickness, displacement thickness, and momentum thickness.</span>  
- <span style="color: black;">Boundary layer separation and wake formation.</span>  
- <span style="color: black;">Drag: skin friction drag vs. pressure drag.</span>  
- <span style="color: black;">Lift generation: Kutta–Joukowski theorem (conceptual introduction).</span>  
- <span style="color: black;">Applications to external flow over cylinders, spheres, and airfoils.</span>  

---

### **Week 16: Turbomachinery**
- <span style="color: black;">Introduction to turbomachinery: classification (pumps, turbines, compressors, fans).</span>  
- <span style="color: black;">Basics of compressible flow: speed of sound, Mach number, and compressibility effects.</span>  
- <span style="color: black;">Compressible flow regimes: subsonic, transonic, supersonic, and their relevance in turbomachinery.</span>  
- <span style="color: black;">Euler’s turbine equation and energy transfer between fluid and rotor.</span>  
- <span style="color: black;">Performance analysis of pumps, turbines, and compressors (head, efficiency, specific speed).</span>  
- <span style="color: black;">Cavitation: causes, effects on performance, and design strategies to mitigate it.</span>  
- <span style="color: black;">Performance curves and characteristic maps: interpretation and applications.</span>  
- <span style="color: black;">Case studies: hydraulic turbines for hydropower, axial compressors in jet engines.</span>  

**Midterm**

## Assessments
- 3 Laboratory Reports (in-lab experiments and computational): 14%
- Midterm Exams (4): 76%
- Free-topic presentation / experiment: 10%

## Material

- **Cengel, Yunus A., and John M. Cimbala.** Fluid Mechanics: Fundamentals and Applications. McGraw-Hill, 2018. {cite}`cengel2018`
- **White, Frank M.** Fluid Mechanics. McGraw-Hill, 2016. {cite}`white2016`
- **Munson, Bruce R., Donald F. Young, Theodore H. Okiishi, and Wade W. Huebsch.** Fundamentals of Fluid Mechanics. Wiley, 2012. {cite}`munson2012`
- **Shames, Irving H.** Mechanics of Fluids. McGraw-Hill, 2003. {cite}`shames2003`
- **Fox, Robert W., Alan T. McDonald, and Philip J. Pritchard.** Introduction to Fluid Mechanics. Wiley, 2011. {cite}`fox2011`
