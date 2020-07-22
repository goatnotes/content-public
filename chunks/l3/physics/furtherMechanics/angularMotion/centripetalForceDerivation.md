---
title: 'derivingTheCentripetalForce'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

We can derive the centripetal force in a somewhat opposite way to how we would derive most physical formulae. Often we derive equations of motion by analysis of the forces that act on the body, drawing a picture of how the body will move based on this analysis.

However, in the case of circular motion we already know (by definition) what the motion looks like - it's a circle. All we have to do in order to derive the equation for centripetal acceleration is find the equation for a circle, and differentiate it twice.

We will work in cartesian parametric coordinates for this, since linear acceleration is always calculated in terms of cartesian coordinates.

DIAGRAM

We wish to express both the $x$ and $y$ coordinates of points on the circle in terms of the same parameter $t$. We can do this by spotting that every point on the circle is at a distance $r$ from the origin, at some angle $\theta$. So find the $x$ and $y$ coordinates of this point we simply resolve into $x$ and $y$ components.

$$
	x = r\cos\theta\qquad y = r\sin\theta
$$

We also know that for uniform circular motion, $\theta = \omega t$. And so, our equations of motion, for uniform circular motion are,

$$
	x = r\cos\omega t\qquad y = r\sin\omega t
$$

To recap, these are two independent equations, both in terms of time, for the cartesian coordinates of a body moving in a circle at uniform angular velocity. We can find the $x$ and $y$ components of linear acceleration simply by taking the second time derivatives of these expressions, and then we can find the direction and mangitude of the total acceleration from the two components.

So, the two components of acceleration come out as,

$$
	a_x = \ddot{x} = -r\omega^2\cos\omega t
$$
$$
	a_y = \ddot{y} = -r\omega^2\sin\omega t
$$

Interestingly, each of the particle's coordinates, independently, obey SHM. That is, they obey the relation,

$$
	\ddot{x} = -\omega^2 x\qquad \ddot{y} = -\omega^2 y
$$

Where the angular velocity of the particle equates to the angular frequency of the SHM it's individual coordinates corresponds to. This fact shows the very close relationship between SMH and circular motion.

To find the direction of the resultant acceleration we can consider forming the vector out of the components of the position and acceleration respectively.

DIAGRAM

Since the acceleration components are equal to the position components multiplied by the same factor, the acceleration vector points in exactly the opposite direction to the position vector. Since the position vector points radially from the center of the circle, to the position of the particle, we have just proven that the centripetal acceleration acts radially **towards** the center of the circle.

To find the magnitude of the total acceleration we just use Pythagoras' law.

$$
	a = \sqrt{a_x^2 + a_y^2} = \sqrt{r^2\omega^4\cos^2(\omega t) + r^2\omega^4\sin^2(\omega t)}
$$

And using the identity $\sin^2 + \cos^2 = 1$ (suppressing the arguments of sine and cos),

$$
	a = \sqrt{r^2\omega^4} = r\omega^2
$$

We can use the relation $\omega = \frac{v}{r}$ to obtain to other form of the expression. Finally.

$$*
	a = r\omega^2 = \frac{v^2}{r}
$$

We obtain the expression for force by multiplying by the mass, $m$, of the particle.
