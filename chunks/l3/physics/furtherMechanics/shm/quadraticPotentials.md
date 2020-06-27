---
title: 'quadraticPotentials'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

Simple harmonic motion occurs in any system which has a quadratic potential. What this means is that the potential energy of the object engaged in the motion varies with the square of the position of the particle from it's equilibrium position.

[DIAGRAM]

In 1-dimension the force acting on a particle (which is proportional to the particle's acceleration) is related to the gradient of it's potential function by,

$$
	a\proptoF = -\frac{\dee V}{\dee x}
$$

Intuitively, this means that particle's acceleration is always in the direction of decreasing potential and is greater for steeper potentials. A way to visualise this (and this holds for all physics systems) is imagine taking the potential function of a particle, constructing a slide in the shape on the potential function and rolling a ball down it. Intuitively we know that the ball is going to accelerate down the most steeply sloped areas faster - this is exactly what all objects do with respect to their potential functions.

So, if $V\propto x^2$, then by taking the derivate (feel free to just take my word that this is indeed the correct derivative),

$$
	F\propto -2x
$$

We can drop the factor of 2 since we are just interested in proportionality, and replace $F$ with $a$ since they are proportional to each other. Finally,

$$*
	a\propto -x
$$

This is the defining property of SHM that is given in many text books. While they're not *wrong*, they do miss a step, which is actually that SHM is to do with quadratic potential wells. This fact will help us to explain approximate SHM (such as the pendulum) later on in the course.
