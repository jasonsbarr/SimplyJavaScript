# Getting started with computing and computer science

## Computing, computers, and computer science

Ok, so technically you don't *have* to understand computer science in order to program. In fact, I worked as a freelance programmer for years before I read my first book on computer science.

Understanding the basics of computer science will help you become a better programmer, though. Once you know how to think like a computer scientist, you'll be able to compose more efficient, more effective programs. Maybe you'll even be able to get paid more! 🤑

I'm going to explain some computer science concepts, starting at a very basic level, to help things make more big-picture sense once we start programming in earnest.

I'll also include examples in JavaScript, the language we'll be using throughout the series, of some of the concepts I discuss here. Don't worry if you don't understand them; that will come as we get into the programming part!

### Computing

To make a very long story very, *very* short, **computing** is basically the act of calculating the solution to a problem, whether the problem is mathematical, scientific, literary, or of some other domain.[^1]

#### *Example 1*

```javascript
// Some computations in JavaScript

// Addition
2 + 4; // -> 6

// Finding the circumference of a circle
2 * Math.PI * 5; // -> 31.41592653589793

// Formatting a name
const caseifyName = name =>
  name[0].toUpperCase() + name.substring(1).toLowerCase();

const badlyFormattedAuthor = "JaSoN bArR"

const properlyFormattedAuthor = badlyFormattedAuthor
  .split(" ")
  .map(name => caseifyName(name))
  .join(" "); // -> Jason Barr
```

### Computers

A **computer** in the broad sense is anything that computes. We usually think of computers as machines, but the first computers were actually human beings!

In fact, the earliest use we know of the word "computer" was a reference to a person who carried out mathematical calculations,[^2] and the word was used exclusively in the same way until mechanical computers became more prominent in the late 19th century.

Early electronic computers were huge&mdash;so huge they could fill a room, or even *several* rooms. They got smaller as computer designs and engineering improved, and now you can fit fully-functional computers with more computing power than those room-sized, 1960s behemoths in your pocket.

![Watching a video on a pocket-sized computer](https://upload.wikimedia.org/wikipedia/commons/d/dd/2015-07-03_Grundschule_Goetheplatz%2C_Hannover%2C_Schulfest_mit_Kinderliedermacher_Unmada_%2842%29.JPG)

*Photo credit: [Bernd Schwabe](https://de.wikipedia.org/wiki/Benutzer:Bernd_Schwabe_in_Hannover), published under Creative Commons ([CC-BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0)). Source: [Wikimedia Commons](https://commons.wikimedia.org/wiki/Category:People_with_smartphones#/media/File:2015-07-03_Grundschule_Goetheplatz,_Hannover,_Schulfest_mit_Kinderliedermacher_Unmada_(42).JPG)*

### Computer science

It follows, then, that **computer science** is the rigorous study of how computing works. Trying to arrive at a precise definition of computer science is rather like nailing Jello to a wall, but we might broadly say it seeks to answer *at least* these 3 questions:[^3]

1. What can we compute?
2. How can we compute it?
3. What can we do with the result?

For most people getting started, questions 2 and 3 are the most pertinent. The act of **programming** is fundamentally about telling a computer what to do to compute a result, and then what to do with it.

### Systematic problem solving

Learning to program takes more than just mastering the grammar and syntax of a programming language, though it also requires that.

To program well, one must acquire the ability to systematically think through problems and compose solutions.

The phrase "compose solutions" hints at a *vital* skill for programmers: the ability to take a big problem and break it down into several smaller ones. Then, if you can solve all the smaller problems, you will also solve the larger one.

The act of taking a big problem and turning it into a series of smaller ones is called **decomposition.**

#### *Example 2*

```javascript
// Example of program decomposition
// Problem: get the sum of the squares of a series of numbers
const numberList = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

// Add two numbers
const add = (x, y) => x + y;

// Get the square of a number
// JavaScript has built-in ways to do this,
// but this is here for illustration:
const square = x => x * x;

// Putting it all together
const sumOfSquares = numbers.reduce((sum, number) =>
  add(sum, square(number)), 0); // -> 385
```

### Algorithms and thinking algorithmically

To solve problems systematically you must learn to think in terms of algorithms. An **algorithm** is a process you use to solve a particular problem.

Recipes for cooking are often used as an analogy for algorithms, and with good reason: a recipe is essentially an algorithm for preparing a particular dish.[^4]

#### *Example 3*

> ***Cookie and ice cream pie***
>
> *For 8 servings*
>
> **Ingredients:**
>
> - 20 chocolate sandwich cookies
> - 1 cup melted chocolate
> - 1 3/4 quarts of softened ice cream
>
> **Preparation:**
>
> 1. Place cookies in a gallon sized plastic bag and hit with a rolling pin or pan until crushed.
> 2. Pat the cookie crumbs into the bottom of a 9” (23 cm) pie dish.
> 3. Spread the softened ice cream on top and smooth out.
> 4. Drizzle the top with melted chocolate.
> 5. Freeze for 4 hours, or until the ice cream is hardened.
> 6. Enjoy!

_Source: [3-ingredient Cookies & Ice Cream Pie Recipe by Tasty](https://tasty.co/recipe/3-ingredient-cookies-ice-cream-pie)_

### Complexity and abstraction

Certain kinds of problems require algorithms that can be generalized. You can solve them the same basic solution.

That kind of generalization is a form of **abstraction,** which basically means taking a complex and/or particular process and "boxing it up" so it can be applied more generally in ways that allow us to treat it as a single unit.

For example, once you have a program that calculates square numbers, you can just use it any time you need a square number in a larger program. You don't need to know how it works in order to use it; you just use it. You may have written it to calculate a particular square root, but proper use of abstraction will let you use it to calculate *any* square number.

#### *Example 4*

```javascript
// Calculating a square number
9 * 9; // -> 81

// Abstracting the computation
const square = x => x * x;
square(4) // -> 16
square(20) // -> 400
square(1747) // -> 3052009
```

Abstraction is a powerful tool for managing complexity. Think about it: if you know how to push the pedals on your car, you don't have to worry about exactly how they work. Pushing the accelerator makes you start moving and speed up, pushing the brake pedal makes you slow down and stop, and if you have a manual transmission pushing the clutch allows you to shift gears.

You don't need to know how the fuel injection system, internal combustion, or the computers that make your car run work; you can just push the pedal and go.

Abstraction and decomposition are powerful tools for managing complexity, which is central to the task of programming. Programming is all about managing complexity in order to create change.[^5]

[^1]: There are some who would say "computing" is just a mathematical term. Those people are silly and should be avoided whenever possible. Or, at the very least, they need to expand their definition of "mathematical."

[^2]: In a book called *The yong mans gleanings* by the English writer Richard Braithwait.

[^3]: See the [online textbook for Berkeley's old CS61AS course](https://berkeley-cs61as.github.io/textbook/intro-to-computer-science.html)

[^4]: Who knew computing could be so delicious?

[^5]: J. Guttag, _Introduction to computation and programming using Python: with application to understanding data_. Cambridge, MA: The MIT Press, 2017, p. 110.
