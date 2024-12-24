# TypeScript Implicit 'any' Type Bug

This repository demonstrates a common TypeScript bug: the implicit use of the `any` type in function parameters.

## Bug Description

The `greet` function in `bug.ts` takes a `Date` object as a parameter. However, TypeScript does not explicitly enforce this type, leading to potential runtime errors if an invalid value is passed. This is because the type is implicitly 'any' if not explicitly defined.

## Solution

The `bugSolution.ts` file shows the corrected code.  By explicitly defining the parameter type, TypeScript can perform type checking and prevent unexpected behavior.

## How to Reproduce

1. Clone this repository.
2. Open `bug.ts` and `bugSolution.ts`.
3. Compile and run the code in both files to observe the difference in behavior.

This example highlights the importance of explicitly specifying types in TypeScript to catch errors at compile time rather than runtime.