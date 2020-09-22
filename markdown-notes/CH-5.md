# CH-5

[TOC]

## 5-1 Failure Theories

Unfortunately, there is **no universal theory** of theory of failure for the general case of material properties and stress state.

Instead, several hypotheses have been formulated and tested, leading to today's accepted practices most designers do

<div align = center><img src = "../assets/CH5-1.png"></div>

## 5-2 Maximum-Shear-Stress Theory for Ductile Materials

### Definition

yielding begins whenever the maximum shear stress in any element equals or exceeds the maximum shear stress in a tension-test specimen of the same material when that specimen begins to yield

### Procedures

- case 1: $\sigma_A\geq\sigma_B\geq 0$
$$
    \sigma_A\geq S_y
$$
- case 2: $\sigma_A\geq 0\geq\sigma_B$
$$
    \sigma_A-\sigma_B\geq S_y
$$
- case 3: $0\geq\sigma_A\geq\sigma_B$
$$
    \sigma_B\leq -S_y
$$

## 5-3 Distortion-Energy Theory for Ductile Materials

### Definition

yielding begins whenever the maximum shear stress in any element equals or exceeds the maximum shear stress in a tension-test specimen of the same material when that specimen begins to yield. 

### Procedures

$$
\sigma_{av} = \frac{\sigma_1+\sigma_2+\sigma_3}{3}
$$

since the strain energy per unit volume for simple tension is $u = \frac{1}{2}[\epsilon_1\sigma_1+\epsilon_2\sigma_2+\epsilon_3\sigma_3]$, which equals to 

$$
u = \frac{1}{2E}[\sigma_1^2+\sigma_2^2+\sigma_3^2-2\nu(\sigma_1\sigma_2+\sigma_2\sigma_3+\sigma_3\sigma_1)]
$$

and the average strain energy could be expressed like

$$
\begin{aligned}
    u_{v} &= \frac{3\sigma_{av}^2}{2E}(1-2\nu)\\[2ex]
          &= \frac{1-2\nu}{6E}(\sigma_1^2+\sigma_2^2+\sigma_3^2+2\sigma_1\sigma_2+2\sigma_2\sigma_3+2\sigma_3\sigma_1)
\end{aligned}
$$

the distortion energy could be obtained by the following equation

$$
u_d = u-u_v = \frac{1+\nu}{6E}((\sigma_1-\sigma_2)^2+(\sigma_2-\sigma_3)^2+(\sigma_3-\sigma_1)^2)
$$

since the distortion energy for tension test specimen is

$$
u_d = \frac{1+\nu}{3E}S_y^2
$$

therefore the relationship becomes

$$
\Big[\frac{(\sigma_1-\sigma_2)^2+(\sigma_2-\sigma_3)^2+(\sigma_3-\sigma_1)^2}{2}\Big]^{1/2} \geq S_y
$$

let $\sigma'$ as the minimum stress

#### Plane Stress

for the plane stress, there're only principal stress and 0 on z-axis

$$
\sigma' = (\sigma_A^2-\sigma_A\sigma_B+\sigma_B^2)^{1/2}
$$

#### Three-Dimensional Stress

for three dimensional stress, there're only tension on x and y, and shear on xy

$$
\sigma' = \frac{1}{\sqrt{2}}[(\sigma_x-\sigma_y)^2+(\sigma_y-\sigma_z)^2+(\sigma_z-\sigma_x)^2+6(\tau_{xy}^2+\tau_{yz}^2+\tau_{zx}^2)]^{1/2} = (\sigma_x^2-\sigma_x\sigma_y+\sigma_x^2+3\tau_{xy}^2)^{1/2}
$$

#### Pure Shear

for the case of pure shear, where for plane stress = 0 

$$
(3\tau_{xy}^2)^{1/2} = S_y
$$

## 5-4 Coulomb-Mohr Theory for Ductile Materials

Since the Mohr's theory dated back to 1900, a new method gives fix on this theory

### Procedures

- Case 1: $\sigma_A\geq \sigma_B\geq0$

$$
\sigma_A\geq S_t
$$

- Case 2: $\sigma_A\geq0\geq\sigma_B$

$$
\frac{\sigma_A}{S_t}-\frac{\sigma_B}{S_c} \geq1
$$

- Case 3: $0\geq\sigma_A\geq \sigma_B$

$$
\sigma_B\leq -S_c
$$

#### Factor of Safety

$$
\frac{\sigma_1}{S_t}- \frac{\sigma_3}{S_c} = \frac{1}{n}
$$

#### Pure Torsion

the pure shear $\tau$, $\sigma_1 = -\sigma_3 = \tau$. The torsional yield strength occurs when $\tau_{max} = S_{xy}$

$$
S_{xy} = \frac{S_{yt}S_{yc}}{S_{yt}+S_{yc}}
$$

## 5-5 Maximum-Normal-Stress Theory for Brittle Materials

### Definition

failure occurs whenever one of the three principal stresses equals or exceeds the strength

### Procedures

- Case 1: $\sigma_1\geq \sigma_2\geq \sigma_3$

$$
\sigma_1\geq S_{ut}\qquad \sigma_3\leq -S_{uc}
$$

- Case 2: $\sigma_A\geq \sigma_B$

$$
\sigma_A\geq S_{ut}\qquad \sigma_B\leq -S_{uc}
$$

## 5-6 Modification of Mohr Theory for Brittle Materials

### Brittle Coulomb Mohr

- $\sigma_A\geq\sigma_B\geq0$

$$
\sigma_A = \frac{S_{ut}}{n}
$$

- $\sigma_A\geq0\geq\sigma_B$

$$
\frac{\sigma_A}{S_{ut}}-\frac{\sigma_B}{S_{uc}} = \frac{1}{n}
$$

- $0\geq\sigma_A\geq\sigma_B$

$$
\sigma_B = -\frac{S_{uc}}{n}
$$

### Modified Mohr

- $\sigma_A\geq\sigma_B\geq0$ or $\sigma_A\geq0\geq\sigma_B$ and $|\frac{\sigma_B}{\sigma_A}|\leq 1$

$$
\sigma_A = \frac{S_{ut}}{n}
$$

- $\sigma_A\geq0\geq\sigma_B$ and $|\frac{\sigma_B}{\sigma_A}|> 1$

$$
\frac{(S_{uc}-S_{ut})\sigma_A}{S_{uc}S_{ut}}-\frac{\sigma_B}{S_{uc}} = \frac{1}{n}
$$

- $0\geq\sigma_A\geq\sigma_B$

$$
\sigma_B = -\frac{S_{uc}}{n}
$$