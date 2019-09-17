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

### I.  Elements of programming and JavaScript language basics

#### 0. Getting started with computer science and programming

-   What is computer science?
    -   Computation
    -   Theoretical CS as applied mathematics
    -   CS as engineering
    -   The 3 big questions
        -   What can we compute?
        -   How do we compute it?
        -   What can we do with the result?
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
        3.  Terminal condition
-   Programs and programming languages
    -   Compiled vs. interpreted
    -   Dynamic vs. static data types
    -   Compile time and runtime
-   Programming languages are languages
    -   Primitives
    -   Syntax
    -   Static semantics
    -   Semantics
-   Overview of JavaScript's basic syntax
    -   Identifiers
    -   Statements and expressions
    -   Strict mode
-   Running JavaScript programs interactively
    -   Browser console
    -   Node REPL
-   The first program: "Hello, JavaScript"

#### 1.  Elements of programming: data types and binding values

-   Value data types (primitives)
    -   Values as expressions
    -   Using object properties and methods
        -   Number
        -   String
        -   Boolean
        -   Symbol
-   Reference data types (composites)
    -   Value vs. reference data types
    -   Array
    -   Object
        -   Properties
        -   Dot and bracket notation
        -   Special built-in objects
    -   Map (and WeakMap)
    -   Set (and WeakSet)
-   Null and undefined
-   Bindings: constants and variables
    -   Assignment expressions
        -   Declaration vs. assignment
        -   _const_
        -   _let_
        -   _var_
        -   Evaluation order from the inside out
        -   Destructuring and spreading
    -   Everything is a(n object) pointer
    -   Garbage collection

#### 2.  Elements of programming: operations and functions

-   Operations and expressions
-   Arithmetic operators
-   Comparison and logical operators
    -   Booleans revisited
    -   Dynamic types and coercion
    -   Type coercion pitfalls
-   Operators and precedence
-   Combining expressions
-   Functions are callable values
-   Function calls as expressions
-   Built-in functions
-   Defining your own functions
    -   Function declarations vs. function expressions
    -   Arrow functions
    -   Functions that take parameters
    -   Parameters vs. arguments
    -   Default parameters
    -   Void functions
    -   Functions that return a value
    -   Pure vs. impure functions
    -   Function signatures, arity, and variadic functions
    -   Docblocks and function definitions
-   Function evaluation & the call stack
-   Functions as values
    -   Anonymous functions
    -   Functions as parameters and return objects
    -   Functions as object methods
    -   Functions, objects, and `this`
        -   Rules for binding `this`
        -   Arrow functions and `this`
        -   `call` and `apply`
        -   `bind`
    -   Callback functions and asynchronicity

#### 3.  Elements of programming: environments and control flow

-   Code blocks
-   Scope, naming, and environments
    -   Global scope
    -   Block scope
    -   Function scope
        -   Nested functions
        -   IIFEs
    -   Local assignment and operations
    -   Lexical environments and stack frames
    -   Hoisting
-   Running time and control structures
-   Conditionals and branching
    -   `if`, `else if`, `else`
    -   `switch`
    -   The conditional (or ternary) operator
    -   Short-circuit evaluation
    -   Branching and function returns
        -   Single point of return
        -   Early returns and guard clauses
-   Recursion
    -   Linear recursion
        -   Dividing the problem
        -   Base cases and recursive calls
        -   The leap of faith
        -   Tail call recursion
    -   Tree recursion
    -   Stack frames and state
    -   Recursive patterns
        -   Every (map)
        -   Keep (filter)
        -   Accumulate (reduce)
    -   Advanced recursion examples
    -   Pitfalls
-   Iteration
    -   `while`
    -   `for`
    -   `break` and `continue`
    -   `for...in`
    -   `for...of`
    -   `.forEach()`
    -   Iteration vs. recursion
        -   State
        -   Memory usage
        -   Performance
-   Errors and error handling
    -   `throw`
    -   `try`/`catch`/`finally`
-   Basic testing
    -   The Assert API
    -   A simple testing library
    -   Using a 3rd party testing library

#### 4.  Building applications: program organization and design

-   Design and process
-   Declarative vs. imperative programming
-   Functions and abstraction
    -   Extracting repeated code
    -   Decomposition
    -   Wishful thinking

**Project**

### II. Programming with Objects and other built-in data types

#### 5.  Advanced techniques with Strings and Symbols

-   Strings
-   Template literals and tagged templates
-   Symbols

#### 6. Creating dictionaries with Objects, Maps, and WeakMaps

#### 7. Prototypes and inheritance, with and without `class`es

#### 8. Arrays, Sets, and other iterable collections

#### 9. Metaprogramming with Symbols, Reflect, and Proxies

#### 10.  Building applications: managing data flow with object-oriented design patterns

-   Classical design patterns
-   Messaging patterns
-   Modules, old and new
-   Application-level design patterns
-   Microservices
-   Functional and reactive patterns

**Project**

### III. Programming with Functions

#### 11. Higher order functions

#### 12. Scope, environments, and closures

#### 13. Purity of function is to do one thing

#### 14. Functional abstraction and composition

#### 15. Containers and monads and functors, oh my!

#### 16. Functional control flow without ifs or loops

#### 16. Composing objects with functions

#### 17. Building applications: functional object-oriented programming

**Project**

### IV. Programming with more complex data and managing application state

#### 18. Data structures and abstraction

-   Stacks, queues, and deques
-   Heaps
-   Trees
-   Linked lists

#### 19. Searching and sorting algorithms

#### 20. Graphs and graph algorithms

-   Breadth-first search
-   Depth-first search
-   Shortest path algorithms
-   Minimum spanning tree

#### 21. Algorithm design and techniques

-   Brute force
-   Divide and conquer
-   Greedy
-   Backtracking
-   Branch and bound

#### 22. Dynamic programming

#### 23. Algorithm complexity and performance

-   Time and space complexity
-   Recursion vs iteration
-   Memoization
-   Orders of growth
-   Examples: analyzing Fibonacci, factorial, and exponentiation

#### 24. Events and state

-   Local vs. global
-   Mutable vs. immutable
-   Synchronicity vs. asynchronicity
-   Events and messaging
-   The finite state machine

#### 25. Building applications: using data structures to manage state

**Project**

### V.  Programming with asynchronicity and streams

**Project**

### VI. Programming with real-world data sets and users

**Project**

### VII. The kitchen sink

#### A. The Date object

#### B. Regular expressions

#### C. Typed Arrays
