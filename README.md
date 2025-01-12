# Unexpected Behavior with $inc and Negative Values in MongoDB

This example demonstrates a potential issue when using the `$inc` operator with a negative value in MongoDB's `updateOne` method. If the target field does not exist, the update operation doesn't throw an error, resulting in the value being set to the negative increment instead of properly decrementing from an existing value.