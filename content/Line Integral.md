---
title: "Line Integral"
---
Idea: [[Fundamental Theorem of Calculus]]
# 1D to 1D
Integrate a [[Scalar function]] over a 1D object in input space, object living in 1D output space
The object is a [[Mapping#from 1D to 1D]]
$$\int_{a}^{b}f(x)\mathrm{d}x=\int_{t_{start}=a}^{t_{end}=b}f(x(t))\mathrm{d}t$$

# 1D to 2D

Integrate a [[Scalar function]] over a 1D object in input space, object living in 2D output space
The object is a [[Mapping#from 1D to 2D]], while the function is $f(x,y): R^{2} \to R$
integrate $f(x,y)$ along the curve $C$: integral **with respect to arc length**


$$\int_{C}f(C)\mathrm{d}C=\int_{t_{start}}^{t_{end}}f(C)\mathrm{d}C=\int_{t_{start}}^{t_{end}}f(x(t),y(t))\mathrm{d}C=\int_{t_{start}}^{t_{end}}f(x(t),y(t))\sqrt{x_{t}^{2}+y_{t}^{2}}\mathrm{d}t$$

# Partial Integral
(It is a random name.)
Integrate a [[Scalar function]] $f(x,y): R^{2} \to R$ **with respect to $x$** as you move along the curve $C$
$\int_{C}f(x,y)\mathrm{d}x=\int_{C}f(x(t),y(t))\frac{\mathrm{d}x}{\mathrm{d}y}\mathrm{d}t$

# 1D to 3D
The object is a [[Mapping#from 1D to 3D]].
The line integral of scalar function $f(x,y): R^{3} \to R$ over C is
$$\int_{t_{start}}^{t_{end}}f(x(t),y(t),z(t))\sqrt{x_{t}^{2}+y_{t}^{2}+z_{t}^{2}}\mathrm{d}t$$
