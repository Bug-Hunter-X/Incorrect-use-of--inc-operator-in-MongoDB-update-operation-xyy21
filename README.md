# Incorrect use of $inc operator in MongoDB update operation
This example demonstrates an error that can occur when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numeric field by a specified value.  However, if a string is provided instead of a number, the result will be unexpected, the string will be appended instead of the numeric increment.

**Bug:**
The provided code attempts to increment the `count` field by 1. However, because the increment value is a string, the string will be added to the field instead of incrementing the numeric value.

**Solution:**
Ensure that the value you provide to the `$inc` operator is a number.  This can be easily done by changing the increment value to a numeric type.
