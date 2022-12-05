---
title: "Green's Theorem"
---
Idea: [[Fundamental Theorem of Calculus]]

Suppose $\vec{F}(x,y)=(P,Q)$

Let $C$ be a positively oriented (see [[Orientation]]), piecewise-smooth, simple closed curve surrounding region $A$. If $P$ and $Q$ have continuous partial derivatives on an open region that contains $A$, then

$$\oint_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\oint_{C} P \mathrm{d}  x+Q \mathrm{d}  y=\iint_{A}\left[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right] \mathrm{d} x \mathrm{d} y$$
(see [[Vector line integral]])

$C$ can be also noted as $\partial{A}$

Integral of $[\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}]$ over a 2D region (or surface) living in 2D space = function $\vec{F}$ over a 1D boundary (or closed curve)

$\left[\frac{\partial Q}{\partial x}=\frac{\partial P}{\partial y}\right]\leftrightarrow \oint_{C} \vec{F} \cdot \mathrm{d} \vec{r} \leftrightarrow \vec{F}$  is [[Path-independent]] $\leftrightarrow \vec{F}$ is [[Conservative]]

# Proof
for the case in which $A$ is a [[Simple region]].

* Show $\int_{C} P(x, y) \mathrm{d} x=-\iint_{D} \frac{\partial P}{\partial y} \mathrm{d} A$ by expressing D as a type I region
* Similarly, show $\int_{C} Q \mathrm{d} y=\iint_{D} \frac{\partial Q}{\partial x} \mathrm{d} A$ by expressing D as a type II region

But we can extend it to the case where $A$ is a finite union of simple regions.

It can also be extended to apply to regions with holes (not simply-connected), with properly-defined [[Orientation]] of boundaries.


> [!QUOTE]-
> George Green worked fulltime in his father’s bakery from the age of nine and taught himself mathematics from library books. In 1828 he published privately An Essay on the Application of Mathematical Analysis to the Theories of Electricity and Magnetism, but only 100 copies were printed and most of those went to his friends.

> [!QUESTION] How come he had friends?

