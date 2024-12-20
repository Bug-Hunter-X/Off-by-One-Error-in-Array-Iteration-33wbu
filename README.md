# Off-by-One Error in Array Iteration

This repository demonstrates a common off-by-one error in Java that can lead to an `ArrayIndexOutOfBoundsException`.  The buggy code iterates one element beyond the array's valid index.  The solution provides the corrected code.

## Bug

The `BuggyArray.java` file contains the erroneous code. The `for` loop condition `i <= arr.length` is incorrect, as arrays are zero-indexed.  The last valid index is `arr.length - 1`.

## Solution

The `FixedArray.java` file contains the corrected code with the loop condition changed to `i < arr.length` to prevent the index out of bounds error.