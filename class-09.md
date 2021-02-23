# Class 9

* ##  Functional Programming Concepts
What is Functional Programming?

Functional programming is a specific way to look at problems and model their solutions. Pragmatically, functional programming is a coding style that exhibits the following characteristics:


* * Power and flexibility. We can solve many general real-world problems using functional constructs

* * Simplicity. Most functional programs exhibit a small set of keywords and concise syntax for expressing concepts

* * Suitable for parallel processing. Via immutable values and operators, functional programs lend themselves to asynchronous and parallel processing.

In functional programming, programs are executed by evaluating expressions, in contrast with imperative programming where programs are composed of statements which change global state when executed. Functional programming typically avoids using mutable state. Everything is a mathematical function. Functional programming languages can have objects, but generally those objects are immutable -- either arguments or return values to functions. There are no for/next loops, as those imply state changes. Instead, that type of looping is performed with recursion and by passing functions as arguments.


* ##  Refactoring Javascript for Readability

After a few years working almost exclusively with Ruby on Rails and some jQuery, I changed my focus to front-end development. I discovered the beauties of JavaScript ES6 syntax and the exciting modern libraries such as React and Vue. I started to implement new features using nothing but ES6 Vanilla JavaScript, and fell instantly in love with all this new class abstraction and those arrow functions.

Nowadays, I’m generating large amounts of JavaScript code. But, since I consider myself a JavaScript Padawan, there’s yet a lot of room for improvement. Through my studies and observations, I’ve learned that even with the use of syntactic sugars featured in ES6, if you don’t follow the main principles of SOLID, your code has a high chance of becoming complex to read and maintain.

To demonstrate what I’m talking about, I’ll walk you through one fantastic Code Review session I had last week with a buddy of mine. We are going to start with a 35-lines JavaScript Class and will finish with a beautiful 11-lines code piece using only slick functions. With patience and resilience, you will be able to observe and apply the pattern to your own codebase.