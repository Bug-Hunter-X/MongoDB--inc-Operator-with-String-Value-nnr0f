# MongoDB $inc Operator with String Value
This repository demonstrates a common error when using the `$inc` operator in MongoDB: attempting to increment a field with a string value instead of a number.

The `bug.js` file shows the incorrect usage, resulting in an error.  The `bugSolution.js` file provides the corrected code.

## Problem
The `$inc` operator is designed to increment a numeric field.  Passing a string value leads to a data type error and prevents the update from working as intended. 

## Solution
Ensure the field you are incrementing is a number (integer or double) and the value used with `$inc` is also a number.