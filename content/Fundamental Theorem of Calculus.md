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
[[Mapping]]: $f: R^{n}\to R$, $\vec{F}=\nabla{f}:R^{n} \to R^{n}$

$$\int_{C} \nabla f \cdot \mathrm{d} \vec{r}=f[\vec{r}(t=b)]-f[\vec{r}(t=a)]$$
(see [[Gradient]])

Integral of [[Derivative]] over a 1D region (or line) living in nD space = difference of function at two 0D boundary (or endpoint)
## Proof
Assign [[Vector field]] $\vec{F}(x,y,z)=\nabla{f}$

[[Chain rule]]

[[Fundamental Theorem of Calculus#1D]]

# [[Surface integral]]
[[Mapping]]: $\vec{F}: R^{2}\to R^{2}$

[[Green's Theorem]]

Integral of $[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}]$ (which are 2 derivatives) over a 2D region (or surface) living in 2D space = function $\vec{F}$ over a 1D boundary (or closed curve)

Sum up rotations inside = rotation of the outside (boundary) (which is a [[Vector line integral]])

(see: [[curl]] for rotation)

So you can also view closed [[Vector line integral]] as a representation of rotation of $\vec{F}$ over the boundary, which makes sense, because if the [[Orientation]] of curve $C$ is positive, then more [[Tangential component]] occurs when $\vec{F}$ is in the same direction as $\mathrm{d}\vec{r}$, namely counterclockwise. 