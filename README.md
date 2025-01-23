# Unexpected Type Coercion with Null in JavaScript Addition

This repository demonstrates a subtle bug in JavaScript related to type coercion and the handling of null values within an addition operation.  The issue arises from the loose comparison (`===`) within the conditional statement.  While seemingly straightforward, this can lead to unexpected behavior when dealing with null values and other data types.

## Bug Description

The `foo` function aims to add two numbers, returning null if either input is null.  The core problem lies in how JavaScript handles type coercion, particularly with loose equality comparisons.  This can cause incorrect results in certain edge cases.

## Solution

The provided solution implements stricter type checking using `typeof` to explicitly handle null values and avoid the unintended type coercion that leads to the error.  This ensures that the function behaves as expected in all cases.

## How to reproduce
1. Clone this repository.
2. Open `bug.js` to see the buggy code.
3. Run `bug.js` to observe the unexpected behavior.
4. Open `bugSolution.js` to see the corrected code.
5. Run `bugSolution.js` to see the expected behavior.