---
layout: page
title: Getting started
parent: JavaScript
nav_order: 1
permalink: js/getting-started/
---

# Getting started with JavaScript
Let's code your first simulation robot in SoccerSim! First, open up [the JavaScript editor](/soccersim/javascript). On the left, you have an editor, where you can program JavaScript code. On the right, you have the simulation.

JavaScript is pretty similar to C or Python - it just has a slightly different syntax. The following links may be helpful:

* [Codecademy: Learn JavaScript](https://www.codecademy.com/learn/introduction-to-javascript) - A very beginner friendly way where students can solve problems and learn JS
* [JavaScript Fundamentals](https://javascript.info/first-steps) - a thorough introductory guide to programming in JavaScript on the browser
* [MDN: JavaScripts basics crash course](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics#Language_basics_crash_course) - useful for students who have done some text programming before

----

## Your first SoccerSim program
The best way to start is to try get the robot moving! The following code will get your robot moving forward:

```js
while (1) {
    setMotorSpeed('motorA', 50);
    setMotorSpeed('motorB', 50);
}
````

Then hit the green Run all button! You should see the robot move forward. You can click and drag on the robot to move it back. To rotate the robot, click and drag on the robot's wheels.

To stop the robot, click the red 'Stop all' button. 

----

For all robot commands, see the [JavaScript reference guide](../reference/).