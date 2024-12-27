# JavaScript Loose Typing Bug
This example demonstrates an unexpected behavior in JavaScript due to its loose typing system. The `+` operator's behavior changes depending on the data types of its operands.  When adding a number and a string, it performs string concatenation instead of numerical addition, which can lead to subtle and hard-to-find errors.

## Bug Description
The function `foo` intends to add two numbers. However, if one of the inputs is a string, it will concatenate the values instead of adding them numerically.  This is counterintuitive for developers expecting standard mathematical addition.

## Solution
The solution involves explicitly converting both operands to numbers before performing the addition using `Number()`.