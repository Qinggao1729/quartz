---
title: "Conservative"
---
[[Gradient]]

A [[Vector field]] $\vec{F}$ is conservative if there exists a [[Scalar function]] $f$ such that  $\nabla f = \vec{F}$



# $\vec{F}$ is conservative $\leftrightarrow \vec{F}$ is [[Path-independent]]
## $\vec{F}$ is conservative $\rightarrow \vec{F}$ is [[Path-independent]]
$\int_{C} \vec{F} \cdot \mathrm{d} \vec{r}=\int_{C} \nabla f \cdot \mathrm{d} \vec{r}=f[\vec{r}(t=b)]-f[\vec{r}(t=b)]$ by [[Fundamental Theorem of Calculus#Vector Line Integral in Higher Dimensions]]
## $\vec{F}$ is conservative $\leftarrow \vec{F}$ is [[Path-independent]]
Letting $\vec{F}(x,y)=(P(x,y),Q(x,y))$
Define $f(x, y)=\int_{(a, b)}^{(x, y)} \vec{F} \cdot \mathrm{d} \vec{r}$
Then $f(x, y)=\int_{(a,b)}^{(a,y)} \vec{F} \cdot \mathrm{d} \vec{r}+\int_{(a,y)}^{(x,y)} \vec{F} \cdot \mathrm{d} \vec{r}$, because of path-independent
Then $f(x,y)=\int_{b}^{y} Q(a,y) \mathrm{d}y+\int_{a}^{x} P(x,y)\mathrm{d}x$, because $\mathrm{d}\vec{r}=(0,\mathrm{d}y)$ for the first part, and $\mathrm{d}\vec{r}=(\mathrm{d}x,0)$ for the second part ([[Vector line integral#Calculate in pieces]])
So $f_{x}=P$, $f_{y}=Q$ by [[Fundamental Theorem of Calculus#1D Calculus]]



# $\vec{F}$ is conservative $\leftrightarrow P_{y}=Q_{x}$
Letting $\vec{F}(x,y)=(P(x,y),Q(x,y))$

## $\vec{F}$ is conservative $\rightarrow P_{y}=Q_{x}$
Because if $\vec{F}$ is conservative, then there exists $f(x,y)$ such that $\nabla{f}=(f_{x}, f_{y})=\vec{F}=(P,Q)$

So, $P_{y}=f_{xy}$ and $Q_{x}=f_{yx}$, and they are the same by [[Clairaut's Theorem]]
## $\vec{F}$ is conservative $\leftarrow P_{y}=Q_{x}$
if that region is simply connected (no holes) ...