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

### I.  [Computers, programming, and JavaScript](1-computers-programming-and-javascript)

#### 0. [Getting started with computing and computer science](1-computers-programming-and-javascript/0-getting-started.md)

-   [What is computing?](1-computers-programming-and-javascript/0-getting-started.md#computing)
-   [What is a computer?](1-computers-programming-and-javascript/0-getting-started.md#computers)
    -   Human computers and calculating machines
    -   1613: first known use of the word "computer"
    -   From human to digital computers
-   [What is computer science?](1-computers-programming-and-javascript/0-getting-started.md#computer-science)
    -   The 3 big questions
        -   What can we compute?
        -   What's the best way to compute it?
        -   What can we make or do with the result?
    -   [Systematic problem solving](1-computers-programming-and-javascript/0-getting-started.md#systematic-problem-solving)
    -   [Algorithms and thinking algorithmically](1-computers-programming-and-javascript/0-getting-started.md#algorithms-and-thinking-algorithmically)
-   [Complexity and abstraction](1-computers-programming-and-javascript/0-getting-started.md#complexity-and-abstraction)
    -   Programming as managing complexity
    -   Abstraction lets us treat a complicated process as a simple understanding
    -   Car example
    -   Managing complexity is central to programming

#### 1. Understanding programs and data processing

-   What is a program? A piece of written language that describes how the computer will perform a computation
    -   Computation and algorithms
        -   Computation: a rational process that transforms inputs into results
        -   Algorithm: a set of instructions, like a recipe, that tells a computer (mechanical or otherwise) how to perform a computation
    -   Data
        -   Data is a symbol or symbols given meaning by specific acts of interpretation (information is data plus interpreted context)
        -   Computation turns data into information by placing it in an interpretive context meaningful to humans
        -   The algorithm that transforms data into information is itself also data
        -   Data is given structure by one or more programs in the computer so it can be stored and retrieved in meaningful and useful ways
    -   State
        -   The computer's or program's sequential memory (not memory as storage)
        -   A current snapshot of the computer's/program's current position in relation to the task it is currently in the process of performing
        -   The current values a program holds/references in memory based on where the program is with regards to its overall process of execution
        -   A computer's or program's output at any given time is completely determined as a function of current inputs and state
        -   Managing machine and program state is one of the most crucial (and difficult!) tasks a programmer must perform
    -   The program gets data as input, performs operations on the data that move it through various states in the process, and outputs the resulting new information
    -   3 parts of an algorithm
        1.  Set of instructions
        2.  Flow of control
        3.  Terminal condition

#### 2. Programming languages: what they are and how they work

-   Programming languages are languages
    -   Digital representation of human language
    -   Elements of programming languages
        -   Primitives
        -   Syntax
        -   Static semantics
        -   Semantics
-   Programs and programming languages
    -   Low level and high level languages
        -   Machine code and assembly
        -   Machine-independent languages and compiling (Grace Hopper and A-0)
        -   The first high-level languages: FORTRAN, LISP, and COBOL
        -   Modern programming languages
    -   Compiled vs. interpreted
    -   Dynamically vs. statically typed
    -   Compile time and runtime

#### 3. The JavaScript language: what it is and how to write your first programs

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
-   Running JavaScript programs interactively
    -   Browser console
    -   Node REPL
-   Your first program(s)

### II. The basic elements of programming

#### 4.  Data, types, and binding values

-   Expressions and values
-   Primitive data types
    -   Immutable
    -   Pass by value
    -   Wrapper Objects and primitive constructors
        -   String
        -   Numbers
        -   BigInt
        -   Boolean
        -   Symbol
-   Composite data types
    -   Mutable by default
    -   Pass by reference
    -   Constructors vs. literal notation
        -   Array
        -   Object
            -   Properties
            -   Dot and bracket notation
            -   JSON
        -   Map (and WeakMap)
        -   Set (and WeakSet)
        -   Function
-   Null and undefined
-   Bindings: constants and variables
    -   Assignment expressions
        -   Declaration vs. assignment
        -   The heap
        -   _const_
        -   _let_
        -   _var_
        -   Evaluation order from the inside out
        -   Destructuring and spreading
    -   Everything is a(n object) pointer
    -   Garbage collection
-   Example: Dog years converter

#### 5.  Operations and functions

-   Operations and expressions
-   Unary and binary operators
-   Comparison and logical operators
    -   Boolean algebra
    -   Truthiness and falsiness
    -   Dynamic types and coercion
    -   Type coercion pitfalls
-   Bitwise operators
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
    -   Function signatures, arity, and taking a variable number of parameters (variadic functions)
    -   Docblocks and function definitions
-   Function evaluation & the call stack
-   Functions as data
    -   Anonymous functions
    -   Functions as parameters and return objects
    -   Functions as Object methods
    -   Functions, Objects, and `this`
        -   Rules for binding `this`
        -   Arrow functions and `this`
        -   `call` and `apply`
        -   `bind`
    -   Functions as abstractions for managing complexity
-   Example: Units converter between SI and Imperial

#### 6.  Scopes and control flow

-   Code blocks
-   Scope, naming, and environments
    -   Environments as data structures for managing bindings
    -   Global scope
    -   Block scope
    -   Function scope
        -   Nested functions
        -   IIFEs
        -   Closures preview
    -   Local assignment and operations
    -   Lexical environments and the stack
    -   The scope chain
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
        -   Conditional execution with enumerables
-   Recursion
    -   Linear recursion
        -   Dividing the problem
        -   Base cases and recursive calls
        -   The leap of faith
        -   Tail call recursion
    -   Stack frames and state
    -   Pitfalls
    -   Example: recursive exponentiation
-   Iteration
    -   `while` and `do...while`
    -   `for`
    -   `break` and `continue`
    -   `for...in` (don't use this)
    -   `for...of`
    -   `.forEach()`
    -   Guess and check algorithms
        -   Exhaustive enumeration (or brute force)
            -   Linear search
            -   Example: number guessing game
        -   Divide and conquer
            -   Binary search
            -   Example: refactored number guessing game
    -   Iteration vs. recursion
        -   State
        -   Memory usage
        -   Performance
        -   Mutability and assignment
    -   Example: iterative exponentiation
-   This is now a Turing complete subset of JavaScript
-   Errors and error handling
    -   `throw`
    -   `try`/`catch`/`finally`
-   Basic debugging and testing
    -   Using the Console
    -   Using a debugger
    -   Example: debugging a square root algorithm
    -   The Assert API
    -   Build a simple testing library
    -   Using a 3rd party testing library
-   Example: Rock, paper, scissors game (Stretch: add lizard, Spock)

#### 7.  Building applications: program organization and design

-   Why design programs?
-   Declarative vs. imperative programming
-   Functions and abstraction
    -   Decomposition
    -   Extracting repeated code
    -   "Wishful thinking"
-   The design process
    -   Clarify the problem. Make sure you understand _why_ the problem needs to be solved, what _results_ a solution would achieve for you, and the _benefits_ of getting those results. Answer the question _what is the purpose of this program?_
    -   Break the problem into smaller, more easily solvable parts (sub-problems). Answer the question _what things need to happen to handle each salient aspect of the overall problem?_
    -   Define the data that will be used to represent the information relevant to one of the sub-problems. Answer the question _how do I accurately model the problem so that the output of the function is an accurate solution to the real-world problem?_
    -   Calculate the outputs you should expect from your function based on various example inputs, to make sure you understand what kind of tranformation you need to apply to inputs in the actual program to get the desired output. Answer the question _how do I need my function to manipulate and process its input data to compute the correct output to solve this part of the overall problem?_
    -   Stub out your function signature to state what kind of data they will both consume as input and produce as output, and then map the data transformation to fulfillment of the function's purpose. Answer the question _how will making the correct computation here contribute to the whole solution?_
    -   Translate your definition(s) into a broad outline of how the parts of the program will each solve the problem it's designed to solve. In other words, describe the steps of your algorithm(s). Answer the question _how will this compute the necessary values to solve this particular part of the problem?_
    -   Fill in the gaps with the first iteration of your program's code. Answer the question _how do I use the programming language and environment to correctly implement the steps of the algorithm?_
    -   Test the function with example inputs to make sure it computes as it should, without unexpected mistakes. If it turns out there are mistakes, review and refine the previous steps and then make adjustments to the code. Continue iterating this process until the function passes all the relevant tests. Answer the question _does this work in all possible situations relevant to the problem itself?_
    -   When you're sure the function is doing as it should, add any necessary relevant information to complement the function signature and definition. That way future users, as well as developers who test and maintain your code, will have documentation to understand the what, how, and why of the function.
    -   Repeat this process until you've created solutions for each sub-problem. Then put them all together so your functions compose a solution to the overall problem.
-   The importance of writing clear, readable code
-   How to organize your code well
-   Using third-party libraries
-   A brief intro to test-driven development
-   Example: A trivia game that runs in the console/REPL (Stretch: add a countdown timer, implement penalties for wrong answers, make it multiplayer)

#### Project: Battleship using TDD
