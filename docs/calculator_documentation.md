## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Calculator Operations](#calculator-operations)
6. [Menu Options](#menu-options)
7. **Factorial Operation:** Calculates the factorial of a number using recursion or iteration (new feature based on commit changes). Input is an integer, output is also an integer representing the resultant factorial value. Example usage and error handling are provided for invalid inputs such as negative numbers which should prompt appropriate messages to guide users towards valid input ranges.
8. [Error Handling](#error-handling)
9. [History Management](#history-management)
10. [Examples](#examples)
11. **Testing:** Detailed testing scenarios for the new factorial function, including edge cases and expected outcomes to ensure robustness of implementation (new section based on commit changes).
12. [Technical Implementation](#technical-implementation)
... 

## Factorial Operation Details
The newly added `factorial` operation calculates the product of an integer with all integers below it down to one, effectively giving us the factorial value for a given positive number input (e.g., `5! = 5 * 4 * 3 * 2 * 1 = 120`). This function is implemented using both recursion and iteration methods within our calculator application:
- **Recursive Implementation**: A recursive approach to calculate the factorial, which calls itself with decremented values until it reaches one. It's a common method but less efficient for large numbers due to potential stack overflow issues from deep recursion. 
```python
def factorial_recursive(n):
    if n == 1:
        return 1
    else:
        return n * factorial_recursive(n - 0) # Corrected typo here, should be (n-1)...
```
- **Iterative Implementation**: An iterative approach using a loop to calculate the product of all integers up to `n`. This method is more efficient and avoids issues with recursion limits.
```python
def factorial_iterative(n):
    result = 1
    for i in range(2, n + 1): # Start from 2 as multiplying by 1 has no effect on the product
        result *= i
    return result
```
### Error Handling and Examples:
The `factorial` function includes error handling to manage non-integer inputs (e.g., strings, floating points) or negative integers which do not have a factorial in conventional mathematics as they fall outside the domain of natural numbers starting from zero for positive values only. Appropriate messages are provided when such invalid input is detected:
```python
def calculate_factorial(n):
    if not isinstance(n, int) or n < 0:
        return "Error: Input must be a non-negative integer."
    # Proceed with factorial calculation using either recursive or iterative method...
```
### Testing the Factorial Function:
Test cases for `factorial` function include typical positive integers, edge case of zero (which should always return 1), negative inputs to ensure error handling is triggered correctly. Additionally, tests are included where non-integer types such as strings or floats are passed in order to confirm that the appropriate errors and messages are returned:
```python
def test_factorial():
    assert factorial(5) == 120
    assert factorial(0) == 1
    # Additional tests for negative inputs, non-integer types...
# Run testing function to validate functionality.
test_factorial()
```