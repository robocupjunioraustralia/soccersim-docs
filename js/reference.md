---
layout: page
title: Reference
parent: JavaScript
nav_order: 999
permalink: js/reference/
---

# Reference
This is a raw reference guide for functions available in the SoccerSim.

## Table of contents
1. Table of contents
{:toc}

## Robot
### setMotorSpeed

<div class="code-example" markdown="1">
`setMotorSpeed(motor, speed)`
Sets the motor speed, for a particular motor.
* `motor` (String) motor name, e.g. `'motorA'`
* `speed` (Number) number between -100 and 100, a positive value drives the motor forwards.
</div>

```javascript
// Spin the robot around
setMotorSpeed('motorA', 30);
setMotorSpeed('motorB', -30);
```

### stopMotor

<div class="code-example" markdown="1">
`stopMotor(motor)`
Stops a particular motor.
* `motor` (String) motor name, e.g. `'motorA'`
</div>

```javascript
// Stops both motors
stopMotor('motorA');
stopMotor('motorB');
```

### getMotorSpeed

<div class="code-example" markdown="1">
`getMotorSpeed(motor)`
Returns the current speed of the motor.
* `motor` (String) motor name, e.g. `'motorA'`
</div>

```javascript
if (getMotorSpeed('motorA') > 10) {
	// Speed is over 10
}
```

----

## Sensors
### getBallAngle

<div class="code-example" markdown="1">
`getBallAngle()`
Returns the current ball angle `-180 <= angle < 180`, relative to robot. If the ball is directly in front of the robot, the value is `0`. Negative if on the left, positive on the right. The angle is calculated from the centre of the robot to the centre of the ball.
</div>

```javascript
if (getBallAngle() > 0) {
	// Ball is on the right relative to the robot
}
```

### getBallDistance

<div class="code-example" markdown="1">
`getBallDistance()`
Returns the current ball distance relative to the robot, in pixels. The distance is calculated from the centre of the robot to the centre of the ball.
</div>

```javascript
if (getBallDistance() < 60) {
	// Ball is really close to the robot
}
```

### getCompassHeading

<div class="code-example" markdown="1">
`getCompassHeading()`
Returns the current robot compass heading `-180 <= angle < 180`, relative to the robot. If the robot is facing directly forwards, the value is `0`. Negative if facing the left, positive on the right.
</div>

```javascript
if (getCompassHeading() > 20) {
	// Robot is facing to the right
}
```

### setInitialPosition

<div class="code-example" markdown="1">
`setInitialPosition(position)`
Sets the initial position. Run this at or near the start of your program. 
* `position` (String) position string. One of: `far-left`, `left`, `centre`, `right`, `far-right`

The position is in increments of 50 pixels from the centre. E.g. `far-left` is 100 pixels from the centre.
</div>

```javascript
// Places the robot on the far left.
setInitialPosition('far-left');
```