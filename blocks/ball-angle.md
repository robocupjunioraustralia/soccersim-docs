---
layout: page
title: Ball distance
parent: Blocks
nav_order: 2
permalink: blocks/ball-distance/
---

# Using the ball distance block

The **'ball distance'** block (Sensors) is used to get a measurement of distance between the centre of the robot, and the centre of the ball, in pixels. You can use the rulers on the right and bottom to gauge how far the robot is from the ball.

## Move until a distance

Let's write a program that will go towards the ball, until it is less than 100 pixels from the ball. To do this:

* We need an **'if'** block (Control) - because the robot needs to make a decision.
* We also need a **'comparison'** block (Operators) - because we need to check that the ball distance is greater than 100.
* *If* the robot is far away, *then* the robot should move forwards.
* *Otherwise*, the robot should stop.

Let's start with the if. Here, we drag the if and comparison, and we want the condition to be that the **ball distance is greater than 100**.

<img src="/soccersim/docs/assets/blocks/ball_distance_if.svg"/>

Now we just need to add the motor movement. The robot should move forward in the first case, and stop moving in the second case.

<img src="/soccersim/docs/assets/blocks/ball_distance.svg"/>
