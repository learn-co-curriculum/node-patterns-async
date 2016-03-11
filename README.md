# Async Library

## Overview

It's possible to implement concurrency with just vanilla Node.js, but the code is not very easy to read or maintain. There are better ways of course. One of the ways is to use `async` which is an npm package for asynchronous code management (Control Flow).

This lesson will cover the most common `async` usage and illustrate (code along) the refactoring of the concurrency implementation.

## Objectives

1. Introduce the async library
1. Refactor previous lab solution using the async lib

## Async Library

To install `async`, you'll need to add the library to your `package.json` in the `dependencies`:

```
  "dependencies": {
    "async": "1.5.2"
  }
```

Then, run npm installation:

```
npm i
```

Now you are ready to use `async` in your Node scripts like this:

```js
var async = require('async')
async.NAME
```

The NAME is the method name which you want to use. The main methods in `async` are control flow methods. They allow to manage asynchronous code:

* `series`: Run multiple functions in sequential order, one after another
* `parallel`, `parallelLimit`: Run multiple function in parallel/concurrent manner
* `whilst`, `doWhilst`: Repeatedly call function when condition is true (akin to `while`)
* `until`, `doUntil`: Inverse of whilst.
* `during`, `doDuring`: Like `whilst` only take asynchronous function as condition while `whilst` take synchronous function (i.e., expression)
* `forever`
* `waterfall`
* `compose`
* `seq`
* `applyEach`, `applyEachSeries`
* `queue`, `priorityQueue`
* `cargo`
* `auto`
* `autoInject`
* `retry`
* `iterator`
* `times`, `timesSeries`, `timesLimit`
* `race`

## Resources

1. []()
1. []()
1. []()


---

<a href='https://learn.co/lessons/node-patterns-async' data-visibility='hidden'>View this lesson on Learn.co</a>
