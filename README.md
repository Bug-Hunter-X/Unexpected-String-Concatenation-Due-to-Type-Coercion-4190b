# Unexpected String Concatenation in JavaScript

This repository demonstrates a common yet subtle bug in JavaScript related to type coercion.  The `foo` function intends to add two numbers, but due to the implicit type conversion of JavaScript, it performs string concatenation when one of the operands is a string.

## Bug Description

The JavaScript interpreter's behavior when performing addition involving different data types can lead to unexpected results. In this case, passing a number and a string to the `foo` function results in string concatenation instead of numerical addition.

## Solution

The solution involves explicitly converting both arguments to numbers using `Number()` before performing the addition. This ensures consistent numerical behavior regardless of the input types.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Open `bug.js` to view the buggy code.
4. Open `bugSolution.js` to view the corrected code.
5. Run both files using a JavaScript interpreter (like Node.js) to see the different outputs.