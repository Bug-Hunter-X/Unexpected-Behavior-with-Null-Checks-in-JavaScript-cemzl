# Unexpected Behavior with Null Checks in JavaScript

This repository demonstrates a common error in JavaScript related to null checks and loose equality. The `foo` function attempts to handle null values, but its implementation uses loose equality (`==`) which can produce unintended results.

## The Bug
The `bug.js` file contains a function that attempts to add two numbers but returns 0 if either number is null. However, due to the use of loose equality, the function incorrectly handles all cases of null values. 

## The Solution
The `bugSolution.js` file provides a corrected version of the function which utilizes strict equality (`===`) to correctly identify and handle null values. Strict equality is recommended when comparing against null or undefined to avoid unintentional type coercion and unexpected outcomes.

## How to Run
1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in a JavaScript environment or browser console.
3. Observe the differing outputs to understand the effect of using loose vs. strict equality.