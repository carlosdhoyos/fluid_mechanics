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

## Problem: Understanding Derivatives and Integrals

Given a function \( f(x) \), find the derivative and the integral of \( f(x) \) over a given interval.

### Problem Statement:
Let \( f(x) = x^3 - 3x^2 + 2x \).

1. Find \( f'(x) \), the derivative of the function.
2. Calculate the integral \( \int f(x) dx \) over the interval [1, 4].

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
