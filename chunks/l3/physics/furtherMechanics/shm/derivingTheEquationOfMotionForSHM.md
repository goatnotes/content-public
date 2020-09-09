---
title: 'derivingTheEquationOfMotionForSHM'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

Starting from our defining equation,

$$
	a = -\omega^2x
$$

We can derive the eqautions of motion for simple harmonic motion.

The first step is to relace the $a$ with $\frac{\dee^2 x}{\dee t^2}$ (the second time derivative of the particle's position). This yeilds an ordinary second order differential equation, which can be solved by standard methods.

$$
	\frac{\dee^2 x}{\dee t^2} = -\omega^2 x
$$

There is a method that they teach at A-Level for solving second order differential equations, however, it is basically based upon making an educated guess for the solution that works for all ordinary second order differential equations (with constant coefficients). Proving *why* the solution works is actually very hard, and as a result making guesses to solutions and substituting into the equation to check them, is actually a widely accepeted form of solving second order differential equations. And so, in that spirit, I am going to *guess* (plot twist, I know it's going to work) a solution and show you that it works by substituting into the equation above.

So, my guess is going to be $x = A\cos(\omega t + \phi)$, where $A$ and $\phi$ are arbitrary constants. Evaluating the derivatives,

$$
	\frac{\dee x}{\dee t} = -\omega\times A\sin(\omega t + \phi)
$$

$$
	\frac{\dee^2 \x}{\dee t^2} = -\omega^2\times A\cos(\omega t + \phi) = -\omega^2 x
$$

And so, it works:

$$
	x = A\cos(\omega t + \phi)
$$

Is the general equation of motion for SHM.
