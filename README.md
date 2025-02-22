# JavaScript Loose Equality Bug

This repository demonstrates a common JavaScript bug related to loose equality (==) when checking for null or undefined values.  The loose equality operator does not distinguish between different falsy values (0, "", false, null, undefined) and can lead to unintended errors.

## Bug Description

The `foo` function in `bug.js` throws an error if `a` or `b` are null.  However, it incorrectly throws an error for other falsy values.

## Solution

The `bugSolution.js` file shows the improved code using strict equality (===) to correctly identify null and undefined values, preventing unintended error triggers.

## How to Reproduce

1. Clone this repository.
2. Run `bug.js` with different values for `a` and `b`, including null, 0, "", false, and other values.
3. Observe the error behavior with loose equality and compare it to the correct behavior in `bugSolution.js`.

This example highlights the importance of using strict equality when dealing with null or undefined values in JavaScript to prevent these subtle yet significant errors.