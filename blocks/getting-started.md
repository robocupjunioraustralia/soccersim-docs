---
layout: page
title: Getting started
parent: Blocks
nav_order: 1
permalink: blocks/getting-started/
---

# Getting started with Blocks
Let's code your first simulation robot in SoccerSim! First, open up [the Blocks editor](/soccersim/blocks). On the left, you have a Scratch-like drag and drop area, where you can click and drag on blocks and place them into the workspace.

On the right, you have the simulation.

----

## Your first SoccerSim program
You can write Blocks programs for each of the blue robots, and use different blocks to loop forever, check the ball angle, or move the motors.

The most common and useful blocks are:

* **Motors**: Here you'll find ways to set the motor speed!
* **Control**: You'll find a 'repeat forever' block to keep your program running, 'if' blocks for testing.
* **Operators**: To make comparisons with 'if' blocks, you will find 'equals', 'greater than' and most other blocks here.
* **Sensors**: for your ball direction (in degrees), ball distance (in pixels) and robot heading (in degrees)

The best way to start is to try get the robot moving! 

First, place a **'repeat forever'** block (Control) into the workspace. This means that our robot is always going to repeatedly move and react to the ball. We also should set the starting position for the robot, meaning we should use a **'set starting position'** block (Events) at the very beginning of our program.

<img src="/soccersim/docs/assets/blocks/starting.svg"/>

## Moving forward

Let's make our robot move forward. Add two **'set motor speed'** blocks (Motors) - one for motor A (left) and motor B (right). Change the speeds to 50.

<img src="/soccersim/docs/assets/blocks/forever_forward.svg"/>

Then hit the green Run all button! You should see the robot move forward. You can click and drag on the robot to move it back. To rotate the robot, click and drag on the robot's wheels.

To stop the robot, click the red 'Stop all' button. 

## Rotating

If we want to rotate on the spot, we can easily set one of the motors to be a negative value. The motor speeds can be between -100 and 100.

If we set the left wheel to -50, and the right wheel to 50, then it will rotate anti-clockwise.

<img src="/soccersim/docs/assets/blocks/anticlockwise.svg"/>

