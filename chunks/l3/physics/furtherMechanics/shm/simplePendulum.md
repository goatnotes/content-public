---
title: 'derivingTheSimplePendulum'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

# Setup

The simple pendulum is set up as follows:

[DIAGRAM]

The *simple* pendulum is actually quite a *complex* system if you want to do the analysis properly. We do want to do the analysis properly, and hence that is what we are going to do. You can't actually *solve* the simple pendulum analytically (mathematically we cannot solve it's equation of motion into closed form), however, we can make approximations which allow us to at least characterise it's motion qualitatively, and approximately quantitatively.

## Initial approximations

We are going to make some approximations straight off the bat. The first of these is that the string of the pendulum has no mass. This is not actually as big an approximation as one might initially expect. Because of the symmetry of the system, giving the string mass simply has the effect of shifting the center of mass of the system up the string a little bit. Therefore, a pendulum system in which the string *does* have mass, can be modelled exactly by a pendulum system in which the string *doesn't* have mass, but is just a little shorter.

[DIAGRAM]

Therefore, we can make this approximation to the system without any real loss in generality in the maths.

# The coordinates

We need a way to paramaterise the position of the pendulum bob.

We are not going to work in cartesian coordinates for this derivation (since they make essentially no sense in this situation). Instead we are going to use plane-polar coordinates, characterising the pendulum's position by it's distance from the point of suspension (which we will call the *radius*, $r$) and the angle that this radius makes from the vertical (which will be labelled $\theta$).

[DIAGRAM]

In most cases the string of the pendulum will *be* the radius (and so $r=l$ and $\theta$ will be the angle the string makes with the vertical). However, I have explicitly defined the pendulum bob's coordinates without reference to the string because, as will be discussed later, there are cases when the string of the pendulum can do weird things that mean it is not a reliable way to define the bob's position.

# Deriving the Equation of Motion

There are two forces that will act on the pendulum bob,

[DIAGRAM]

Gravity which always acts vertically downwards (this is actually an approximation that we make), and the tension in the string which always acts radially. Some other quantities have been labelled on the diagram above, for later reference.

There will be two equations of motion for the pendulum system: One for $r$ (the radial motion) and one for $\theta$ (the tangential motion). A naiive assessment of the pendulum leads one to beleive that there is no radial motion (that is the radius of the motion is constant and equal to the length fo the string), however, this is indeed a naiive assessment, and as we will see it should not be taken as a given that a pendulum will move in a perfectly circular arc around the point of suspension.

We will derive the radial and tangential motion seperately here, and bring them together at the end.

## Radial Forces

The resultant force in the radial direction is given by the sum of the tension force and the component of gravity resolved in the radial direction. The radial component of gravity is given by $mg\cos\theta$ and hence the resultant force in the radial direction is given by,

$$
	F_r = mg\cos\theta - T
$$

The convention taken above is that the positive $r$ direction is directed away from the point of suspension.

Now, importantly, we cannot apply Newton's second law here. I.e. $F_r \ne m\ddot{r}$. This is because we are not in cartesian coordinates, the $r$ direction is constantly changing. However, what we can do is notice that the pendulum bob is moving in a circular motion, and hence the resultant force in the radial direction must precisely equal the centripetal force required to keep an object moving in a circle. That is,

$$
	mg\cos\theta - T = -m\dot{\theta}^2r
$$

Where $\dot{\theta}$ is the angular velocity of the bob. There are two important observations to make about this equation. Firstly, the term $mg\cos\theta$ (the radial component of gravity) will change as the bob moves round the arc (i.e. as $\theta$ changes). Similarly, from inuition alone we know that $\dot{\theta}$ will not be constant around the arc, since the bob is going to be swinging backwards and forwards. Hence, to make this equality hold the tension, $T$, in the string must change throughout the pendulum's motion. This idea will be discussed more later, however, it is just something worth bearing in mind throughout the rest of the derivation.

The second point is that, although this is the *radial* equation, it contains both radial *and* angular terms. In this respect we say that the two equations of motion for the pendulum are **coupled** - that is, they each contain both coordinates. The fact that this equation deals with the radial forces doesn't really relate at all to how we will ultimately derive the radial equation of motion - we will have to use both of the derived equations in order to find either of the final equations of motion. We say that the simple pendulum system is described by a *system* of *coupled differential equations*. Coupled systems of equations can often be seperated into seperate, uncoupled equations, only involving a single variable, by employing a change of coordinates, however, it is not going to be beneficial for us to do that here.

## Tangential Motion

In the tangential direction there is only one force acting on the pendulum bob: The radial component of gravity, given by $-mg\sin\theta$. The minus sign indicates that the tangential force acts to pull the pendulum bob to equilbrium (i.e. in the opposite direction as that of increasing $\theta$).

In order to form the differential equation in the tangential direction we are first going to introduce a new variable: The arc length.

[DIAGRAM]

The arc length, $x$, is the distance along the arc through which the pendulum has moved. It is related to the angle $theta$ by the equation,

$$
	x = r\theta
$$

The reason for doing this is that we can apply Newton's second law to the variable $x$. Loosely speaking this can be done because we can *bend* the arc of the motion into a straight line and expect it to follow the same equation of motion. The fact that the variable $x$ is a distance around an arc doesntt matter; it is still a linear *displacement* (just like cartesian coordinates) and hence obeys Newton's second law.

Therefore, using this logic,

$$
	F_t = -mg\sin\theta = m\ddot x
$$

$$
	\ddot x = -g\sin\theta
$$

Since $x = r\theta$, we need to apply the product rule of differentiation to obtain $\ddot x$.

$$
	\dot x = \dot r \theta + r\dot\theta
$$

$$
	\ddot x = \ddot r \theta + \dot r\dot \theta + \dot r\dot theta + r\ddot\theta
$$

$$
	\ddot x = \ddot r \theta + 2\dot r\dot \theta + r\ddot\theta
$$

Which gives us the differential equation,

$$
	\ddot r \theta + 2\dot r\dot \theta + r\ddot\theta = -g\sin\theta
$$

## Summary of Equations

Our two differential equations that we would like to solve are,

$$
	mg\cos\theta - T = -m\dot{\theta}^2r
$$

$$
	\ddot r \theta + 2\dot r\dot \theta + r\ddot\theta = -g\sin\theta
$$

Where we have made the following approximations:
- The string of the pendulum has no mass (and we have already discussed how this isn't really an approximation at all).
- The pendulum only moves in a flat plane - i.e. there is no motion in or out of the page (a pendulum of this form is called a conical pendulum, and has a seperate analysis).
- Gravity acts vertically downwards.
- There is no air resistance.

Now, at this point there is a bit of an anti-climax, in that we don't know how to solve these equations. Mathematically speaking, we would say that there are no **closed form solutions** to these equations, meaning that we don't know how to find equations of the the form $r = f(t)$ and $\theta = g(t)$ where $f(t)$ and $g(t)$ are some functions of time.

One thing we can do though, is explore what these equations *imply*, and find closed form solutions to approximate forms of these solutions.
