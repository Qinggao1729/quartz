---
title: "Fundamental Theorem of Calculus"
tags:
- ideas 
- MultivariableCalculus
---
#ideas 

Integral of [[Derivative]] over a region = function over a boundary

Sum up the total weight or amount of a function described in input space.

# 1D
$f: R\to R$
$$\int_{a}^{b} \frac{\mathrm{d} f}{\mathrm{d} x} \mathrm{d}x=f(b)-f(a)$$
Integral of [[Derivative]] over a 1D region (or line) living in 1D space = difference of function at two 0D boundary (or endpoint)

# [[Vector line integral]] in Higher Dimensions
[[Mapping]]: $f: R^{n}\to R$, $\nabla{f}:R^{n} \to R^{n}$

$$\int_{C} \nabla f \cdot \mathrm{d} \vec{r}=f[\vec{r}(t=b)]-f[\vec{r}(t=a)]$$
(see: [[Gradient]])

Integral of [[Derivative]] over a 1D region (or line) living in nD space = difference of function at two 0D boundary (or endpoint)
## Proof
Assign [[Vector field]] $\vec{F}(x,y,z)=\nabla{f}$

[[Chain rule]]

[[Fundamental Theorem of Calculus#1D]]

# [[Surface integral]]
[[Mapping]]: $\vec{F}(x,y)=(P,Q): R^{2}\to R^{2}$
At any point on the boundary, we can decompose the [[Vector field]] $\vec{F}$ into a [[Tangential component]] and a [[Normal component]]
$$\vec{F}=[\vec{F}\cdot \vec{T}]\vec{\tau}+[\vec{F}\cdot \vec{n}]\vec{n}$$
where $\vec{\tau}$ and $\vec{n}$ are unit vectors in tangential and normal direction, respectively.
## Collecting [[Tangential component]]

[[Green's Theorem]]: 

$$\oint_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\oint_{C} P \mathrm{d}  x+Q \mathrm{d}  y=\iint_{A}\left[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right] \mathrm{d} x \mathrm{d} y$$

Integral of $[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}]$ (which are 2 derivatives) over a 2D region (or surface) living in 2D space = function $\vec{F}$ over a 1D boundary (or closed curve)

Also, Sum up rotations inside = rotation of the outside (boundary) (which is a [[Vector line integral]])

(see: [[Curl]] for rotation inside, [[Vector line integral#Rotation]] for rotation outside)

We can view Green's Theorem as collecting all the [[Tangential component]] of $\vec{F}$ over the boundary, since

$$\int_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\int_{C} \vec{F} \cdot \vec{T} \mathrm{d} C$$

(see: [[Vector line integral#Definition]])
## Collecting [[Normal component]]
$\vec{F}\cdot \vec{n}\mathrm{d}s$ is the normal component

Unit tangent vector is $\vec{T}(t)=(\frac{x^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|}, \frac{y^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|})$

Since $\vec{T} \cdot \vec{n}=0$, unit normal vector is $\vec{n}(t)=(\frac{y^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|} , -\frac{x^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|} )$ (see: [[Orientation#Normal of Curve in 2D]])

$$\int_{C} \vec{F} \cdot \vec{n} \mathrm{d} s =\int_{a}^{b}(\vec{F} \cdot \vec{n}(t))\left|\vec{r}^{\prime}\right| \mathrm{d} t=\int_{a}^{b}\left[P \frac{y^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|}-Q \frac{x^{\prime}(t)}{\left|\vec{r}^{\prime}(t)\right|}\right]\left|\vec{r}^{\prime}(t)\right| \mathrm{d} t$$
$$=\int_{a}^{b}\left[P y^{\prime}(t)-Q x^{\prime}(t)\right] \mathrm{d} t  =\int_{C} -Q \mathrm{d} x +P \mathrm{d} y$$
From [[Green's Theorem]], we have $\oint_{C} -Q \mathrm{d} x +P \mathrm{d} y=\iint_{A}\left[\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right] \mathrm{d} x \mathrm{d} y$, then
$$\oint_{C} \vec{F} \cdot \vec{n} \mathrm{d} s =\oint_{C} -Q \mathrm{d} x +P \mathrm{d} y=\iint_{A}\left[\frac{\partial P}{\partial x}+\frac{\partial Q}{\partial y}\right] \mathrm{d} x \mathrm{d} y=\iint_{A} \nabla \cdot \vec{F} \mathrm{d} x \mathrm{d} y$$

