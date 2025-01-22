# JavaScript Bug: Null Arguments in Addition Function

This repository demonstrates a subtle bug in a JavaScript function designed to add two numbers. The function unexpectedly returns 0 when one or both of its arguments are null. This behavior might not be immediately obvious and can lead to unexpected results in applications.

## Bug Description

The `foo` function is intended to add two numbers. However, if either or both of the input arguments are `null`, it returns 0. This is a potential source of errors if the function is used with values that might be null or undefined. 

## Solution

The solution involves adding explicit null checks to handle the case where the arguments might be null. The updated function checks for null values and returns NaN if any input is null, providing a more appropriate and clear indication of an invalid input condition. 

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` in your preferred JavaScript environment.
3. Run the code. Observe the unexpected output where it returns 0 for null input.
4. Examine `bugSolution.js` to see the corrected function.