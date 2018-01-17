---
layout: project
type: project
image: images/Scheme.png
title: Shaka Scheme Project
permalink:
# All dates must be YYYY-MM-DD format!
date: 2016-01-20
labels:
  - Scheme
  - C++
  - MinGW
summary: A clean implementation of R7RS-small Scheme written in C++.
---

The UHM Curriculum Database is a database system I designed and built using FileMaker Pro 16 as a part of my job for the College of Natural Sciences. It is used to manage and archive all curriculum changes for all the departments under the college since 1986. 

The Shaka Scheme project is a scheme interpreter written in C++ built using the MinGW environment. Our goal was do a clean implementation of R7RS-small Scheme. The project was broken up into two teams, Parsing-IO and Core Systems. The Parsing-IO team was responsible for the the front-end systems which includes organizing user input into a structure for procedure calls and evaluators. The Core Systems team was responsible for the vital systems, data structures, and algorithms for things that Scheme relies on that cannot be coded into Scheme itself such as conditional statements, functions, environments, and memory management.       

For this project, I was part of the core-systems team which handles the core evaluations of Shaka Scheme. I contributed to the team by writing some of the native procedure calls, and the string and symbol datatypes of Shake Scheme. Along with a partner, we programmed some of the native procedure calls like the conditional statements "if," and evaluation calls such as "greater than" and "less than." In addition, I also wrote two of the datatypes, "symbol" and "string."        

Here is some code that illustrates how we implemented the symbol datatype:

,,,

Symbol(const std::string& v) :
      value(v) {}

  friend void swap (shaka::Symbol& lhs, shaka::Symbol& rhs) {
    using std::swap;

    swap(lhs.value, rhs.value);
  }

  shaka::Symbol operator= (shaka::Symbol other) {
    shaka::Symbol temp(other);
    swap(*this, other);

    return *this;
  }
  
,,,

Source: <a href="https://github.com/uhmanoa-transpiler-project/shaka-scheme"><i class="large github icon"></i>uhmanoa-transpiler-project/shaka-scheme</a>

