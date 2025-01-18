# MongoDB $inc Operator Error

This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The error arises from providing a string value instead of a numeric value for the increment.

## Bug Description
The original code attempts to increment a field by '1' (a string). This results in the update failing or having unexpected results.  The `$inc` operator requires a numeric value.

## Solution
The solution involves changing the increment value from a string to a number. This corrected code ensures the field is incremented correctly.

## How to Reproduce
1. Clone this repository.
2. Ensure you have a MongoDB instance running.
3. Create a collection named 'myCollection' and insert at least one document with an `_id` of 1 and a field to increment.
4. Run the bug.js script to observe the incorrect behavior.
5. Run the bugSolution.js script to observe the correct behavior.