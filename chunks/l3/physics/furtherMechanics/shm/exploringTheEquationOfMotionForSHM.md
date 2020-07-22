---
title: 'exploringTheEquationOfMotionForSHM'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

To recap, the *general* equation of motion for SHM is,

$$
	x = A\cos(\omega t + \phi)
$$

Where $\omega$ is the angular freqency of the motion, and $A$ and $\phi$ are arbitrary constants.

# Boundary Conditions

Notice that in the equation above there are three constants: $A$, $\phi$ and $\omega$. Now, the third of these constants is fixed by the equation of motion of the system. It's value is determined by the shape of the potential well in which the particle is oscillating.

The first two of these constants, however, are arbitrary constants that arose due to our solving the differential equation of motion - they can, in theory, take any values and still satisfy the equation of motion. Now of course, in reality, for a given motion they must take *some* specific values - so which values do they take? Well, their values are determined by the initial (boundary) conditions of the motion - They depend on where we set the oscillator in motion, and what initial velocity we give it (the conditions at the *boundary* of the motion).

# Plotting the motion

Let's plot the equation above, for $0\le x\le \frac{4\pi}{\omega}$ and $\phi = 0$

[DIAGRAM]

Firstly, we see that the motion repeats itself after $t = \frac{2\pi}{\omega}$, suggesting that the period of the motion is,

$$*
	T = \frac{2\pi}{\omega}
$$

We should have guessed this from circular motion (in fact the maths here is going to look awfully similar to that of circular motion).

Secondly, we see that the **amplitude** of the motion (maximum distance from equilibrium) is $A$.

# The Phase Factor

The final constant that we need to be aware of is $\phi$. This is another boundary condition (along with $A$), and as a result can be made to have any value based on how we set the oscillator in motion. Mathematically, changing $\phi$ simply has the effect of shifting our graph backwards and forwards - it changes which part of the cycle the oscillator starts out in (whether it is at the maximum position, the equilibrium position, or somewhere in the middle). It does not change the amplitude of the motion (which only depends on $A$) or the angular frequency (which is fixed by the shape of the potential well).
