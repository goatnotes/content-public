---
title: 'generalisedCoordinates'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

Why do we use cartesian coordinates generally? Because they are convenient. Occasionally, when dealing with rotating bodies (or when looking at orbits) we use polar coordinates (an angle and a radius) - why do we do this? Again, it is because they are convenient for that situation.

The point I am trying to make is that there is nothing special about cartesian and polar coordinates, they are just two ways of describing a system which simplify the analysis in certain special situations. Generally speaking, in two dimensions, we need two numbers to fully locate a position within a system. In cartesian coordinates this is the distance along two perpendicular axes, and in polar coordinates it is the distance from the origin and the angle from the positive $x$ axis to the line connecting the point to the origin.

[DIAGRAM]

Another way to think of this fact is that in both cases our point is given by the intersection of two lines. In cartesian coordinates we construct a line parallel to the $y$ axis going through a particular value on the $x$ axis (this is the line associated with our $x$ coordinate), and we construct a similar line, but the other way around (this is the line associated with our $y$ coordinate). Our point is then specified by the intersection of these lines.

[DIAGRAM]

In the case of polar coordinates we have a stright half-line (meaning it terminates at the origin) inclined at an angle $\theta$ to the positive $x$ axis, and a curved line which is a circle of radius $r$. We see that, just as in the case of cartesian coordinates, we have a line associated with each coordinate (one is curved, but that is no matter), and the intersection of these lines specifices our point.

[DIAGRAM]

Hopefully this idea of a point being specified by the intersection of two lines is enough to convince you that we always need two numbers to describe a point in cartesian coordinates (in fact, we can't actually have more than two numbers as this would overdetermine our problem. Two non-parallel lines will always intersect in at least one place, whereas with three lines there is no guaruntee they will all intersect at the same point, and thus we cannot uniquely define a point in the plane based on their intersection). In three dimensions the general argument is the same, but our point is determined by the intersection of three planes (some, or all, of which may be curved). 3D cartesian coordinates uses three flat planes, each parallel to two of the coordinate axes.

Now, how does this relate to A-Level physics? Well, in A-Level physics (and beyond) you are taught linear classical mechancs ($F=ma$, $p=mv$, etc) and rotational mechanics ($\omega=\frac{v}{r}$, $F_c=m\omega^2 r$, etc). The first is based in linear coordinates: It defines distances as straight lines and momentum as a linear property of matter (in fact $p=mv$ is actually called linear momentum). In the second case we are dealing with polar coordinates. All the *physics* is the same, we just use different coordinates and hence are able to describe the system more easily when dealing with rotating or orbiting bodies. The equations that transform between the two ($\sqrt{x^2 + y^2}=r\theta$, $\omega = \frac{|v|}{r}$) are just transformation laws that allow you to move from one coordinate system into the other.

We could anlyse any system with whatever coordinate system we wanted. In many cases it would be difficult, and pointless, hence why we don't - but in principle we could. In fact, we are initially taught physics in term of linear coordinates, and we define rotational mechanics in terms of linear mechanics. However, linear mechancis is no more *fundamental* than rotational mechanics. Newton's second law can be written in term of rotational mechanics and it would have been just as correct (just less intuitive).

The natural question to ask now is: Is there a formulation of physics which doesn't reference a specific set of coordinates - that is, it is coordinate agnostic? The answer is yes. There is a branch of mechanics (which I won't go into the details of here) called Lagrangian mechanics. Lagrangian mechanics formulates the laws of mechanics in terms of generalized coordinates (that is, not worrying about what the specific coordinates represent).
