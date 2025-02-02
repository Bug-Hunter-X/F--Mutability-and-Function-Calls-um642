# F# Mutability and Function Calls

This example demonstrates a common issue in F# related to mutability and how functions handle mutable variables.  The core problem is that the `add` function calculates a sum using the values of `x` and `y` *at the time the function is called*. Subsequent changes to `x` and `y` do not affect the result of this calculation. 

The included code shows this behavior, and the solution demonstrates how to obtain a sum that reflects the most up-to-date values of `x` and `y`.