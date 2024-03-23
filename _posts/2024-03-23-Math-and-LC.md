---
title: Math and Liquid Crystals
date: 2024-03-23
categories: [Liquid Crystals, Math]
tags: [soft matter] # TAG names should always be lowercase
math: true
toc: true
---

The purpose of this article is to briefly describe some of the principal properties of liquid crystals and how they can be described mathematically.

Let's begin by assuming that the liquid crystal (LC) lives in some domain $\Omega\subset R^3$, then, we can describe the configuration of the LC at one point $\mathbf{x}$ by the director $\mathbf{n}(\mathbf{x})$, which is a unit vector giving the mean orientation of $\mathbf{x}$ of the rod like molecules in the system. In mathematical terms, we say that $\mathbf{n}(\mathbf{x})\in S^2$, where $S^2$ is the 2-sphere, which lives in $R^3$.
Now, there are many theories on which we can describe the LC, the principal two are via the Osen-Frank Energy and the Landau-de Gennes Theory.

## Osen-Frank Energy (vector field)

Def.(Free Energy) In this model, the free energy is given by

$$I(\mathbf{n}) = \int_{\Omega}W(\mathbf{n},\nabla\mathbf{n})d\mathbf{x},$$

where the $W$ function is given by

$$W(\mathbf{n},\nabla\mathbf{n}) = K_{1}(\nabla\cdot\mathbf{n})^2 + K_{2}(\mathbf{n}\cdot\nabla\times\mathbf{n})^2 + K_{3}|\mathbf{n}\wedge\nabla\times\mathbf{n}|^{2}+(K_{2} + K_{4})[tr(\nabla\mathbf{n})^{2} - (\nabla\cdot\mathbf{n})^2],$$

and the constants $K_i$ are called Frank constants, which are usually assumed to satisfy the strict form of the Ericksen inequalities, that is

$$K_{1}>0, K_{2} > 2, K_{3} > 0, K_2>|K_{4}|, 2K_{1}>K_{2} + K_{4},$$

and this conditions are necessary and sufficient to prove that

$$W(\mathbf{n},\nabla\mathbf{n})>c_{0}|\nabla\mathbf{n}|^2,\forall\mathbf{n},c_{0}>0,$$

and it's also important to say that every one of the elements in the OF free energy has it's own name and correspond to a specific deformation of the director:

- Splay: $\rightarrow K_{1}(\nabla\cdot\mathbf{n})^2.$
- Twist: $\rightarrow K_{2}(\mathbf{n}\cdot\nabla\times\mathbf{n})^2$
- Bend: $\rightarrow K_{3}|\mathbf{n}\wedge\nabla\times\mathbf{n}|^{2}$
- Saddle Splay (Null Lagrangian): $(K_{2} + K_{4})[tr(\nabla\mathbf{n})^{2} - (\nabla\cdot\mathbf{n})^2]$

On the other hand, the integral of the last term, i.e., the integral of the saddle splay

$$
(K_{2} + K_{4})\int_{\Omega}(K_{2} + K_{4})[tr(\nabla\mathbf{n})^{2} - (\nabla\cdot\mathbf{n})^2]d\mathbf{x}
$$

depends only on the values of the director $\mathbf{n}$ on the boundary $\partial \Omega$. Therefore, if the values of the director are given know on the boundary, via boundary conditions (homeotropic or planar), this term can be ignored.
