# MongoDB $inc Operator Error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The error arises from providing a string value instead of a number to the `$inc` operator, leading to incorrect updates.

The `bug.js` file shows the incorrect usage, resulting in the age field not being incremented as expected. The `bugSolution.js` file provides the correct implementation.

## How to reproduce

1.  Set up a MongoDB instance.
2.  Create a collection (e.g., `users`).
3.  Insert a document (e.g., `{name: "John", age: 30}`).
4.  Run the code in `bug.js`. 
5.  Observe that the age is not updated correctly.
6.  Run the code in `bugSolution.js` to see the correct update.

## Solution
Ensure that you pass a numerical value to the `$inc` operator.