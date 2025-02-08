# Uncommon C Pointer Arithmetic Bug

This repository demonstrates a subtle bug related to pointer arithmetic in C.  The code appears simple, but its behavior can be unexpected, particularly with compiler optimizations or different system architectures. The bug is in the way the pointer is being used to modify the value of the variable and the lack of consideration to undefined behavior.

## Bug Description

The code initializes an integer variable 'x' and then uses a pointer 'ptr' to modify its value. While seemingly straightforward, there is a small chance of undefined behavior.

## How to Reproduce

1. Compile the code using a C compiler (e.g., gcc).
2. Run the executable.

## Solution

The solution file 'bugSolution.c' offers a correct way to modify x through the pointer, avoiding potential ambiguity.  