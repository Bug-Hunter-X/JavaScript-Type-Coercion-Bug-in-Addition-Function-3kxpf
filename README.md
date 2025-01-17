# JavaScript Type Coercion Bug

This repository demonstrates a subtle bug in a JavaScript function that involves type coercion. The `foo` function is designed to add two numbers but fails when it encounters null values or values that are not numbers.

## Bug Description

The `foo` function correctly handles numerical addition. However, it uses loose comparison (`===`) which can lead to unexpected results when the input values are of different types or are null, causing type coercion that leads to incorrect output. This can be difficult to debug without a thorough understanding of JavaScript's type system.

## Bug Solution

The solution includes explicit type checking and handling, preventing type coercion issues and ensuring the function behaves as expected. The improved code handles null values gracefully and performs strict type checking before attempting addition.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` to observe the erroneous behavior.
3. Open `bugSolution.js` to see the correct implementation.