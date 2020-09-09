---
title: 'theVelocityEquation'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

We can obtain an equation for the velocity of the motion by differentiating the general equation of motion.

$$*
	v(t) = \frac{\dee}{\dee t}x(t) = -A\omega\sin(\omega t + \phi)
$$

The key points here are that the maximum absolute value of the velocity is given by $A\omega$ and that if we plot this on the same graph as the position function we see that the velocity lags behind the position function by $\frac{\pi}{2}$ radians.

# V in terms of X

We can also obtain an expression for the velocity of the particle in terms of it's position. This is quite an arbitrary thing to do (in my opinion) but we are going to do it anyway. The key insight we need to make to obtain such an expression is that,

$$
	\sin^2(\omega t + \phi) + \cos^2(\omega t + \phi) = 1
$$

This is just the standard trigonometric identity (since it doesn't matter what the inner bit is, as long as they are the same). We then spot,

$$
	\sin^2(\omega t + \phi) = \frac{v^2}{A^2\omega^2}
$$
$$
	\cos^2(\omega t + \phi) = \frac{x^2}{A^2}
$$

And so,

$$
	\frac{v^2}{A^2\omega^2} + \frac{x^2}{A^2} = 1
$$

Re-arranging,

$$*
	v(x) = \pm\omega\sqrt{A^2 - x^2}
$$

We can plot this, and what we see is,

[DIAGRAM]

The velocity peaks at the center of the motion, and is zero at the edges. The reason for their being positive and negative *branches* of the graph is that for every position in the motion the particle can either be moving left (for the first half of the cycle, let's say) or right (which it would do on the return *trip*).
