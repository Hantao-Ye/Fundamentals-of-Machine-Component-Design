# CH-3

[TOC]

## 3-1 Equilibrium and Free-Body Diagrams

### Equilibrium

$$
\sum{F} = 0\qquad \sum{M}=0
$$

A system with zero acceleration is said to be in **equilibrium**, if that system is motionless or, at most, has constant velocity.

### Free-Body Diagram

Free-body diagrams help simplifying the analysis of a very complex structure or machine by successively isolating each element and then studying and analyzing it.

## 3-2 Shear Force and Bending Moments in Beams

### Definition

$$
\begin{aligned}
V &= \frac{\mathrm{d}M}{\mathrm{d}x}\\[2ex]
\frac{\mathrm{d}V}{\mathrm{d}x}&=\frac{\mathrm{d}^2M}{\mathrm{d}x^2}=q
\end{aligned}
$$

## 3-3 Cartesian Stress Components

### Definition

**Normal stress** is normal to a surface, designated by $\sigma$

**Shear stress** is tangent to a surface, designated by $\tau$

### Plane-Stress Transformation Equations

$$
\begin{aligned}
    \sigma &= \frac{\sigma_x+\sigma_y}{2}+\frac{\sigma_x-\sigma_y}{2}\cos2\phi+\tau_{xy}\sin2\phi\\[2ex]
    \tau &= -\frac{\sigma_x-\sigma_y}{2}\sin2\phi+\tau_{xy}\cos2\phi
\end{aligned}
$$

### Principal Stresses for Plane Stress

$$
\sigma_1, \sigma_2 = \frac{\sigma_x+\sigma_y}{2}\pm\sqrt{(\frac{\sigma_x-\sigma_y}{2})^2+\tau_{xy}^2}
$$

### Principal Directions

$$
\tan2\phi_P = \frac{2\tau_{xy}}{\sigma_x-\sigma_y}
$$

### Maximum Shear Stress

$$
\tau_1,\tau_2 = \pm\sqrt{(\frac{\sigma_x-\sigma_y}{2})^2+\tau_{xy}^2}
$$

### Mohr's Circle Diagram

<div align = center><img src = "/assets/CH3-1.png"></div>

- center: $\frac{\sigma_x+\sigma_y}{2}$
- radius: $\sqrt{(\frac{\sigma_x-\sigma_y}{2})^2+\tau_{xy}^2}$
- $2\phi_P$: $\frac{2\tau_{xy}}{\sigma_x-\sigma_y}$
- $\phi_S$: $\frac{\pi}{4}-\phi_P$

## 3-4 General Three-Dimensional Stress

<div align = center><img src = "/assets/CH3-2.png"></div>

where

$$
\tau_{1/2} = \frac{\sigma_1-\sigma_2}{2}\qquad\tau_{2/3}=\frac{\sigma_2-\sigma_3}{2}\qquad\tau_{1/3}=\frac{\sigma_1-\sigma_3}{2}
$$

## 3-5 Elastic Strain

### Hooke's Law

$$
\sigma = E\epsilon
$$

- $E$: Young's modulus, or modulus of elasticity

Tension in one direction produces negative strain in a perpendicular direction

$$
\epsilon_x = \frac{\sigma_x}{E}\qquad \epsilon_y=\epsilon_z = -\mu\frac{\sigma_x}{E}
$$


- $\mu$: the Poisson's ratio

### 3-Dimensional Cases

$$
\begin{aligned}
\epsilon_x &= \frac{1}{E}[\sigma_x-\mu(\sigma_y+\sigma_z)]\\[2ex]
\epsilon_y &= \frac{1}{E}[\sigma_y-\mu(\sigma_x+\sigma_z)]\\[2ex]
\epsilon_z &= \frac{1}{E}[\sigma_z-\mu(\sigma_x+\sigma_y)]\\[2ex]
\end{aligned}
$$

### Hooke's Law for Shear

$$
\tau = G\gamma
$$

- $G$: the shear modules of elasticity

> for a linear, isotropic and homogeneous material **$E = 2G(1+\mu)$**

## 3-6 Stresses

### Uniformly Distributed Stresses

**For tension and compression**

$$
\sigma = \frac{F}{A}
$$

**For direct shear**

$$
\tau = \frac{V}{A}
$$

### Normal Stresses for Beams in Bending

the beam is subjected to pure bending, which means the shear force is zero and that no torsion or axial loads are present

| <img src = "/assets/CH3-3.png"> | <img src = "/assets/CH3-4.png"> |
| :-----------------------------: | :-----------------------------: |

the bending stress varies linearly with the distance from the neutral axis

$$
\sigma_x = -\frac{My}{I}
$$

where $I$ is the second-area moment about the z-axis

$$
I = \int{y^2\mathrm{d}A}
$$

and the maximum magnitude of the bending stress will occur where $y$ has the greatest magnitude, where c is the neutral axis

$$
\sigma_{max} = \frac{Mc}{I}
$$

### Two-Plane Bending

cross sections with one or two planes of symmetry only

$$
\sigma_x = -\frac{M_z y}{I_z}+\frac{M_y z}{I_y}
$$

for solid circular cross section, the maximum bending stress is

$$
\sigma_m = \frac{Mc}{I} = \frac{\sqrt{M_y^2+M_z^2}(d/2)}{\pi d^4/64} = \frac{32}{\pi d^3}\sqrt{M_y^2+M_z^2}
$$

### Shear Stresses for Beams in Bending

$$
\tau = \frac{VQ}{Ib}
$$

where $Q$ is the first moment of the area

$$
Q = \int_{y_1}^c{y\mathrm{d}A}
$$

the traverse shear stress in common cross sections 
<div align = center><img src = "/assets/CH3-5.png"></div>


## 3-6 Torsion

### the Round Plane

$$
\theta = \frac{TI}{GJ}
$$

- $T$: torque
- $l$: length
- $G$: modulus of rigidity
- $J$: polar second moment of area

and shear stresses develop throughout the cross section

$$
\tau = \frac{T\rho}{J}\qquad \tau_{max} = \frac{Tr}{J}
$$

where the second polar moment for the solid round section is

$$
J = \frac{\pi d^4}{32}
$$

### Power, Speed and Torque

Power equals torque times speed

$$
H = T\omega
$$

A convenient conversion with speed in rpm

$$
T = 9.55\frac{H}{n}
$$