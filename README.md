# Stack Overflow in Recursive Factorial Function

This repository demonstrates a common error in recursive functions: stack overflow. The `foo` function calculates the factorial recursively.  For large inputs, the recursive calls consume too much stack space leading to a crash. The solution demonstrates using an iterative approach to avoid this issue.

## How to reproduce

1. Clone this repository.
2. Compile and run `bug.hack` using the HHVM compiler.
3. Observe the stack overflow error for sufficiently large input values (e.g., `foo(10000)`).
4. Run `bugSolution.hack` which shows the iterative solution which fixes the problem.

## Solution

The solution involves replacing the recursive approach with an iterative one. This avoids the unbounded stack growth associated with recursion, making the function robust to large inputs.