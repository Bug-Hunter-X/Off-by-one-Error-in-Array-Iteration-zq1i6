# Off-by-one Error in Array Iteration

This repository demonstrates a common off-by-one error in Java when iterating through arrays. The error occurs when the loop condition incorrectly includes the last index, causing an `ArrayIndexOutOfBoundsException`.

## Bug Description

The `Bug.java` file contains a `for` loop that iterates through an integer array. The loop condition `i <= arr.length` is incorrect because array indices start from 0 and end at `length - 1`.  This leads to an attempt to access an element beyond the array's bounds.

## Bug Solution

The `BugSolution.java` file corrects this error by changing the loop condition to `i < arr.length`. This ensures that the loop iterates only through valid array indices.

## How to Run

1. Clone this repository.
2. Compile and run `Bug.java` to see the exception.
3. Compile and run `BugSolution.java` to see the corrected output.