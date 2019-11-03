# Working with data and types

The basic task of any program is to do some kind of transformation with **data.**

Data is a symbol or collection of symbols that are given meaning by specific acts of interpretation.

This is a bit of a philosophical definition, but it's necessary in this case: in order to use data it must be given meaning in some way so a program (or, indeed, a human) knows how to use it.

## Data types

Programming languages classify data according to **data types.** A data type tells the computer how to work with a bit of data under the hood.

For example, data types make sure it doesn't try to work with words as if they were numbers.

## Built-in JavaScript data types

JavaScript has several built-in data types. We'll start with 3 of them: Numbers, Strings, and Booleans.

These are known as **primitive data types,** which are the basic building blocks of data in JavaScript. Later we'll also look at complex data types.

If you did the exercises for the previous chapter, you've already seen the 3 types in action. Now I'll explain them in greater detail.

If you didn't, go do them now and then come back here.

### Numbers and arithmetic

Unlike other languages, JavaScript uses one **Number** type for both integers and floating-point numbers.[^1]

**Integers** are just regular numbers like the ones you count with that don't evaluate to fractions.

They include positive whole numbers, negative numbers, and zero.

**Floating-point numbers** are written like and work in the same way as decimals, but the underlying representation is in binary.

This can lead to some interesting quirks since things that are evenly divisible with decimal numbers might not be with binary numbers.

_Follow along by typing the examples into your console_

#### Example 1: floating-point rounding error

```javascript
// Should be 0.9
0.3 * 3; //-> 0.8999999999999999
```

The most basic numeric operation is arithmetic. You can use arithmetic operators in JavaScript just like you'd expect:

#### Example 2: JavaScript arithmetic

```javascript
10 + 3; //-> 13
21.7778 - 3.2; //-> 18.5778
17 * 22.7; //-> 385.9
100 / 2; //-> 50

// Note floating-point rounding weirdness
100 / 3; //-> 33.333333333333336
```

There's also a 5th arithmetic operator, the `modulo` (%). It takes 2 numbers and returns the remainder from dividing the first by the second.

#### Example 3: The `modulo` operator

```javascript
9 % 3; //-> 0
9 % 4; //-> 1
```

A common way to use the `%` operator is to check if a number is divisible by another number. If it is, the `return` value will be `0`.

#### Example 4: Checking if a number is even

```javascript
3 % 2; //-> 1, so it's not even
10 % 2; //-> 0, so it's even
```

### Strings

A String is simply text data. Strings need to be enclosed in quotes. You can use double-quotes:

#### Examples 5-7: JavaScript strings

```javascript
"This is a string"
```

single-quotes:

```javascript
'So is this';
```

or backticks:

```javascript
`This is too`;
```

Strings defined with backticks can span multiple lines:

#### Example 8: Multi-line strings

_Use `CTRL+ENTER` to enter a line break without making the interpreter try to evaluate an incomplete expression_

```javascript
`
This is a string
that spans across
multiple
lines
`;
```

You can also do some pretty neat things with backtick strings that we'll talk about in future chapters.

You can use both the `+` and `*` operators with strings. This is called **operator overloading.**

#### Example 9: Overloaded operators

```javascript
"My name is" + " Jason " + "Barr.";
//-> "My name is Jason Barr.

"JavaScript is fun!" * 3; // Note the lack of a space between repeats
//-> "JavaScript is fun!JavaScript is fun!JavaScript is fun!"
```

### Booleans

Booleans are simply `true` or `false` values. It may not seem like much, but they're one of the most useful concepts in programming.[^2]

It's rare that you'll work with Booleans directly in their raw `true` and `false` form. The most common use for Booleans is to evaluate expressions for **truthiness** or **falsiness** to determine the flow of a program or another conditional operation.

We'll look more at Boolean logic and expressions in the next chapter.

## Binding data to names: constants and variables

A binding applies a valid name to a value so the value can be used later in the program.

Bindings can be either constant, where the binding cannot be changed once assigned, or variable, where it can.

Valid names in JavaScript start with a dollar sign ($), underscore (_), or letter and may contain both those characters and numbers.

#### Example 11: valid and invalid names

```javascript
// Valid names
hello
_startsWithUnderscore
CapitalLetter
$dollarDollarBill

// Invalid names
123_this_is_wrong
so's_this
%nopeNotThis
```

### Naming Conventions

Most of the time in JavaScript code you'll see names written either with camelCase or PascalCase.[^3]

Sometimes you'll see names written in snake_case, which uses underscores to separate words.

Still other times you'll see names written with ALL_CAPS_SNAKE_CASE, usually by old-school C programmers to denote constant values. As you will soon see, I recommend using constant values exclusively whenever possible, so I don't use any special convention for constants vs. variables.

### The difficulty of naming things

It may not seem like it now, but deciding what to name things in your program is often one of the most difficult things you'll have to do.

It usually works best if you use names that describe what the data is and does.

Instead of `x` use `number`. Instead of `str` for a String, use `firstName` or another descriptive name.

### Assignment expressions

An assignment expression simply uses a single equals sign (=) to bind the value on the right side to the name on the left.

It starts with either the keyword `const` for a constant binding or `let` for a variable.[^4]

### Variables, constants, and (im)mutability

I use `const` almost exclusively for bindings in my own programs because having bindings that don't change makes it so that, at least with simple data types, you can always know what value a name refers to without having to read through the whole program.

Programs that mutate a binding's value are more difficult to read and understand than those that use constant values.

Data bindings that can't be changed are **immutable.** Primitive data types are immutable by definition, which makes sense because, for example, the numbers 8 and 12 will always be different numbers no matter what names they are bound to.

Complex types require more work to make them immutable. We'll see more about that in chapter 4.

You should use constant, immutable data whenever possible.

#### Example 12: Simple bindings

```javascript
// Constant binding expressions
const firstName = "Jason";
const lastName = "Barr";
const fullName = firstName + " " + lastName;

// Variable binding expression;
let number = 3;

// You can use previous bindings in a current one
let sum = number + 18; //-> 21

// Variable bindings can be reassigned
number = 10;

// Reassigning a variable doesn't affect its earlier use
console.log(sum); //-> still 21
```

The `fullName` constant can be defined more cleanly with a backtick String, also known as a **template literal,** which allows you to interpolate values and expressions using `${}`:

#### Example 13: Using a template literal

```javascript
const fullName = `${firstName} ${lastName}`;
```

I always use template literals when using values in strings, but you'll see interpolation with `+` especially in older code, as template literals weren't officially part of JavaScript until 2015.[^5]

You can also assign the value of an expression to a name. This can be any expression, including an arithmetic operation, a function, or any other expression.

#### Example 14: Assigning expressions

```javascript
const sum = 15 + 10; //-> 25
const intPi = parseInt(Math.PI) //-> 3
const value = 5 + (2.9 * 4.2) / 3.14; //-> 8.878980891719745
```

## Try it yourself: exercises for further learning

1. Assign a numeric value to a constant `number` that uses the most complicated, gnarly arithmetic operation you can think of. See if you can use all 5 operators!
2. Assign your first and last names to two separate constants. Don't use a space in either binding. Use them to assign your full name to its own constant using `+` to join them (don't forget the space!).
3. Now assign them using a template literal. Don't forget: you can't re-assign values to a constant!
4. Think of a name and value you might want to use as a binding in a program. Type the name by itself into the console. Use `CTRL+ENTER` to insert a line break and use it in an assignment expression on the second line. Now hit `ENTER`. What happens? Is it what you expected?
5. What problems do you think mutating a variable's value in a program could cause?

### Notes

[^1]: There is a new `BigInt` data type proposal, but it is not yet part of the JavaScript standard as of November 2019.

[^2]: Booleans are named after the English mathematician, philosopher, and logician [George Boole](https://en.wikipedia.org/wiki/George_Boole). Boole made the first formulation of what is now known as Boolean Algebra, which measures truth and falsity based on conjunction (_and_), dysjunction (_or_), and negation (_not_) and forms the logical basis of modern computing.

[^3]: Confusingly, sometimes people will refer to UpperCamelCase and lowerCamelCase.

[^4]: There is also the `var` keyword, which was originally the only way way to bind variables in JavaScript, but you shouldn't use it anymore. You'll see it in the wild, mostly in older code, so you need to know what it is, but it's never necessary or desirable to use it anymore because it has some really annoying quirks I will go into in a later chapter. For now all you need to know is _always_ use `const` when possible, and when it's not use `let`.

[^5]: From now on I'll use either **ES6+** or the year a feature was added (e.g. **ES2015**) to describe language features added to JavaScript since 2015 when regular updates to the standard began. **ES** stands for **ECMAScript,** named after ECMA, the standardizing body for JavaScript. ECMAScript is the official name of the standardized JavaScript language. We'll discuss that more when we go over the history of JavaScript in a future chapter.