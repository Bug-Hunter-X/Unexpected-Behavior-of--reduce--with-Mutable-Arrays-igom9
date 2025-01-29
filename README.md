# Swift Reduce Unexpected Behavior

This example demonstrates an often-misunderstood aspect of the `reduce` function in Swift when used with mutable arrays. The `reduce` function operates on a copy of the array, not the array itself. Therefore, changes to the array after the `reduce` operation are not reflected in the result.

## Bug

The provided `bug.swift` code shows how the sum of an array remains unchanged even after adding elements to the array because the reduce was already performed on a copy. The solution demonstrates the correct way to handle this.

## Solution

The `bugSolution.swift` file presents a solution to obtain the updated sum after modifying the array.