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
\begin{aligned}
\tau_{max} &= \frac{Gr}{l_0}\theta\\[2ex]
\tau_{max} &= \frac{Tr}{J}\\[2ex]
\end{aligned}
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

<div align = center><img src = "/assets/CH2-3.png"></div>

**Modulus of resilience $u_R$**:

- **Energy absorbed per unit volume without permanent deformation**
- Equals the *area under the stress-strain curve* up to the elastic point
- Elastic limit often approximated by **yield point**

$$
u_R \approx \int_0^{\epsilon_y}{\sigma\mathrm{d}\epsilon}
$$

if elastic region is linear

$$
u_R \approxeq \frac{1}{2}S_y\epsilon_y = \frac{1}{2}(S_y)(S_y/E) = \frac{S_y^2}{2E}
$$

### Toughness

#### Definition

the capacity of a material to absorb energy without fracture is called toughness

<div align = center><img src = "/assets/CH2-4.png"></div>

$$
u_T = \int_0^{\epsilon_f}{\sigma\mathrm{d}\epsilon}
$$

- $\epsilon_f$: the strain at the fracture point

$$
u_T \approx (\frac{S_y+S_{ut}}{2})\epsilon_f
$$

## 2-2 Statistical Significance of Material Properties

Strength values are obtained from testing many nominally identical specimens

Strength, a material property, is distributional and thus statistical in nature

**statistical quantity is defined by**:

- mean
- standard deviation
- distribution type

## 2-3 Strength and Cold Work

### Strengths from Tables

Property tables often only report a single value for a strength term

Common to use 99% min strength, indicating 99% of samples exceed the reported value

### Cold Work

#### Definition
<div align = center><img src = "/assets/CH2-5.png"></div>

- process of plastic straining **below recrystallization temperature** in the *plastic region* of stress-strain diagram
- loading to point i beyond yield point, then unloading, causes **permanent plastic deformation**
- reloading to point i behaves elastically, with additional elastic strain

$$
\epsilon = \epsilon_p+\epsilon_e = \epsilon_p+\frac{\sigma_i}{E}
$$

- yield point is effectively increased to point i
- material is less ductile since the plastic zone between yield strength and ultimate strength is reduced
- repeated strain hardening can lead to brittle failure

therefore there's a reduction in area called $R$, which is a measure of ductility

$$
R = \frac{A_0-A_f}{A_0}=1-\frac{A_f}{A_0}
$$

> **Ductility** represents the ability of a material to absorb **overloads** and **to be cold-worked**

## 2-4 Hardness

### Definition

the resistance of a material penetration by a pointed tool

**common hardness-measuring systems**:

- Rockwell
- Brinell
- Vickers

### Brinell hardness number

For steels

$$
S_u = \begin{cases}
    0.5H_B\quad \text{kpsi}\\[2ex]
    3.4H_B\quad \text{MPa}\\[2ex]
\end{cases}
$$

For cast iron

$$
S_u = \begin{cases}
    0.23H_B-12.5\quad \text{kpsi}\\[2ex]
    1.58H_B-86\quad \text{MPa}\\[2ex]
\end{cases}
$$

## 2-5 Impact Properties

Charpy notched-bar test is used to determine brittleness and impact strength

Specimen struck by pendulum

Energy absorbed: computed from height of swing after fracture


