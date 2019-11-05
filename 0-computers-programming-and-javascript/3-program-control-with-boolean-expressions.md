# Program control and Boolean expressions

We've covered some of the most important concepts in the JavaScript language and programming in general, including what programs are and how they work, thinking like a programmer with algorithms and abstraction, and how to use data in your programs.

Now I'm going to give you some tools that will allow you to write more complex (and more useful) programs.

## Algorithm basics

Studying and understanding how algorithms work will empower you to compose powerful programs that are both efficient in how they work and comprehensible to other programmers. Remember from [the first chapter](./0-getting-started.md) that an algorithm is like a recipe that tells a computer how to perform a computation.

An algorithm has 3 basic parts:

1. A list of instructions
2. A way to decide which instructions to execute, and when to execute them
3. A way to know when to stop[^1]

Declarative and imperative programs look at algorithm implementation differently, and program control is a major area of difference. This chapter will show you examples of both.

## Branching algorithms

All the examples so far, including the programs you've written, have been valid, complete JavaScript programs. They haven't been very _interesting_, though. Reading through a list of instructions isn't exactly the most riveting thing.[^2]

The programs we've seen so far have all been **straight-line programs.**

Straight-line programs take a list of instructions, execute one after the other in the order in which they are written, and then stop when they run out of instructions.

**Branching** programs are more interesting. They use some kind of conditional expression to decide which of two or more options to take when faced with a choice. We're going to look at conditional execution in both declarative and imperative styles because it's important for you to be familiar with both.

But first you need to thoroughly understand Boolean logic, which is the means by which a program chooses its path.

## What is Boolean logic?

### Boolean expressions

### Booleans and type coercion

## Control logic: declarative style

### Short-circuit evaluation

## Control flow: imperative style

### Conditional statements

## Control flow vs. logical flow

[^1]: See more about the 3 steps and how to define an algorithm in [Dr. Ana Bell's lecture for MIT 6.0001](https://youtu.be/nykOeWgQcHM?t=869), Introduction to Computer Science and Programming in Python, Fall 2016 (link takes you to 14:29).

[^2]: Explanation of straight-line and branching programs adapted from J. Guttag, _Introduction to computation and programming using Python: with application to understanding data_. Cambridge, MA: The MIT Press, 2017, p. 15.
