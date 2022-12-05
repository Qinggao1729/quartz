---
title: "Curl"
---
Idea: 

Convert [[Vector field]] $\vec{F}(x,y,z)=(P,Q,R)$ ([[Mapping]]: $R^{3}\to R^{3}$)  to a 3D vector.

$\nabla \times \vec{F} = \left(\frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z}, \quad \frac{\partial P}{\partial z}-\frac{\partial R}{\partial x}, \quad \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}\right)$

(see: [[Nabla]])

# Geometric Intuition
Consider $\vec{F}=(P(x,y),Q(x,y),0)$ 

Then $\nabla \times \vec{F}=(0,0,(\frac{\partial{Q}}{\partial{x}}- \frac{\partial{P}}{\partial{y}}))$

$\frac{\partial{Q}}{\partial{x}}>0$ and $\frac{\partial{P}}{\partial{y}}<0$ should contribute to a counterclockwise rotation.

$\frac{\partial{Q}}{\partial{x}}<0$ and $\frac{\partial{P}}{\partial{y}}>0$ should contribute to a clockwise rotation.
# $\nabla \times \vec{F}=0 \leftrightarrow \vec{F}$ is [[Conservative]]
## $\nabla \times \vec{F}=0 \leftarrow \vec{F}$ is [[Conservative]]
