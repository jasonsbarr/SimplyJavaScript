# Future tutorial outlines

Ok, so there is _no way_ I can manage writing the behemoth, 51-chapter project I originally outline, and I think I knew that when I was writing the outline.

Here's the rest of it so I have it for future reference if I continue the series beyond the introductory level, which I would very much like to do.

Some of this, especially materials related to built-in data structures, will need to go into the original now, but that's ok too.

## The rest of the outline

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
-   Handling events with Promises and streams

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
    -   Handle errors with `.catch()`
-   Promise's promises
    -   Better callback timing
    -   Using `.then()` as `finally`
    -   You can chain multiple callbacks that will execute sequentially by calling `.then()` multiple times

#### 42. Async/await for more readable async code

-   Promise chaining and readability
-   `async...await` makes asynchronous code look more like synchronous
-   Defining `async` functions
-   Calling `async` functions
-   `async` pitfalls and gotchas

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

#### 48. Programming the browser: `Window` and the Document Object Model

-   Build a component-based, reactive UI with modern state management principles

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
