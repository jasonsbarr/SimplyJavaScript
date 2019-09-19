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
    -   Computation and computing
    -   Theoretical CS as applied mathematics
    -   Applications of CS
    -   The 3 big questions
        -   What can we compute?
        -   How do we compute it?
        -   What can we do with the result?
-   Complexity and abstraction
-   What is a computer?
    -   Human computers and computing devices
    -   From analog to digital computing
    -   Fixed program vs stored program
    -   Turing completeness
    -   Code as both instructions and data (Von Neumann architecture)
-   What is a program?
    -   Computations and algorithms
    -   Data, operations, and state
    -   3 parts of an algorithm
        1.  Set of instructions
        2.  Flow of control
        3.  Terminal condition
-   Programming languages are languages
    -   Primitives
    -   Syntax
    -   Static semantics
    -   Semantics
-   Programs and programming languages
    -   Ada Lovelace programs the Analytical Engine
    -   Low level and high level languages
        -   Machine code and assembly
        -   Machine-independent languages and compiling (Grace Hopper and A-0)
        -   The first high-level languages: FORTRAN, LISP, and COBOL
        -   Modern programming languages
    -   Compiled vs. interpreted
    -   Dynamic vs. static data types
    -   Compile time and runtime
-   A _very brief_ history of JavaScript
-   Overview of JavaScript's basic syntax
    -   Identifiers
    -   Statements and expressions
    -   Syntactic ambiguities
    -   Strict mode
-   Running JavaScript programs interactively
    -   Browser console
    -   Node REPL
-   Your first program: "Hello, JavaScript"

#### 1.  Elements of programming: data types and binding values

-   Value data types (primitives)
    -   Values as expressions
    -   Using object properties and methods
        -   String
        -   Numbers and Math
        -   BigInt
        -   Boolean
        -   Symbol
-   Reference data types (composites)
    -   Value vs. reference data types
    -   Array
    -   Object
        -   Properties
        -   Dot and bracket notation
        -   JSON
        -   Dates
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

#### 3.  Elements of programming: scopes and control flow

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
    -   Stack frames and state
    -   Pitfalls
-   Iteration
    -   `while`
    -   `for`
    -   `break` and `continue`
    -   `for...in`
    -   `for...of`
    -   `.forEach()`
    -   Exhaustive enumeration algorithms
    -   Iteration vs. recursion
        -   State
        -   Memory usage
        -   Performance
        -   Mutability and assignment
-   Errors and error handling
    -   `throw`
    -   `try`/`catch`/`finally`
-   Basic debugging and testing
    -   Using the Console
    -   Using a debugger
        -   Browser debuggers
        -   Node's built-in Debugger
        -   Debugging Node with the Chrome debugger
    -   The Assert API
    -   Build a simple testing library
    -   Using a 3rd party testing library

#### 4.  Building applications: program organization and design

-   Design and process
-   Declarative vs. imperative programming
-   Functions and abstraction
    -   Decomposition
    -   Extracting repeated code
    -   "Wishful thinking"
-   Writing clear, readable code

**Project**

### II. Programming with Objects and other built-in data types

#### 5.  Advanced String techniques

-   Working with Unicode and other advanced String shenanigans
-   Template literals and tagged templates
-   Regular Expressions

#### 6. Keyed data structures (dictionaries) with Objects, Maps, and WeakMaps

-   Advanced object creation
    -   Objects without prototypes
    -   Accessors
    -   Using Symbols as keys
    -   Setting property attributes
    -   Freezing Objects
    -   Standard methods
-   Mutating Objects
-   Working with immutable Objects
-   Key/value data structures
    -   Associative array
    -   Dictionary
    -   Hash table
-   Using Objects as dictionaries
-   Better dictionaries with Maps
-   Maps vs. WeakMaps
-   Structs

#### 7. Objects and prototypal inheritance

-   Understanding object-oriented programming
    -   Abstraction
    -   Encapsulation
    -   Inheritance
    -   Polymorphism
-   Understanding JavaScript's Object model and prototypes
-   The `__proto__` property
-   Prototypes _are_ Objects
-   Inheritance and the prototype chain
-   Constructor functions and the `new` keyword
-   Emulating classes and subclasses with constructors and prototypes
-   Encapsulation and private data
-   The ES5 module pattern

#### 8. ES6 Classes and inheritance

-   Classes as syntactic sugar for prototypal inheritance pattern
    -   Creating subclasses with `extend` and `super()`
    -   Extend Classes with non-Class Objects
    -   Classes and strict mode
    -   Static methods
    -   Private data?
    -   Field declaration syntax (experimental)
    -   Classes and `this`
    -   Class expressions
    -   Classes and hoisting
    -   Classes as special functions
    -   Classes, mixins, and composition
-   Converting constructors to Classes
-   Differences between Classes and pseudoclassical inheritance with constructors
-   Using Symbols to simulate interfaces
-   Decorators, monkey patching, and duck typing
-   Problems with inheritance, `new`, and ES6 Classes
-   Alternate approach: behavior delegation
-   Looking ahead to functional object-oriented programming

#### 9. Arrays, Sets, and other iterable collections

-   Iteration, iterators, and iterables
-   Arrays as lists
-   Searching and sorting Arrays
-   Higher order Array methods
-   Mutable vs. immutable Arrays
-   Typed Arrays and binary data
-   Sets and WeakSets
-   Iterating with Objects, Maps, and WeakMaps
    -   Making iterable Objects
    -   HTML collections in the browser
    -   Building a jQuery-like HTML Element collection
-   Multidimensional Arrays
-   [Symbol.iterator] and iterator methods
    -   Building a Matrix data structure with multidimensional Arrays and [Symbol.iterator]
    -   Tool functions and combinators
    -   Infinite iterables
-   Building a Python-like Tuple data structure
-   Using collection libraries
    -   Collection.js
    -   Immutable.js

#### 10. Metaprogramming JavaScript

-   Introspection
-   Using constructors for built-in data types
-   Defining code at runtime
    -   The `new Function()` syntax
    -   Is `eval()` evil?
-   `Symbol`
-   `Reflect`
-   `Proxy`
-   Feature testing
-   Macros with Sweet.js

#### 11.  Building applications: organizing code and managing data flow with object-oriented design patterns

-   Classical design patterns
-   Messaging and event-driven patterns
-   Module patterns
-   Application-level design patterns
-   Microservices
-   Functional and reactive patterns

**Project**

### III. Programming with Functions

#### 12. Higher order functions

-   Recap: functions as data
-   Functions as abstractions
-   Higher order functions
    -   Functions as parameters
    -   Generalize methods of computation with polymorphic functions
    -   Functions as returned values
    -   Lambda expressions
    -   Function decorators

#### 13. Scopes and closures

-   Lexical environments and functions
    -   Bound and free variables
    -   Stack frames and call objects
-   Closures
    -   You've been using closures all along
    -   Nested functions and extended environments
    -   Enclosing loops and code blocks
    -   Closures, private data, and modules
    -   Abstraction and encapsulated state
    -   Referring to closures from global scope
-   Using closures and higher order functions together
-   Basic functional composition

#### 13. Recursion revisited

-   Advantages of recursion over iteration for functional programming
-   Declarative recursion
-   Exhaustive enumeration with linear recursion
-   Mutual recursion
-   Tree recursion
-   Improving performance and memory management
    -   Memoization
    -   Proper tail calls
    -   Replacing the stack
    -   Continuation passing style
    -   Trampolines
    -   Self-adjusting code
    -   Tail call optimization with Fext.js
-   Recursive patterns
    -   Every (map)
    -   Keep (filter)
    -   Accumulate (reduce)
-   Advanced recursion examples

#### 13. Purity of function is to do one thing

#### 14. Partial application and functional composition

-   Composition definition and basics
-   Expressions, abstractions, and applications: using the Lambda calculus to model computation

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
-   The application as a finite state machine

#### 25. Building applications: using data structures to manage state

**Project**

### V.  Programming asynchronously

**Project**

### VI. Programming reactively with real-time data and streams

-   Observables and the observer pattern

**Project**

### VII. Programming the browser

**Project**

### VIII. Programming on the server

**Project**

### IX. Building a full-stack application with real world data and users

### X. The kitchen sink

-   A. Problem solving methodology
-   B. Code formatting and style guides
-   C. Software engineering paradigms
    -   Waterfall
    -   Agile
