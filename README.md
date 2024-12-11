# MongoDB $inc operator error with String field

This repository demonstrates an example of an uncommon error in MongoDB related to the misuse of the `$inc` operator.

The `$inc` operator is used to increment a numeric field in MongoDB. Attempting to use it on a string field leads to an error.

## Bug
The `bug.js` file shows an example of incorrect usage of the `$inc` operator where we try to increment a string field. 

## Solution
The `bugSolution.js` file provides the corrected code. Before using `$inc`, ensure that the target field is of numeric type (int, long, double). If your field is a string representing a number, you must first convert it to a numeric type before performing any arithmetic operations.
