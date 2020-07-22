---
title: 'mathematicalDefinitionOfAField'
author: 'Ben Rogers-Newsome'
level: 3
type: 'core'
---

For the meantime we are going to just think of fields as mathematical tools used to describe forces, and not worry about what they *actually* are (I mean, this is what they *actually* are, really, but of that fact I will try to convince you at a later point).

Let's think of a field as being an *assignment* of some measurable mathematical object (a number or a vector in all the cases we will discuss) to each point in space. As you move through space, the measured value of this object will generally change. A classic example of a scalar field (scalar meaning we assign a number to each point of space) is that which describes the temperature of a room - near the radiator the temperature will be high, and as we move towards the open window the measured value of the temperature will drop. Importantly, there is a number that we *assign* to each point of the room, to describe the temperature at that point in the room.

Mathematically we can simply describe this assignment as a function $\Phi: \tor x\rightarrow T$. What this notation means is that our function, labelled $\Phi$, is taking *in* a vector representing some position, labelled $\tor x$, and returning the temperature at that position, labelled $T$. Mathematically speaking, the field *is* the function $\Phi$.

In the case of fields that represent forces we have a slightly different situation. Force's are represented by vectors, and as such our field must return a vector (not a vector equal to a force, but a vector that we will use to calculate the force later). Our field can be written $\Psi: \tor x\rightarrow \tor v$ where $\tor v$ is a vector. We say that the field is **vector valued** since the the field is assinging each point in space with a vector.
