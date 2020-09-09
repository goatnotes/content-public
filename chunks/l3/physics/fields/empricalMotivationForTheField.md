---
title: 'empiricalMotivationForTheField'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

Let's suppose you have a *gun*, able to fire different types of particles (such devices exist, although they have less in common with guns than with short half-life radioactive samples), and you can change what particles this gun is firing (by changing the sample for example). Let's also suppose that you have some kind of chamber into which you can fire this gun, and observe the paths of particles as they move through space (such chambers also exist). Finally, just to simplify the following discussion, let's suppose you already know the mass of all the particles you are firing from this gun (this is also possible).

Now you run this experiment a few times, with different particles from this gun. With some particles you observe they just come straight out the gun and move in a straight line while with others you observe a path that arcs, and changes direction moving through the chamber, with varying severity and direction depending on the particle. From this arching of the particle's path you are able to infer that there must be some force acting on the particle (if the particle's velocity changes it is necessarily accelerating, hence a force must be acting on it). You can calculate this force numerically by calculating it's acceleration from it's path and using the (known) mass of the particles to calculate the force. What you find is that both the direction and magnitude of this force changes along the particle's path - It is not subject to a constant force in space.

To recap:
	- There is some unknown force acting on the particles
	- The magnitude and direction of this force can be different for different particles, within the same region of space
	- The magnitude and direction of this force can be different for the same particle in different regions of space

If we wanted to model this phenomena mathematically what would we need to take account of?

Well, there are two main parameters we need to keep track of. There is clearly some property of the particles that is affecting how they experience the force (which we will call the coupling constant for reasons that will become clear) and some other property which changes in space to account for the changing force along the particle's track.

This second factor is where fields come in. In classical physics, fields allow us to describe non-contact forces that continuously vary in space, and how they act on particles.
