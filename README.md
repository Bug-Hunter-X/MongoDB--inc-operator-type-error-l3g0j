# MongoDB $inc Operator Type Error
This example demonstrates an incorrect usage of the MongoDB `$inc` operator, resulting in a type error. The `$inc` operator is designed to increment a numeric field by a specified value.  Using a string as the increment value will not work as expected. The solution involves ensuring the increment value is a number.

## Bug
The provided code attempts to increment the `field` by the string "1".  This will not increment the field correctly, and may even cause an error.

## Solution
The corrected code ensures that the increment value is a number by using the integer literal `1`.