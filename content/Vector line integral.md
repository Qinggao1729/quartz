---
title: "Vector line integral"
---
Idea: [[Fundamental Theorem of Calculus]]
integrate the [[Vector field]] $\vec{F}$ over the curve $C$, where $\vec{F}(x, y)=\left(f_{1}(x, y), f_{2}(x, y)\right)$
Both $\vec{F}$ and $C$ are 1D object living in 2D space.

# Why do this?
* We can talk about the projection of $F$ onto $C$
* It's an analogy of total work done in moving particle
# Definition
$C$ is given by $\vec{r}(t)$, then $\vec{r}^{\prime}(t)$ is tangent to curve $C$, then $\vec{F} \cdot \vec{r}^{\prime}(t)$ is the [[Tangential compenent]] of $\vec{F}$ along curve $C$.
$$\int_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\int_{C} \vec{F} \cdot \vec{r}^{\prime} \mathrm{d} t=\int_{C} \vec{F}(\vec{r}(t)) \cdot \vec{r}^{\prime} \mathrm{d} t$$
Also, unit tangent $\vec{T}=\frac{\vec{r}^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|}$, then $\mathrm{d}\vec{r}=\vec{T}\left|\vec{r}^{\prime}(t)\right|\mathrm{d}t$
$\left|\vec{r}^{\prime}(t)\right|$ is the [[Magic factor]] in [[Mapping#from 1D to 2D]]and [[Mapping#from 1D to 3D]]
So $\left|\vec{r}^{\prime}(t)\right|\mathrm{d}t = \mathrm{d}C$
$$\int_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\int_{C} \vec{F} \cdot \vec{T} \mathrm{d} C$$
# Calculate in "pieces"
Let $\vec{F}=(P(x, y), Q(x, y))$, and we have $\vec{r}^{\prime}(t)=\left(x^{\prime}(t), y^{\prime}(t)\right)$
$$\int_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\int_{C} \vec{F} \cdot \vec{r}^{\prime} \mathrm{d} t=\int_{C} P(x, y) x^{\prime}(t) \mathrm{d}t+\int_{C} Q(x, y) y^{\prime}(t) \mathrm{d}t
=\int_{C} P(x, y) \mathrm{d}x+\int_{C} Q(x, y) \mathrm{d}y$$
Or intuitively, that's from $\mathrm{d} \vec{r}=(\mathrm{d} x, \mathrm{d} \vec{y})$
