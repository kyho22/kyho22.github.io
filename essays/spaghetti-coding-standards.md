---
layout: essay
type: essay
title: Spaghetti, Some People Like It, All Programmers Hate It.
# All dates must be YYYY-MM-DD format!
date: 2018-02-08
labels:
  - Software Engineering
  - Coding Standards
  - ESLint
  - IntelliJ IDEA
---

## The foundation
I believe that coding standards are important. I feel like they help you write better and cleaner code which makes it much easier to read. Coding standards help establish a common ground for everyone so that there is some control over what is and is not correct. It acts as a guide that people follow to maintain order in programming.

## Why so strict?
Although I agree that there should be a set of coding standards, I do not believe that they should be extremely strict. To elaborate, I feel like programmers should have the freedom use any type of style they wish, (ie. camel case, underscore case, Allman style, K&R style, etc), but still have a common ground of what are good programming practices and what aren't. To analogize, think about people writing in English, anyone can write in any style they want, comic-sans, script, etc., however everyone must follow the same spelling and grammatical rules established in the English standard. In other words, I believe that you can use any coding style you're comfortable with, however your code better not look like something that just came fresh out of The Old Spaghetti Factory's kitchen.     

## My first experience with coding inspectors
Over the past week, I have been using ESLint while I was programming on IntelliJ. At first, I thought it was very annoying because of all the minor spacing errors and when to use "const" and "let," but after a few days, I got accustomed to it. What I disliked about ESLint was how it sometimes doesn't want you to return your results in variables. For example, when I have a function that will sum up all values in a list using the function "reduce" in the Underscore library, ESLint will give me a warning saying that be putting the result of the "reduce" function in a variable is unnecessary. Although I do agree that I can just return the result directly from the function, sometimes those function calls gets really long and can start nesting more functions or call really long object properties. In cases like that, I want to save the results in a variable so that it's easier to interpret what kind of value it is.

## Wrapping it up  
Overall, I believe that ESLint and IntelliJ are really useful tools for programming because they can be used to clean up messy code. On top of that, I think that coding standards are important in programming because it sets up a foundation on what is good and what is bad. I just don't agree with coding standards that are really strict about minute things such as indents and where to place curly brackets.         
