---
title: 'angularVelocity'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

If an object is moving in a circle, it makes sense to think about the angle, $\theta$, the object moves through, rather than it's linear coordinates.

[DIAGRAM]

Let's say that the object is moving in a circule of radius $r$. If the object moves through an angle $\Delta\theta$ then we know that the length of the arc is moves through is $\Delta x = r\Delta\theta$. If the object does this in a time $\Delta t$, then we know that the linear velocity of the particle is given by,

$$
 v = \frac{\Delta x}{\Delta t}
$$

Provided the velocity is constant. This gives us,

$$
 v = r\frac{\Delta\theta}{\Delta t}
$$

Now, that term on the right hand side is simply the angle the object moves through per unit time, or in other words, the *angular velocity*, $\omega$, and in fact the expression above can be taken as a definition for angular velocity.

$$
 \omega\equiv\frac{\Delta \theta}{\Delta t} = \frac{v}{r}
$$

Where $v$ is the linear velocity and $r$ is the radius of the circle.
