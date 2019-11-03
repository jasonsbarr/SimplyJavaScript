## Programs and algorithms

Programs are where the [systematic problem solving](./1-computers-programming-and-javascript/0-getting-started.md#systematic-problem-solving) aspect of computer science meets the practical needs of programmers and the people who benefit from programming in all areas of life.

Programming and algorithms, [the "recipes" that tell a computer what to do to perform a computation](./0-getting-started.md#algorithms-and-thinking-algorithmically), go hand-in-hand. Programming a computer often involves either coming up with a new algorithm to solve a problem or applying one someone else has designed.

We will revisit the topic of how to both design algorithms and interpret them for effectiveness and efficiency several times throughout this series.

Improving algorithm efficiency is a crucial part of programming and something computer scientists spend much of their time doing.

### The 3 parts of an algorithm

## Control flow: conditional branching

### Boolean operators and control flow

## Input, output, and processing data

## Data and program state

## Imperative vs. declarative programming styles

A program may go into great detail about exactly _how_ the computer should solve the problem in a step-by-step manner, or it can be written more to tell the computer _what_ to do and trust the computer itself to apply the proper steps.

The former is called **imperative** programming style; the latter is known as a **declarative** style.

For the first example, here's an imperative program that gets the even values from a list of numbers.

#### Example 1: imperative JavaScript

This example uses the modulo arithmetic operator (`%`), which gives you the remainder from dividing the first number by the second. If the first is divisible by the second, the result will be zero.

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

const evens = [];

for (let i = 0; i < numbers.length; i += 1) {
  if (numbers[i] % 2 === 0) {
    evens.push(numbers[i]);
  }
}

console.log(evens);
```

Now here's a program that does the same thing, but in a declarative style.

#### Example 2: declarative JavaScript

Defining the `isEven` function isn't actually necessary, but I wanted to make what's going on here more explicit for the reader.

```javascript
const numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const isEven = number => number % 2 === 0;

const evens = numbers.filter(isEven);

console.log(evens)
```

Even if you don't understand exactly how each of these programs work just yet, you can probably still see how the declarative program is simpler to read and understand than the imperative one.

The second program also the advantage of using **immutable data**, which means the data structures you define in your program do not change.

We'll see why that's a good thing later.

### The declarative trend

Declarative style is a rising trend right now, but that doesn't necessarily mean it's _better_ than imperative programming.

A good programmer knows how to use either style or a mix of the two depending on what a given situation requires.

Since declarative programming is such a big deal right now, I'm going to take extra care in making sure you understand how to read and write programs written in that style.

By the time we're finished you should be equally fluent in each paradigm.
