# Understanding programs, algorithms, and data

In article 0,[^1] [Getting started with computing, computers, and computer science](./0-getting-started.md), I mentioned programming a few times. In this article I'll discuss a bit about what exactly programming is, how programming and programming languages work, characteristics of different programming languages, and how to start programming in JavaScript.

## What is a program?

At its most basic level, a program is a piece of written language that tells the computer to perform a computation. How exactly a program is written depends on the language, the programmer's style, and in some cases the machine the program is written for.

### Imperative vs. declarative programming styles

A program may go into great detail about exactly _how_ the computer should solve the problem in a step-by-step manner, or it can be written more to tell the computer _what_ to do and trust the computer itself to apply the proper steps.

The former is called **imperative** programming style; the latter is known as a **declarative** style.

Here's an imperative program that gets the even values from a list of numbers.

#### Example 1: imperative JavaScript

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const imperativeFilter = numbers => {
  const evens = [];

  for (let i = 0; i < numbers.length; i += 1) {
    // % is the modulo operator, which gives you the
    // remainder from dividing its first argument
    // by its second argument. If a number is
    // divisible by a second number, the
    // result will be zero.
    if (numbers[i] % 2 === 0) {
      evens.push(numbers[i]);
    }
  }

  return evens;
}
```

Now here's a program that does the same thing, but in a declarative style.

#### Example 2: declarative JavaScript

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const declarativeFilter = numbers => {
  // Defining the helper function isn't strictly
  // necessary, but I wanted to make the steps
  // of the function as explicit as possible
  // so it's easier to read and understand.
  const isEven = number => number % 2 === 0;
  return numbers.filter(isEven);
}
```

Even if you don't understand exactly how each of these programs work just yet, you can probably still see how the declarative program is simpler to read and understand than the imperative one.

The second program also the advantage of using **immutable data**, which means the data structures you define in your program do not change.

We'll see why that's a good thing later.

### The declarative trend

Declarative style is a rising trend right now, but that doesn't necessarily mean it's _better_ than imperative programming.

A good programmer knows how to use either style or a mix of the two depending on what a given situation requires.

Since declarative programming is such a big deal right now, I'm going to take extra care in making sure you understand how to read and write programs written in that style.

By the time we're finished you should be equally fluent in each paradigm.

### Programs, computation and algorithms

Programs are where the [systematic problem solving](./1-computers-programming-and-javascript/0-getting-started.md#systematic-problem-solving) aspect of computer science meets the practical needs of programmers and the people who benefit from programming in all areas of life.

Programming and algorithms, [the "recipes" that tell a computer what to do to perform a computation](./0-getting-started.md#algorithms-and-thinking-algorithmically), go hand-in-hand. Programming a computer often involves either coming up with a new algorithm to solve a problem or applying one someone else has designed.

We will revisit the topic of how to both design algorithms and interpret them for effectiveness and efficiency several times throughout this series.

Improving algorithm efficiency is a crucial part of programming and something computer scientists spend much of their time doing.

<hr>

### Notes

[^1]: In most programming languages, counting starts from zero instead of one.
