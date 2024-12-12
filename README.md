# Go Slice Out of Bounds Error

This repository demonstrates a common Go error: an out-of-bounds error when iterating over a slice.

The `bug.go` file contains code with the error, and `bugSolution.go` provides a corrected version.

## Bug
The original code incorrectly iterates up to and including `len(a)` resulting in an index out of range error when accessing `a[i]`. 

## Solution
The solution modifies the loop condition to `i < len(a)`, ensuring that the loop terminates before accessing an index beyond the slice's valid range. 