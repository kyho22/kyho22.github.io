---
layout: project
type: project
image: images/micromouse.jpg
title: Shaka Scheme Project
permalink: projects/micromouse
# All dates must be YYYY-MM-DD format!
date: 2016-01-20
labels:
  - Scheme Interpreter
  - C++
summary: An R7R Scheme Interpreter written in C++.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/micromouse-robot.png">
  <img class="ui image" src="../images/micromouse-robot-2.jpg">
  <img class="ui image" src="../images/micromouse.jpg">
  <img class="ui image" src="../images/micromouse-circuit.png">
</div>

The Shaka Scheme project is a scheme interpreter written in C++. It is broken up into two teams, Parsing-IO and Core Systems. The Parsing-IO team was responsible for the the front-end systems which includes organizing user input into a structure for procedure calls and evaluators. The Core Systems team was responsible for the vital systems, data structures, and algorithms for things that Scheme relies on that cannot be coded into Scheme itself such as conditional statements, functions, environments, and memory management.            
For this project, I was the lead programmer who was responsible for programming the various capabilities of the mouse.  I started by programming the basics, such as sensor polling and motor actuation using interrupts.  From there, I then programmed the basic PD controls for the motors of the mouse.  The PD control the drive so that the mouse would stay centered while traversing the maze and keep the mouse driving straight.  I also programmed basic algorithms used to solve the maze such as a right wall hugger and a left wall hugger algorithm.  From there I worked on a flood-fill algorithm to help the mouse track where it is in the maze, and to map the route it takes.  We finished with the fastest mouse who finished the maze within our college.

For this project, I was part of the core-systems team which handles the core evaluations of Shaka Scheme. I contributed to the team by writing some of the native procedure calls, and the string and symbol datatypes of Shake Scheme. Along with a partner, we programmed some of the native procedure calls like the conditional statements "if," and evaluation calls such as "greater than" and "less than." In addition, I also wrote two of the datatypes, "symbol" and "string."        

Here is some code that illustrates how we read values from the line sensors:

```js
byte ADCRead(byte ch)
{
    word value;
    ADC1SC1 = ch;
    while (ADC1SC1_COCO != 1)
    {   // wait until ADC conversion is completed   
    }
    return ADC1RL;  // lower 8-bit value out of 10-bit data from the ADC
}
```

You can learn more at the [UH Micromouse Website](http://www-ee.eng.hawaii.edu/~mmouse/about.html).



