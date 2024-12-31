# Unhandled Exception in Groovy Closure

This example showcases a common issue in Groovy where an exception thrown within a closure is not handled properly by the encompassing method. This can lead to unexpected program termination and make debugging more difficult.

The `bug.groovy` file contains the erroneous code, while `bugSolution.groovy` provides a corrected version demonstrating proper exception handling.

## How to Reproduce
1. Save the code in `bug.groovy`.
2. Run the script using a Groovy interpreter (e.g., `groovy bug.groovy`).
3. Observe that the program terminates prematurely before printing the final message. 

## Solution
The solution involves using a `try-catch` block within the `methodWithClosure` to handle the potential `RuntimeException`. 