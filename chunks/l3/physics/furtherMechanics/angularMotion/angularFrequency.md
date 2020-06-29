---
title: 'angularFrequency'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

The angular velocity of a particle, $\omega$, is also known as the *angular frequency*, and here we will explore why that is the case.

Suppose, as usual, that we have a particle moving in a circle. It has a constant angular velocity $\omega$, and naturally after some time, which we will label $T$, it will return to it's original position (by virtue of the fact that the particle is moving in a circle).

![Circular motion](/img/physics/furtherMechanics/angularMotion/circularMotion.png)

The question is: What is the time $T$ in terms of the angular velocity $\omega$?

The answer is relatively straight forwards. $\omega$ is, by definition, the angle moved by the particle per unit time:

$$
	\omega = \frac{\Delta \theta}{\Delta t}
$$

For one full rotation around the circle $\Delta\theta = 2\pi$, and by definition $\Delta t = T$. Therefore,

$$*
	T = \frac{2\pi}{\omega}
$$

Where $T$ is the *period* of the circular motion.

Now, just as in the study of waves, if the period is the time taken for one full cycle we can define the frequency,

$$
	f = \frac{1}{T}
$$

as the number of complete cycles per second.

In this case,

$$*
	\omega = 2\pi f
$$

And so we see that the angular velocity of the motion only differes from the frequency of the motion by a factor of $2\pi$ - that is, they are directly proportional to each other. In this sense, angular velocity is just as equaly a measure of rate of change of angle, as it is a measure of the frequency of the oscillation, and hence the term angular frequency.
