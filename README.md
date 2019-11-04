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

I've learned a lot from John DeNero's [_Composing Programs_](https://composingprograms.com/), which is itself based on _SICP_ and adapted for students beginning with Python as their first language.

Allen Downey's [_Think Python, 2e_](https://greenteapress.com/wp/think-python-2e/) and its alternate version [_Think Java_](https://greenteapress.com/wp/think-java) are outstanding introductions to programming for beginners that also emphasize fundamentals of computer science and program design.

The [Modern JavaScript Tutorial](https://javascript.info) stands out as a stellar example of a basic JavaScript tutorial that emphasizes modern techniques and code style.

[_Eloquent JavaScript_](https://eloquentjavascript.net) by Marijn Haverbeke is an excellent introduction to programming that uses JavaScript. I strive for his conciseness and clarity, although I hope the learning curve over the first few chapters is less steep here than it is in his excellent work.

Finally, [_JavaScript for Impatient Programmers_](https://exploringjs.com/impatient-js/) by Dr. Axel Rauschmayer is a fantastic introduction to modern JavaScript for newcomers who already know how to program in another language.

## Other versions

- Dev.to &ndash; [Simply JavaScript: learn computer science and programming in the world's most ubiquitous language (introduction and index)](https://dev.to/jasonsbarr/simply-javascript-learn-computer-science-and-programming-in-the-world-s-most-ubiquitous-language-introduction-and-index-29m5)

## Outline/Table of Contents

Since I'm in the _very_ early stages of developing this series, this is subject to change _radically_ without notice

### I.  [Computers, programming, and JavaScript](0-computers-programming-and-javascript)

#### 0. [Getting started with computing and computer science](0-computers-programming-and-javascript/0-getting-started.md)

-   [What is computing?](0-computers-programming-and-javascript/0-getting-started.md#computing)
-   [What is a computer?](0-computers-programming-and-javascript/0-getting-started.md#computers)
-   [What is computer science?](0-computers-programming-and-javascript/0-getting-started.md#computer-science)
    -   [Systematic problem solving](0-computers-programming-and-javascript/0-getting-started.md#systematic-problem-solving)
    -   [Algorithms and thinking algorithmically](0-computers-programming-and-javascript/0-getting-started.md#algorithms-and-thinking-algorithmically)
-   [Complexity and abstraction](0-computers-programming-and-javascript/0-getting-started.md#complexity-and-abstraction)

#### 1. Understanding and writing JavaScript programs

-   Hello, world: our first JavaScript program
    -   How to access the JavaScript console
    -   Writing your first JavaScript program
    -   How the interpreter works to run your first program
-   What is a program?
    -   Try it yourself: exercises for further learning

#### 2. Working with data and types

-   Data types
-   Built-in JavaScript data types
    -   Numbers
    -   Arithmetic operations
    -   Strings
    -   Type coercion
    -   Operator overloading
    -   Booleans
    -   Null and undefined
-   Binding data to names: constants and variables
    -   Naming conventions
    -   The difficulty of naming things
    -   Assignment expressions
    -   Variables, constants, and (im)mutability
    -   Assigning expressions
-   Try it yourself: exercises for further learning

#### Interlude: Setting up your development environment

#### 3. Functions: the building blocks of complex programs

-   Boolean logic and conditional execution
    -   Booleans and coercion
    -   Short-circuit evaluation
    -   The conditional expression
    -   Conditional statements
    -   Control flow vs. logical flow
-   Defining functions
    -   The new way: arrow function expressions
    -   The old way: the `function` keyword
-   Parameters and arguments
-   Returning values
    -   Void functions
    -   The `return` statement
-   Pure vs. impure functions
-   The `Function` data type

#### 4. Complex data types and iteration

-   Primitive vs. complex data types
-   Primitives as objects
    -   String properties and methods
    -   Number properties and methods
-   Arrays
    -   Creating Arrays
    -   Array properties and methods
    -   Destructuring and spreading Arrays
-   Iteration with Array methods
-   Objects
    -   Creating Objects
    -   Properties and methods
    -   Destructuring and spreading Objects
-   Iterating over Objects
-   Complex data types and (im)mutability
    -   Bindings and `const`
    -   `Object.seal`
    -   `Object.freeze`
-   Sets
-   Maps
-   Type checking
-   Imperative control flow: loops

#### Interlude: Programming languages in depth and the history of JavaScript

-   Programming languages are languages
    -   Digital representation of human language
    -   Elements of programming languages
        -   Primitives
        -   Syntax
        -   Static semantics
        -   Semantics
-   Programs and programming languages
    -   Low-level and high-level languages
        -   Machine code and assembly
        -   Machine-independent languages and compiling (Grace Hopper and A-0)
        -   The first high-level languages: FORTRAN, LISP, and COBOL
        -   Modern programming languages
    -   Compiled vs. interpreted
    -   Dynamically vs. statically typed
    -   Compile time and runtime
-   A _very brief_ history of JavaScript
    -   Early history and influences
    -   ECMAScript versions 3, 4, and 5
    -   NodeJS
    -   ECMAScript 6 and beyond
-   Overview of JavaScript's basic syntax
    -   Identifiers
    -   Statements and expressions
    -   Syntactic ambiguities
    -   Strict mode

### II. Abstracting with functions

#### ##. Scopes and closures

#### ##. Higher-order functions

#### ##. Recursion

#### ##. Composition

#### ##. Lists and streams

#### Interlude: Declarative vs. imperative programming styles

### III. Abstracting with data

#### ##. Simple vs. compound data

#### ##. Strings and string operations

#### ##. Numbers, math, and dates

#### ##. Arrays and iterators

-   `Array#map`
-   `Array#filter`
-   `Array#reduce`
-   `Array#find`, `#findIndex`, `#some`, and `#every`

#### ##. Objects and dictionaries

#### ##. Sequential abstractions

#### ##. Hierarchical abstractions

#### Interlude: Program decomposition and state management

### IV. Abstracting with state

#### ##. Program state and mutability

#### ##. Objects with prototypes

#### ##. Classes and inheritance

#### ##. Design patterns

#### ##. Declarative patterns with functional OOP

#### ##. Sorting and searching

#### ##. Graphs and dynamic programming

#### Interlude: Algorithms and analysis

-   Computation and algorithms
    -   Computation: a rational process that transforms data into results
    -   Algorithm: a set of instructions, like a recipe, that tells a computer (mechanical or otherwise) how to perform a computation
-   3 parts of an algorithm
    1.  Set of instructions
    2.  Program control
    3.  A terminal condition
-   Data, processing, and input/output
    -   Data is a symbol or symbols given meaning by specific acts of interpretation (information is data plus interpreted context)
    -   Computation turns data into information by placing it in an interpretive context meaningful to humans
    -   The algorithm that transforms data into information is itself also data
    -   Data is given structure by one or more programs in the computer so it can be stored and retrieved in meaningful and useful ways
-   Managing program state
    -   The computer's or program's sequential memory (not memory as storage)
    -   A current snapshot of the computer's/program's current position in relation to the task it is currently in the process of performing
    -   The current values a program holds/references in memory based on where the program is with regards to its overall process of execution
    -   A computer's or program's output at any given time is completely determined as a function of current inputs and state
    -   Managing machine and program state is one of the most crucial (and difficult!) tasks a programmer must perform
-   The program gets data as input, performs operations on the data that move it through various states in the process, and outputs the resulting new information

### V. Engineering applications

#### ##. Designing programs

#### ##. Asynchronous basics

#### ##. Events and reactivity

#### ##. Programming the browser: the Document Object Model

#### ##. Programming the server: Understanding Node.js

#### ##. HTTP requests and working with external data sources

#### ##. Full-stack development: Managing state with reactive UI

#### ##. Full-stack development: API development with Node and Express

#### ##. Putting it all together
