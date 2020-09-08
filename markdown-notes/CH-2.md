# CH-2

[TOC]

## 2-1 Material Strength and Stiffness

### Stress and Strain

#### Definition

<div align = center><img src = "/assets/CH2-1.png"></div>

$$
\sigma = \frac{P}{A_0}\\[2ex]
\epsilon = \frac{l-l_0}{l_0}\\[2ex]
$$

#### Graphs of Different Materials

<div align = center><img src = "/assets/CH2-2.png"></div>

These are the graphs of the ductile material and the brittle material

- $pl$: the proportional limit, where we can get the Hooke's law
    $\sigma = E\epsilon$
- $el$: the elastic limit, where the further load will cause the plastic deformation
- yield point: a point where the strain begin to increase very rapidly without a corresponding increase in stress
- $S_y$: yield strength, which is defined by offset method, usually 0.2 percent of the original gauge length ($\epsilon=0.002$)
- $S_u$ or $S_{ut}$: the maximum stress

#### Engineering Strain

$$
\epsilon =\int_{l_0}^l{\frac{\mathrm{d}l}{l}}=\ln{\frac{l}{l_0}}
$$

the engineering strain is based on net change in length from the original length

### Torsional Strength

#### Definition

$$
\tau_{max} = \frac{Gr}{l_0}\theta\\[2ex]
\tau_{max} = \frac{Tr}{J}
$$

- $G$: the shear modulus
- $r$: the radius of the specimen
- $l_0$: the gauge length
- $T$: the applied torque
- $J$: the polar second moment of area of the cross section

$$
S_u = \frac{T_u r}{J}
$$

- $S_u$: the modulus of rupture for the torsion test

### Resilience

#### Definition

Capacity of a material to absorb energy within its elastic range

**Modulus of resilience $u_R$**:

- **Energy absorbed per unit volume without permanent deformation**
- Equals the *area under the stress-strain curve* up to the elastic point
- Elastic limit often approximated by **yield point**

$$
u_R \approxeq \int_0^{\epsilon_y}{\sigma\mathrm{d}\epsilon}
$$

if elastic region is linear

$$
u_R \approxeq \frac{1}{2}S_y\epsilon_y = \frac{1}{2}(S_y)(S_y/E) = \frac{S_y^2}{2E}
$$

## 2-2 Statistical Significance of Material Properties

## Hardness
