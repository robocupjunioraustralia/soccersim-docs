---
layout: page
title: Ball angle
parent: Blocks
nav_order: 3
permalink: blocks/ball-angle/
---

# Using the ball angle block

The **'ball angle'** block (Sensors) is used to get a measurement of angle, between -180 and +180. If the ball is on the left of the robot, the number is negative. If the ball is on the right, the ball is positive.

## Rotate to face the ball

Let's write a program that will rotate the robot to face the ball. 

* We need an **'if'** block (Control) - because the robot needs to make a decision.
* We also need a **'comparison'** block (Operators) - because we need to check that the ball distance is greater than 100.

We have three conditions:
* *If* the ball is to the left (ball angle < -20), *then* the robot should rotate left.
* *Otherwise, if* the ball is to the right (ball angle > 20), *then* the robot should rotate right.
* *Otherwise*, the robot should stop.

We're using -20 and 20 degrees because the robot can't stop instantly.

Let's start with the if. Here, we drag the if and comparison blocks, and we can also press the + to get the 'else if' section.

<img src="/soccersim/docs/assets/blocks/ball_angle_if.svg"/>

Now we just need to add the motor movement. 
* Rotate left means the left wheel needs to go backwards (negative) and the right wheel goes forwards (positive).
* The opposite for rotating right.

<img src="/soccersim/docs/assets/blocks/ball_angle.svg"/>
