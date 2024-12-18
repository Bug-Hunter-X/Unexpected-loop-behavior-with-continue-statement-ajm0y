# Unexpected Loop Behavior with Continue Statement in C

This repository demonstrates a subtle bug in a C program involving a `continue` statement within a `while` loop.  The program's intention is to print numbers 1 through 10, skipping 5. However, due to the placement of the `continue` statement, the output is unexpected.

## Bug Description

The `continue` statement prematurely terminates the current iteration of the loop, but the increment operation (`i++`) is still performed. This leads to a value being skipped in the output.  The program does not produce the expected output of 1, 2, 3, 4, 6, 7, 8, 9, 10.  Instead, it skips a different value.

## Solution

The solution involves re-arranging the code to ensure correct behavior of the continue statement within the loop.  The corrected program now produces the expected output.

## How to Reproduce

1. Clone the repository.
2. Compile `bug.c` using a C compiler (e.g., gcc).
3. Run the compiled executable.  Observe the incorrect output.
4. Compile `bugSolution.c` and run it to observe the corrected output.
