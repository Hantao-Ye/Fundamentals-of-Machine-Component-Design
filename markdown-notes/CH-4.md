# CH-4

[TOC]

## 4-1 Springs

### Definition

A mechanical element that exerts a force when deformed. If we designate the general relationship between force and deflection by the equation

**spring rate**

$$
k(y) = \frac{\mathrm{d}F}{\mathrm{d}y}
$$

- k is constant for linear force-deflection problems

## 4-2 Deflection Due to Bending

the curvature of a beam subjected to a bending moment M is given by

$$
\frac{1}{\rho} = \frac{M}{EI}
$$

where $\theta = \frac{\mathrm{d}y}{\mathrm{d}x}$

$$
\begin{aligned}
    \frac{M}{EI} &= \frac{\mathrm{d}^2y}{\mathrm{d}x^2}\\[2ex]
    \frac{V}{EI} &= \frac{\mathrm{d}^3y}{\mathrm{d}x^3}\\[2ex]
    \frac{q}{EI} &= \frac{\mathrm{d}^4y}{\mathrm{d}x^4}\\[2ex]
\end{aligned}
$$

### Ex 4-1

Determine the equation for the slope and deflection of the beam, the slopes at the ends, and the max deflection

$$
\begin{aligned}
    M = \frac{wl}{2}x-\frac{w}{2}x^2\\[2ex]
\end{aligned}
$$

By using the bending moment equation we could get that

$$
\begin{aligned}
    EI v'' = EI \frac{\mathrm{d}^2y}{\mathrm{d}x^2}&=M\\[2ex]
    EI v' &= \int{\frac{wl}{2}x-\frac{w}{2}x^2\mathrm{d}x}=\frac{wl}{4}x^2-\frac{w}{6}x^3+C_1\\[2ex]
    EI v &= \frac{wl}{12}x^3-\frac{w}{24}x^4+C_1 x+C_2\\[2ex]
    x = 0 &\Longrightarrow C_2 = 0\\[2ex]
    x = l &\Longrightarrow C_2 = 0
\end{aligned}
$$

### Beam Deflections by Superposition

**superposition** revolves the effect of combined loading on a structure by determining the effects of each load *separately* and adding the results *algebraically*

and some common results have been calculated in the Table A-9

## 4-3 Strain Energy

### Definition

the external work done on an elastic member in deforming it is transformed in to **strain**, or **potential**, **energy**, which equals to the product of the average force and the deflection

$$
U = \int{\frac{F^2}{2AE}\mathrm{d}x} = \int{\frac{F^2}{2AG}\mathrm{d}x} = \int{\frac{T^2}{2GJ}\mathrm{d}x}
$$

which is the strain energy for **tension**, **direct shear** and **torsion**

### Strain Energy in Beam Bending

$$
\begin{aligned}
    U_{\text{bending}} &= \int{\frac{M^2}{2EI}\mathrm{d}x}\\[2ex]
    U_{\text{shear}} &= \int{\frac{CV^2}{2AG}\mathrm{d}x}
\end{aligned}
$$

## 4-4 Castigliano's Theorem

### Definition

when forces act on elastic systems subject to small displacements, the **displacement** corresponding to any force, in direction of the force, is equal to the **partial derivative** of the **total strain energy** with respect to that force

$$
\begin{aligned}
    \delta_i &= \frac{\partial{U}}{\partial{F_i}}\\[2ex]
    \delta_{\text{tension}} &= \int{\frac{1}{AE}\Big(F\frac{\partial{F}}{\partial{F_i}}\Big)}\\[2ex]
    \theta_{\text{torsion}} &= \int{\frac{1}{GJ}\Big(T\frac{\partial{T}}{\partial{M_i}}\Big)}\\[2ex]
    \delta_{\text{bending}} &= \int{\frac{1}{EI}\Big(M\frac{\partial{M}}{\partial{F_i}}\Big)}\\[2ex]
\end{aligned}
$$

### Procedures

- set up equation for the total strain energy
- find an expression for the desired deflection
- since Q is a fictitious force, solve the expression by setting Q equal to 0

## 4-5 Compression Member-General