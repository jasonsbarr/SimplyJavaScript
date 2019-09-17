# Simply JavaScript: an introduction to modern programming and computer science using the world's most popular programming language

While there are literally thousands of beginner JavaScript tutorials out there, most have at least one of the following fatal flaws:

-   They use outdated JavaScript syntax and programming techniques
-   They teach the JavaScript language, but not good programming fundamentals
-   They give you just enough JavaScript to get by before diving into the framework of the day

My goal here is to create a series of tutorials that avoids these pitfalls and helps students develop a strong foundation in computing, program design, and interacting with machines from a programmer's point of view.

## Programming, not web development

The purpose of this series is to teach students how to write well-structured, efficient programs using the JavaScript language.

It is _not_ a web development tutorial.

This is an important distinction. The latter will teach you how to build applications for a specific environment: a web browser and/or web server users will interact with via the browser.

These tutorials will teach you **how to program**, a skill that will enable you to build applications for any environment.

There's nothing wrong with web development tutorials as such, but it's crucial to have a strong programming foundation. If you know programming, you will build better web applications.

Given that web applications are the most common use for JavaScript, you will also learn a little about how to apply your programming knowledge to both client- and server-side web development, but it's not the main focus.

## Computer science fundamentals, with modern programming techniques

After working through these tutorials you will have a solid understanding of basic computer science: how computers work, how machines parse and execute programs, how to organize and process data, and how to evaluate and improve program efficiency.

You will also develop the basic skills needed to write programs other developers can read, understand, and work on (and sometimes that "other programmer" will be you, 6 months in the future).

When you understand these things you'll have a massive advantage over others who have only learned the framework _du jour_ or the basics of the JavaScript language itself.

You'll also be able to apply these fundamentals to any other programming language or framework.

## Sources of inspiration

Much of what I write here is influenced by Abelson, Sussman, and Sussman's seminal [_Structure and Interpretation of Computer Programs_](https://mitpress.mit.edu/sites/default/files/sicp/full-text/book/book.html), although it is certainly not an attempt to translate _SICP_ into JavaScript.

I've also taken some inspiration from Harvey and Wright's [_Simply Scheme_](https://people.eecs.berkeley.edu/~bh/ss-toc2.html), which was written as a kind of basic primer for students who are not quite yet to the level of starting with _SICP_.

I've also learned a lot from John DeNero's [_Composing Programs_](https://composingprograms.com/), which is itself based on _SICP_ and adapted for students beginning with Python as their first language.

Allen Downey's [_Think Python, 2e_](https://greenteapress.com/wp/think-python-2e/) and its alternate version [_Think Java_](https://greenteapress.com/wp/think-java) are outstanding introductions to programming for beginners that also emphasize fundamentals of computer science and program design.

The [Modern JavaScript Tutorial](https://javascript.info) stands out as a stellar example of a basic JavaScript tutorial that emphasizes modern techniques and code style.

[_Eloquent JavaScript_](https://eloquentjavascript.net) by Marijn Haverbeke is an excellent introduction to programming that uses JavaScript. I strive for his conciseness and clarity, although I hope the learning curve over the first few chapters is less steep here than it is in his excellent work.

Finally, [_JavaScript for Impatient Programmers_](https://exploringjs.com/impatient-js/) by Dr. Axel Rauschmayer is an outstanding introduction to modern JavaScript for newcomers who already know how to program in another language.

## Outline/Table of Contents

Since I'm in the _very_ early stages of developing this series, this is subject to change _radically_ without notice

### I.  Elements of Programming and JavaScript Language Basics

#### 0.  Getting started

    -   What is computer science?
        -   What can we compute?
        -   How do we compute it?
        -   What can we do with that?
    -   Complexity and abstraction
    -   What is a program?
        -   Computations and algorithms
        -   Data and operations
            -   I/O
            -   Instructions
            -   Data and state
        -   3 parts of an algorithm
            1.  Set of instructions
            2.  Flow of control
            3.  A way to tell when to stop
    -   Running JavaScript programs interactively
        -   Browser console
        -   Node REPL
    -   "Hello, JavaScript"

#### 1.  Elements of programming: data, values, types, & binding

    -   Value data types
        -   Number
        -   String
        -   Boolean
    -   Reference data types
        -   Array (list)
        -   Object (dictionary)
            -   Properties
            -   Dot and bracket notation
            -   Special built-in objects
        -   Map (and WeakMap)
        -   Set (and WeakSet)
    -   Null and undefined
    -   Bindings: constants and variables
        -   Assignment expressions
            -   _const_
            -   _let_
            -   _var_
            -   Mutable vs. immutable data
        -   Everything is a(n object) pointer
    -   Code blocks and binding scope

#### 2.  Elements of programming: operations and functions

    -   Expressions
    -   Arithmetic operators
    -   Comparison and logical operators
        -   Booleans revisited
        -   Dynamic types
        -   Coercion and gotchas
    -   Combining expressions
    -   Functions: callable values
    -   Functions as expressions/callables
    -   Built-in functions
    -   Defining your own functions
        -   Functions that take params
        -   Default params
        -   Void functions
        -   Functions that return a value
        -   Pure vs. impure functions
    -   Function evaluation & the call stack
    -   Functions as values
        -   Anonymous functions
        -   Passing functions as params
        -   Functions as object methods
        -   Functions, objects, and `.bind`

#### 3.  Elements of programming: control flow

    -   Statements
        -   Compound statements
        -   Code blocks
    -   Scope
        -   Block scope
        -   Function scope
        -   Local assignment and operations
        -   Environments
    -   Conditionals
    -   Recursion
        -   Dividing the problem
        -   Base cases
        -   The leap of faith
        -   Tree recursion
        -   Environments and the call stack
    -   Iteration
    -   Errors and error handling

#### 4.  Building applications: program organization and function design

    -   Design and process
    -   Declarative vs. imperative programming
    -   Functions and abstraction
        -   When to abstract?

### II. Programming with Objects and other built-in data types

#### 5.  Working with value data types

    -   Strings and methods
    -   Numbers, their methods, & the Math object

#### 6.  Creating dictionaries with Objects, Maps, and WeakMaps

#### 7.  Object-oriented programming: prototypes and inheritance

#### 8.  Arrays, Sets, and other iterable collections

#### 9.  Building applications: managing data flow with design patterns

### III. Programming with Functions as Objects

#### 10. Higher order functions, callbacks, and functions as objects

#### 11. Scope, environments, and closures

#### 12. Functional programming: abstraction & composition

#### 13. Composing objects with functions

#### 14. Building applications: functional object-oriented programming

### IV. Programming with more complex data and managing application state

#### 15. Data structures and abstraction

    -   Strings
    -   Advanced template literals
    -   Stacks, queues, and deques
    -   Heaps
    -   Trees
    -   Linked lists

#### 16. Searching and sorting algorithms

#### 17. Graphs and graph algorithms

    -   Breadth-first search
    -   Depth-first search
    -   Shortest path algorithms
    -   Minimum spanning tree

#### 18. Algorithm design and techniques

    -   Brute force
    -   Divide and conquer
    -   Greedy
    -   Backtracking
    -   Branch and bound

#### 19. Dynamic programming

#### 20. Algorithm complexity and performance

    -   Time and space complexity
    -   Recursion vs iteration
    -   Memoization
    -   Orders of growth
    -   Examples: analyzing Fibonacci, factorial, and exponentiation

#### 21. State and mutability

    -   Local vs. global
    -   Mutable vs. immutable
    -   Synchronicity vs. asynchronicity

#### 22. Building applications: using data structures to manage state

### V.  Programming with asynchronicity and streams

### VI. Programming with real-world data sets and users
