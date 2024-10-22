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


# Prerequisites

## Mathematics Prerequisites
1. **Calculus I and II**:
   - Understanding of derivatives and integrals, especially related to functions of one or more variables.
   - Concepts of partial derivatives, chain rule, and multiple integrals.
   - Parametric equations and their applications.

2. **Differential Equations**:
   - Ability to solve ordinary differential equations (ODEs), which are essential for understanding fluid dynamics, particularly in deriving the Navier-Stokes equations and other conservation laws.
   - Familiarity with linear and non-linear differential equations.
   - Exposure to boundary value problems and initial conditions.

3. **Vector Calculus**:
   - Mastery of vector fields, gradient, divergence, and curl operations.
   - Line integrals, surface integrals, and volume integrals.
   - Understanding the physical meaning of the divergence theorem and Stokes' theorem, which are crucial in fluid flow analysis using control volumes and differential analysis.

4. **Linear Algebra (optional)**:
   - Some familiarity with matrices and solving systems of equations, particularly in computational aspects like numerical simulations or matrix-based methods for solving differential equations.

## Physics Prerequisites
1. **General Physics I (Mechanics)**:
   - Mastery of Newton's laws of motion and their application to different systems.
   - Knowledge of energy conservation (kinetic and potential energy) and momentum conservation, as these concepts directly translate to Bernoulli's equation and fluid statics.
   - Basics of forces, including gravitational forces and frictional forces.

2. **General Physics II (Electricity and Magnetism, optional)**:
   - Some exposure to wave propagation, which can help in understanding aspects of compressible flow and shock waves.
   - Familiarity with concepts like pressure fields, as similar ideas are used in both electromagnetism and fluid mechanics.

---

## Problem 1: Understanding Derivatives and Integrals

Given a function  $f(x)$, find the derivative and the integral of $f(x)$ over a given interval.

### Problem Statement:
Let $f(x) = x^3 - 3x^2 + 2x$.

1. Find $f'(x)$, the derivative of the function.
2. Calculate the integral $ \int f(x) dx $ over the interval [1, 4].

### Solution:

1. **Derivative**:  
   Using basic differentiation rules:

   $$
   f'(x) = 3x^2 - 6x + 2
   $$

2. **Integral**:  
   The indefinite integral is:
   
   $$
   \int (x^3 - 3x^2 + 2x) dx = \frac{x^4}{4} - x^3 + x^2 + C
   $$

   To evaluate the definite integral over the interval [1, 4]:
   
   $$
   \left[\frac{x^4}{4} - x^3 + x^2 \right]_{1}^{4}
   $$
   
   Substituting the limits and evaluating gives the final result for the definite integral.

For more problems and detailed solutions, you can visit the [MIT OCW problem set](https://ocw.mit.edu/courses/18-01sc-single-variable-calculus-fall-2010/pages/1.-differentiation/part-a-definition-and-basic-rules/problem-set-1/).


---


## Problem 2: Partial Derivatives, Chain Rule, and Multiple Integrals

### Problem Statement:
Let $z = f(x, y)$ where $x = u^2 + 3v$ and $y = uv$.

1. Find the partial derivative of $z$ with respect to $u$, denoted as $\frac{\partial z}{\partial u}$, using the chain rule.
2. Calculate the double integral of $z(x, y) = x + y$ over the region $R$, where $R$ is the square defined by $0 \leq x \leq 2$ and $0 \leq y \leq 1$.


### Solution:

#### 1. **Applying the Chain Rule**:

Let $f(x, y) = x + y$.

To find $\frac{\partial z}{\partial u}$, use the chain rule:

$$
\frac{\partial z}{\partial u} = \frac{\partial f}{\partial x} \cdot \frac{\partial x}{\partial u} + \frac{\partial f}{\partial y} \cdot \frac{\partial y}{\partial u}
$$

For the function $f(x, y) = x + y$:

$$
\frac{\partial f}{\partial x} = 1, \quad \frac{\partial f}{\partial y} = 1
$$

Next, calculate $\frac{\partial x}{\partial u}$ and $\frac{\partial y}{\partial u}$:

Given $x = u^2 + 3v$ and $y = uv$:

$$
\frac{\partial x}{\partial u} = 2u, \quad \frac{\partial y}{\partial u} = v
$$

Now substitute these into the chain rule equation:

$$
\frac{\partial z}{\partial u} = 1 \cdot 2u + 1 \cdot v = 2u + v
$$

Thus, the partial derivative of $z$ with respect to $u$ is:

$$
\frac{\partial z}{\partial u} = 2u + v
$$


#### 2. **Multiple Integrals**:

Now, let's compute the double integral of $z(x, y) = x + y$ over the region $R$, defined by $0 \leq x \leq 2$ and $0 \leq y \leq 1$.

The integral to solve is:

$$
\int_0^1 \int_0^2 (x + y) \, dx \, dy
$$

First, integrate with respect to $x$:

$$
\int_0^2 (x + y) \, dx = \int_0^2 x \, dx + \int_0^2 y \, dx = \left[ \frac{x^2}{2} \right]_0^2 + \left[ yx \right]_0^2
$$

Evaluating the integrals:

$$
\frac{2^2}{2} - 0 + y(2 - 0) = 2 + 2y
$$

Now, integrate with respect to $y$:

$$
\int_0^1 (2 + 2y) \, dy = \int_0^1 2 \, dy + \int_0^1 2y \, dy = \left[ 2y \right]_0^1 + \left[ y^2 \right]_0^1
$$

Evaluating the integrals:

$$
2(1 - 0) + (1^2 - 0^2) = 2 + 1 = 3
$$

Thus, the value of the double integral is:

$$
\int_0^1 \int_0^2 (x + y) \, dx \, dy = 3
$$


For more detailed problems and solutions, you can check out [Paul's Online Math Notes](https://tutorial.math.lamar.edu/) or [MIT OCW Multivariable Calculus](https://ocw.mit.edu/courses/18-02sc-multivariable-calculus-fall-2010/pages/2.-partial-derivatives/part-b-chain-rule-gradient-and-directional-derivatives/problem-set-5/).


---


## Problem 3: Parametric Equations and Applications

### Problem Statement:
A particle is moving along a curve defined by the following parametric equations:

$$
x(t) = 3t^2 - 2t
$$

$$
y(t) = 2t^3 - t
$$

where $x(t)$ and $y(t)$ represent the particle's position at time $t$.

1. Find the velocity and acceleration vectors of the particle at time $t$.
2. Determine the time $t$ when the particle’s velocity is zero.
3. Find the length of the curve traced by the particle between $t = 0$ and $t = 2$.


### Solution:

#### 1. Velocity and Acceleration Vectors:
To find the velocity and acceleration, we differentiate the parametric equations with respect to time $t$.

- **Velocity** is the derivative of position with respect to time:

  $$
  v_x(t) = \frac{dx}{dt} = 6t - 2
  $$

  $$
  v_y(t) = \frac{dy}{dt} = 6t^2 - 1
  $$

  Therefore, the velocity vector at time $t$ is:

  $$
  \mathbf{v}(t) = (6t - 2) \hat{i} + (6t^2 - 1) \hat{j}
  $$

- **Acceleration** is the derivative of velocity with respect to time:

  $$
  a_x(t) = \frac{d^2x}{dt^2} = 6
  $$

  $$
  a_y(t) = \frac{d^2y}{dt^2} = 12t
  $$

  Therefore, the acceleration vector is:

  $$
  \mathbf{a}(t) = 6 \hat{i} + 12t \hat{j}
  $$

#### 2. Time When the Particle's Velocity is Zero:
For the velocity to be zero, both components of the velocity vector must be zero simultaneously:

  $$
  6t - 2 = 0 \quad \text{and} \quad 6t^2 - 1 = 0
  $$

From $6t - 2 = 0$, solving for $t$ gives:

  $$
  t = \frac{1}{3}
  $$

Substituting $t = \frac{1}{3}$ into the second equation:

  $$
  6 \left(\frac{1}{3}\right)^2 - 1 = \frac{2}{3} - 1 = -\frac{1}{3} \neq 0
  $$

Thus, there is no time $t$ where the particle’s velocity is exactly zero in both the $x$ and $y$ directions.

#### 3. Length of the Curve:
The length of the curve traced by the particle from $t = 0$ to $t = 2$ is given by the formula:

  $$
  L = \int_0^2 \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2} \, dt
  $$

Substitute the derivatives $v_x(t) = 6t - 2$ and $v_y(t) = 6t^2 - 1$:

  $$
  L = \int_0^2 \sqrt{(6t - 2)^2 + (6t^2 - 1)^2} \, dt
  $$

This integral can be solved either numerically or using appropriate substitution techniques to find the length of the curve.


### Applications:
Parametric equations are widely used to describe curves and motions in physics, engineering, and computer graphics. For instance, they are used to model the trajectory of particles, motion along a path, and even design complex curves in computer-aided design (CAD) software.


---


## Problem 4: Separable Differential Equation

Solve the following first-order separable ODE:

$$
\frac{dy}{dx} = x^2 + x
$$

with the initial condition $y(1) = 3$.

### Solution:

To solve, integrate both sides with respect to $x$:

$$
y = \int (x^2 + x) \, dx = \frac{x^3}{3} + \frac{x^2}{2} + C
$$

Using the initial condition $y(1) = 3$, substitute $x = 1$ and $y = 3$:

$$
3 = \frac{1^3}{3} + \frac{1^2}{2} + C \quad \Rightarrow \quad 3 = \frac{1}{3} + \frac{1}{2} + C
$$

Solving for $C$, we get $C = \frac{15}{6}$, so the solution is:

$$
y = \frac{x^3}{3} + \frac{x^2}{2} + \frac{15}{6}
$$

---

## Problem 5: Exponential Growth

Solve the differential equation:

$$
\frac{dy}{dx} = e^x + x
$$

with the initial condition $y(0) = 10$.

### Solution:

To solve, integrate both sides with respect to $x$:

$$
y = \int (e^x + x) \, dx = e^x + \frac{x^2}{2} + C
$$

Using the initial condition $y(0) = 10$:

$$
10 = e^0 + \frac{0^2}{2} + C \quad \Rightarrow \quad 10 = 1 + C
$$

Thus, $C = 9$, and the solution is:

$$
y = e^x + \frac{x^2}{2} + 9
$$

---

## Problem 6: Separable Differential Equation

Solve the differential equation:

$$
\frac{dy}{dx} = \frac{1}{y}
$$

with the initial condition $y(1) = 2$.

### Solution:

This equation is separable, so we can rewrite it as:

$$
y \, dy = dx
$$

Next, integrate both sides:

$$
\int y \, dy = \int dx
$$

This gives:

$$
\frac{y^2}{2} = x + C
$$

Now, multiply by 2 to simplify:

$$
y^2 = 2x + 2C
$$

Using the initial condition $y(1) = 2$, substitute $x = 1$ and $y = 2$:

$$
2^2 = 2(1) + 2C \quad \Rightarrow \quad 4 = 2 + 2C
$$

Solving for $C$, we get:

$$
C = 1
$$

Thus, the solution is:

$$
y^2 = 2x + 2
$$

Taking the square root of both sides:

$$
y = \pm \sqrt{2x + 2}
$$

For the positive root, the solution is:

$$
y = \sqrt{2x + 2}
$$


---


## Problem 7: Linear and Non-Linear Differential Equations

Consider the following two differential equations:

1. **Linear Differential Equation**:  
   Solve the linear first-order differential equation:

   $$
   \frac{dy}{dx} + y = e^x
   $$

2. **Non-Linear Differential Equation**:  
   Solve the non-linear differential equation:

   $$
   \frac{dy}{dx} = y^2 - x
   $$

### Solution:

#### 1. **Linear Differential Equation**

The equation is of the form:

$$
\frac{dy}{dx} + P(x) y = Q(x)
$$

where $P(x) = 1$ and $Q(x) = e^x$.

**Step 1**: Find the integrating factor $\mu(x)$:

$$
\mu(x) = e^{\int P(x) \, dx} = e^{\int 1 \, dx} = e^x
$$

**Step 2**: Multiply both sides of the differential equation by the integrating factor $\mu(x)$:

$$
e^x \frac{dy}{dx} + e^x y = e^{2x}
$$

**Step 3**: The left-hand side is the derivative of $e^x y$, so we can rewrite the equation as:

$$
\frac{d}{dx} \left( e^x y \right) = e^{2x}
$$

**Step 4**: Integrate both sides:

$$
e^x y = \int e^{2x} \, dx = \frac{e^{2x}}{2} + C
$$

**Step 5**: Solve for $y$:

$$
y = \frac{e^x}{2} + Ce^{-x}
$$

Thus, the general solution is:

$$
y = \frac{e^x}{2} + Ce^{-x}
$$

---

#### 2. **Non-Linear Differential Equation**

The given equation is:

$$
\frac{dy}{dx} = y^2 - x
$$


This is a **non-linear** differential equation and does not have a straightforward analytical solution. However, it can be solved using numerical methods, such as **Euler's method**, or qualitative techniques like **direction fields** to analyze the behavior of the solutions. 

```{note}

While there is no simple analytic solution to present here, numerical solutions can be computed based on initial conditions.

We use the **Runge-Kutta method** to solve the differential equation:

```

$$
\frac{dy}{dx} = y^2 - x
$$

##### Python Code:

```{code-cell} python
import numpy as np
import matplotlib.pyplot as plt

# Function representing the ODE dy/dx = y^2 - x
def dydx(x, y):
    return y**2 - x

# Fourth-order Runge-Kutta method for numerical solution of ODE
def runge_kutta_method(dydx, x0, y0, x_end, h):
    x_values = np.arange(x0, x_end + h, h)
    y_values = np.zeros(len(x_values))
    y_values[0] = y0
    
    for i in range(1, len(x_values)):
        x = x_values[i-1]
        y = y_values[i-1]
        
        k1 = h * dydx(x, y)
        k2 = h * dydx(x + h/2, y + k1/2)
        k3 = h * dydx(x + h/2, y + k2/2)
        k4 = h * dydx(x + h, y + k3)
        
        y_values[i] = y + (k1 + 2*k2 + 2*k3 + k4) / 6
    
    return x_values, y_values

# Adjust the domain to avoid large values causing overflow
x0 = 0  # Initial x
y0 = 1  # Initial y
x_end_new = 1  # Limit the domain to avoid instability
h = 0.01  # Step size

# Solve the ODE using Runge-Kutta method with a smaller domain
x_values_rk_new, y_values_rk_new = runge_kutta_method(dydx, x0, y0, x_end_new, h)

# Plot the solution with the new domain
plt.plot(x_values_rk_new, y_values_rk_new, label="Numerical Solution (Runge-Kutta Method)", color="orange")
plt.xlabel('x')
plt.ylabel('y')
plt.title("Solution of $dy/dx = y^2 - x$ using Runge-Kutta Method")
plt.legend()
plt.grid(True)
plt.show()

```
