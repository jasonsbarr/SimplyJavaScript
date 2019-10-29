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

## Outline/Table of Contents

Since I'm in the _very_ early stages of developing this series, this is subject to change _radically_ without notice

### I.  Computers, programming, and JavaScript

#### 0. Getting started with computing and computer science

##### _Write most of this section as separate articles_

-   What is a computer?
    -   Human computers and calculating machines
    -   Primitive computing
    -   1613: first known use of the word "computer"
    -   19th and early 20th century computing
        -   Human computing
    -   Mechanical computing
    -   The Analytical Engine: the first theoretically universal computing machine
        -   The first computer programs
        -   Ada's vision of symbolic computing
    -   Early digital computers
        -   ABC
        -   Colossus
    -   Turing completeness and computability
        -   ENIAC – the first Turing complete digital computer
    -   Stored program computers and code as data (von Neumann architecture)
        -   Manchester Mark 1
        -   EDVAC
    -   Computers continue to get smaller and faster and more powerful
-   What is computer science?
    -   Computation and computing
    -   Theoretical computer science
    -   Applications of CS
    -   The 3 big questions
        -   What can we compute?
        -   What's the best way to compute it?
        -   What can we make or do with the result?
    -   Thinking algorithmically
-   Complexity and abstraction
    -   Programming as managing complexity
    -   Abstraction lets us treat a complicated process as a single understanding
    -   Car example
-   "Radical computer science"
    -   Programming as human expression
        -   Using machines and code to express human thoughts and (hopefully) solve human problems
        -   Translating between machines and humans
        -   Programming is _hard_, regardless of whether you approach it as art or science (it's both)
    -   Code is ποίησις.
        -   Expressing ideas, not just getting computers to do things
        -   Structured programming: computing based on control and correctness
        -   Symbolic programming: computing based on ideas
            -   Taking human ideas and making them material
            -   Programs are "little bits of you that perform independently"
        -   To program is to build something, and not just crunch numbers
        -   Computing can produce art, music, architecture, theatre
        -   Symbols are data the computer, and by extension the engineer, transforms into something meaningful
    -   The most important thing I can accomplish with these tutorials is to enable you to express yourself more fully by building something beautiful

#### 1. Understanding programs and programming languages

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
-   Your first program: "Hello, JavaScript"

### II. The basic elements of programming

#### 2.  Data, types, and binding values

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

#### 3.  Operations and functions

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

#### 4.  Scopes and control flow

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

#### 5.  Building applications: program organization and design

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

### III. Programming with Objects and other simple data structures

#### 6. String techniques

-   Working with Unicode and other advanced String shenanigans
-   Template literals and tagged templates
-   Regular Expressions
-   Voca.js: supercharged string manipulation
-   Example: An HTML parser that takes a tagged template string (Stretch: encode HTML entities, add Markdown parser)

#### 7. Numbers, Math, and Dates

-   The Number data type
-   Floating-point arithmetic
    -   Imprecision in binary-to-decimal conversion
    -   Handling money and other cases where you _must_ have absolute precision
-   The Math object
-   More advanced math operations with Math.js
-   Working with Dates
-   Better dates with Moment.js
-   Example: Calculator (Stretch: add a memory function and additional math operations) - HTML will be provided, DOM code will be explained

#### 8. Keyed data structures (dictionaries) with Objects, Maps, and WeakMaps

-   Advanced object creation
    -   Objects without prototypes
    -   Composing with `Object.assign()`
    -   Accessor properties
    -   Using Symbols as keys
    -   Setting property attributes
    -   Freezing and sealing Objects
    -   Standard methods
-   Mutating Objects
-   Working with immutable Objects
-   Key/value data structures
    -   Associative array
    -   Dictionary
    -   Hash table
    -   Example: hash table with hashing function
-   Using Objects as dictionaries
-   Better dictionaries with Maps
-   Maps vs. WeakMaps
-   Example: making a struct
-   Extend objects with Sugar.js
-   Example: Word frequency counter that searches for and fetches texts from Project Gutenberg (Stretch: count parts of speech, filter out stop words, visualize with graph/chart,)

#### 9. Objects and prototypal inheritance

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
-   UI components
-   Example: Blog feed (Stretch: add form to create new articles, sort, search, and filter articles)

#### 10. ES6 Classes and inheritance

-   Classes as syntactic sugar for prototypal inheritance pattern
    -   Creating subclasses with `extend` and `super()`
    -   Extend Classes with non-Class Objects
    -   Extending native Classes
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
-   Example: Build a library manager with OOP that fetches book info from API with HTML UI and data persistence in LocalStorage (Stretch: list books in multiple categories, implement a lending and return system with overdue reports and fees, let users reserve books)

#### 11. Arrays, Sets, and other iterable collections

-   Iteration, iterators, and iterables
-   Arrays as lists
-   Searching and sorting Arrays
-   Higher order Array methods
-   Mutating Arrays
    -   Reference data types and mutability
    -   Destructive Array methods
    -   The problem with mutation
    -   Non-destructive Array methods
    -   How to avoid mutating Arrays
    -   Use `Object.seal()` to create fixed-length Arrays
    -   Immutable Arrays with `Object.freeze()`
-   Typed Arrays and binary data
-   Sets and WeakSets
-   Example: removing duplicate entries from an array
-   Iterating with Objects, Maps, and WeakMaps
    -   Maps and WeakMaps are iterable by default
    -   Objects are not
        -   Using `for...in` on enumerable properties
        -   Why you shouldn't use `for...in`
    -   Making iterable Objects
    -   HTML collections in the browser
        -   The old way: `document.getElementsBy[Tag|Class]Name()`
        -   The better old way: jQuery selection and the `$` object
        -   The new way: `document.querySelectorAll()`
    -   Example: building a jQuery-like HTML Element collection
-   Multidimensional Arrays
-   [Symbol.iterator] and iterator methods
    -   Example: building a Matrix data structure with multidimensional Arrays and [Symbol.iterator]
    -   Tool functions and combinators
    -   Infinite iterables
-   Processing iterables the Lazy(.js) way
-   Example: building a Python-like Tuple data structure
-   Example: Build a Collection library that extends the native Array class (Stretch: replace the native Array class, make an immutable version, implement other data structures, change the `.toString()` method to generate a representation of the contained data)

#### 12. Iterators with synchronous generators

-   What are generators?
    -   Defining generator functions and methods
-   Iterating with generators as observables
    -   Generators return iterables and fill their values with `yield`
-   3 ways to iterate over a generator
    -   `for...of`
    -   Spreading
    -   Destructuring
-   `yield` and execution flow
    -   Functions and run-to-completion (`yield` pauses execution)
    -   The benefits of `yield` and lazy evaluation
    -   Returning from a generator
    -   Throwing errors from a generator
    -   Limitations of `yield`
-   Example: using a generator to build `range()`
-   Combinators and reducers
    -   Map
    -   Filter
    -   Reduce
-   Recursive and other nested generators
    -   You'll think this should work, but it doesn't
    -   The `yield*` operator
    -   Iterating over trees and nested arrays
-   External and internal iteration
    -   Example: reusing traversal code
        -   Building a tree
        -   Internal iteration and pushing values
        -   External iteration and pulling values
-   Generators as observers
    -   Sending values with `next()`
    -   `yield` and loose binding
    -   Using `return()` and `throw()`
        -   Terminating the generators
        -   Signaling an error
    -   `yield*` in more detail
    -   Example: processing asynchronous data
-   Reversing the direction of `yield`
-   Two-way data flow with cooperative multitasking
    -   Understanding the generator interface
    -   Creating coroutines
    -   Use cases for cooperative multitasking
        -   Processing streams
        -   Working with asynchronous operations
    -   Limitations of cooperative multitasking
-   Additional generator use cases
    -   Create iterables more easily
    -   Easier infinite iterables
    -   Example: infinite Fibonacci generator
-   Inheritance and the iteration API
    -   `IteratorPrototype`
    -   Understanding `this` with generators
-   Example: Make the collection class lazy

#### 13. Metaprogramming JavaScript

-   Introspection
-   Using constructors for built-in data types
-   Defining code at runtime
    -   The `new Function()` syntax
    -   Is `eval()` evil?
-   `Symbol`
-   `Reflect`
-   `Proxy`
-   Feature testing
-   Implement macros with Sweet.js
-   MetaScript: full-scale code transformation

#### 14.  Building applications: organizing code and managing data flow with object-oriented design patterns

-   Classical design patterns
-   Messaging and event-driven patterns
-   Module patterns
-   Application-level design patterns
-   Microservices
-   Functional and reactive patterns

**Project**

### IV. Programming with Functions

#### 15. Higher order functions

-   Recap: functions as data
-   Functions as abstractions
-   Higher order functions
    -   Functions as parameters
    -   Generalize methods of computation with polymorphic functions
    -   Functions as returned values
    -   Lambda expressions
    -   Function decorators

#### 16. Scopes, closures, and contexts

-   Lexical environments and functions
    -   Bound and free variables
    -   Stack frames and call objects
-   Closures
    -   You've been using closures all along
    -   Definition vs. execution contexts
    -   Nested functions and extended environments
    -   Enclosing loops and code blocks
    -   Closures, private data, and modules
    -   Abstraction and encapsulated state
    -   Referring to closures from global scope
-   Using closures and higher order functions together
-   Basic functional composition

#### 17. Recursion revisited

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

#### 18. The importance of using immutable data

-   Better functional data structures with Immutable.js

#### 19. Purity of function is to do one thing

#### 20. Currying, partial application and composition

-   Composition definition and basics
-   Expressions, abstractions, and applications: using the Lambda calculus to model computation

#### 21. Containers and monads and functors, oh my!

#### 22. Functional control flow without ifs or loops

-   Ramda.js

#### 23. Composing objects with functions

#### 24. Building applications: functional object-oriented programming

**Project**

### V.  Programming with complex data structures

#### 25. Data structures and abstraction

#### 26. Linear data structures

-   Lists, Arrays, and ArrayLists
-   Vectors
-   Stacks, queues, and deques
-   Linked lists
-   Sets
-   Matrices
-   Lookup tables

#### 27. Hierarchical and key/value data structures

-   Trees
-   Heaps
-   Associative arrays and dictionaries
-   Hashing and hash tables

#### 28. String algorithms

#### 29. Searching and sorting algorithms

-   Searching algorithms
    -   Linear search
    -   Binary search
    -   Jump search
    -   Interpolation search
-   Sorting algorithms
    -   Selection sort
    -   Bubble sort
    -   Insertion sort
    -   Merge sort
    -   Quick sort
    -   Radix sort

#### 30. Abstract data types and graphs

-   Breadth-first search
-   Depth-first search
-   Shortest path algorithms
-   Minimum spanning tree

#### 31. Blockchain: a distributed, decentralized data structure

-   Distributed hash tables
    -   Chord
    -   Content addressable network
    -   Tapestry
    -   Pastry
-   Peer-to-peer networks
    -   Distributed nodes
    -   The network as graph
    -   Example: Napster
    -   Example: BitTorrent
-   Consensus algorithms
-   Distributed ledgers
-   Blockchain

#### 32. Algorithm design and techniques

-   Guess and check
-   Brute force
-   Divide and conquer
-   Greedy
-   Backtracking
-   Branch and bound

#### 33. Dynamic programming

#### 34. Algorithm complexity and performance

-   Time complexity
    -   Asymptotic notations
        -   Big O
        -   Big Omega
        -   Big Theta
-   Space complexity
-   Recursion vs iteration
-   Memoization
-   Orders of growth
-   Examples: analyzing Fibonacci, factorial, and exponentiation

#### 35. Working with complex data and state

-   Local vs. global
-   Mutable vs. immutable
-   Synchronicity vs. asynchronicity
-   The application as a finite state machine

#### 36. Building applications: using data structures to manage state

**Project**

### VI. Programming with asynchronous patterns

#### 37. Understanding asynchronous programming in JavaScript

-   Synchronous vs. asynchronous operations
    -   Functions are synchronous by default
    -   Sequential tasks in a single process
    -   Asynchronous functions
        -   Callback-based
        -   Promise-based
        -   Synchronous-looking `async` and `await`
-   The heap and call stack
-   The event loop
-   JavaScript runtime and blocking
    -   Example: blocking the process in the browser UI
    -   How to avoid blocking the process
        -   Deliver the result asynchronously
        -   Generate separate processes
            -   Web Workers in the browser
            -   Worker Threads in Node
        -   Take breaks during longer computations
            -   `setTimeout` and `clearTimeout`
            -   `setInterval`
            -   Run to completion
-   Asynchronous patterns
    -   Events
    -   Callbacks
    -   Promises and `async...await`
-   Downsides of using asynchronous code
    -   Asynchronous code tends to be more verbose
    -   Asynchronous code is "infectious"
-   Asynchronous programming and runtime environments
    -   Asynchronous code depends on APIs provided by the runtime environment
    -   Different environments may have different APIs for similar tasks
    -   Browsers vs. Node

#### 38. The event pattern
-   Event-driven programming is reactive
-   Events as observables
-   Event observers
-   The event flow
    -   Subscribe
    -   Unsubscribe
    -   Notification
    -   Using events with callbacks
        -   DOM events
            -   The bad old days
            -   Things are better now
            -   `.addEventListener()`
            -   `.removeEventListener()`
            -   Preventing default actions
            -   Event propagation
            -   Creating your own events
                -   The Event constructor
                -   Subscribing and unsubscribing
                -   Dispatching the event
                -   Using CustomEvent to pass data with your event
                -   Propogating your event
                -   Dynamic event creation
            -   Programmatically triggering built-in events
        -   Node events
            -   Emitters and listeners
            -   Handling events with built-in modules
            -   The EventEmitter class
                -   Creating your own events
                -   Subscribing and unsubscribing
                -   Events with multiple callbacks
                -   Firing an event
                -   Make an event that only fires once
                -   Attaching data to your event
                -   Retrieving event listeners
-   Event-driven applications and reactive programming

#### 39. Using callbacks
-   Callbacks aren't always asynchronous
-   But sometimes they are
-   Callbacks and errors
-   Callback abstraction
-   Downsides of callbacks
    -   Lack of readability
    -   Callback Hell
-   Avoiding Callback Hell
    -   Keep it shallow
    -   Modularize
    -   Use more named and defined functions
    -   Handle all errors
    -   Rewrite with Promises
    -   Use `async...await`

#### 40. Making HTTP requests

-   A concise overview of HTTP
    -   The request/response cycle
    -   HTTP verbs
        -   GET
        -   POST
        -   PUT and PATCH
        -   DELETE
    -   Sending data and headers
    -   Anatomy of a response
-   Making HTTP requests in the browser
    -   The old way: `XMLHTTPRequest` and callbacks
    -   The new way: `fetch()` and Promises
-   HTTP requests with Node
-   Axios: a simpler way to make HTTP requests

#### 41. Better asynchronous functions with Promises

-   The Promise object
-   The basic Promise flow
    -   Similarities to the event pattern
    -   Resolved vs. rejected Promises
    -   Handle results with `.then()`
-   Promise's promises
    -   Better callback timing
    -   Callbacks added with `.then()` will even execute after success _or_ failure
    -   You can chain multiple callbacks that will execute sequentially by calling `.then()` multiple times

#### 42. Async/await for more readable code

#### 43. Asynchronous iterators and generators

-   Streams and lazy pushing/pulling
-   Pausing long computations
-   Communicating Sequential Processes (CSP)

#### 44. Creating your own task runners and queues for managing asynchronous operations

-   DIY
-   Async.js

#### 45. Processes, threads, and the event loop in detail

#### 46. Building applications: when and how to use (and _not_ use) asynchronous programming to call APIs, handle data, and manage state

**Project**

### VII. Software engineering in the real world: building full stack JavaScript applications

#### 47. Programming reactively with real-time data and streams

-   Observables and the observer pattern in more detail
-   Streams
-   Reactive libraries
    -   Bacon.js
    -   Rx.js
    -   Cycle.js
    -   Most.js
    -   xstream.js

#### 48. Programming the browser: `Window` and the Document Object Model

-   Build a component-based UI to abstract away DOM objects and manipulations with Riot.js

#### 49. Additional browser and Web APIs

#### 50. Programming for the server: applications and APIs with Node and Express

-   Express.js
-   Knex.js

#### 51.  Building a full-stack application with real-world data and users

### Appendix A. Important tools for modern developers

-   UI frameworks and libraries
-   Code linters, auto-formatters, and style guides
-   Editors and IDEs
-   Tools for testing and debugging
-   Version control and project management tools
-   Task runners and bundlers/build tools
-   Deployment and CI/CD tools
-   Static typing languages
