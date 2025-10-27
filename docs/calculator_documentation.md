## Calculator Application Documentation - Version Updated with Factorial Operation Feature

The Python-based command-line calculator application now includes a factorial operation feature, as per recent commit changes by bluepal-nipun-marwaha on April 15, 2023. This addition enhances the functionality of our Calculator Application to not only provide basic arithmetic operations but also advanced mathematical computations like calculating the factorial of numbers.

### Table of Contents (Updated)

1. [Overview](#overview)
2. [Features](#features)
   - Basic Arithmetic Operations: Addition, subtraction, multiplication, division
   - Advanced Operations: Power/exponentiation and Factorial Operation
3. [Installation](#installation)
4. [Usage](#usage)
5. [Calculator Operations (Updated Section)](calculator-operations#factorial-operation)
6. [Menu Options](#menu-options)
7. [Error Handling](#error-handling)
8. [History Management](#history-management)
9. [Examples](#examples)  # New section for examples with factorial operation included
10. [Testing](#testing)

## Overview (Updated Section)
The Calculator Application is a Python-based command-line calculator that provides basic arithmetic operations, advanced mathematical computations including power/exponentiation and the newly added factorial operation feature along with an interactive interface for user convenience. The application also includes calculation history tracking to view all previous calculations made by users as well as comprehensive error handling mechanisms in place for invalid inputs or division-related errors.

## Calculator Operations (Updated Section)
The calculator supports the following operations:
- Addition, subtraction, multiplication and division of two floating point numbers with appropriate input validation to handle non-numeric entries gracefully. 
- Power/exponentiation operation which raises a number to an exponent provided by the user as inputs. The function ensures that both operands are numeric values before performing calculations. Error handling is in place for invalid or zero exponents, providing informative error messages and preventing crashes of application flow.
- Factorial Operation: Calculates the factorial of a non-negative integer input by users using recursion to provide accurate results within its defined scope (non-negative integers only). The function includes appropriate checks against negative inputs with an understandable user prompt for valid entries, along with error handling mechanisms in place.

## Menu Options (Updated Section)
Here are the updated menu options that now include a factorial operation:
```markdown
=== Sheet: Menu Options ===
Option Number | Option Name       | Function                         | Input Required                | Output        | Example    | Error Handling
1            | Addition          | Adds two numbers               | Two floating-point numbers   | Sum of the numbers  | 5.5 + 3.2 = 8.7 | Handles invalid input gracefully
...           # Existing options remain unchanged here for brevity in this example ...
10            | Factorial         | Calculates factorial             | Non-negative integer          | Result of the calculation   | `5!` (factorial) = 120    | Handles invalid input gracefully, non-integer inputs with an understandable user prompt for valid entries. Error handling mechanisms in place to prevent crashes and provide informative error messages when encountering negative integers or other unsupported types of inputs.
```
## History Management (Updated Section)
The application now tracks all calculations performed by users including the newly added factorial operation, providing a comprehensive history management feature for user reference on past computations made within this calculator tool. 

## Examples (New Section Added)
Here are some examples of how to use each menu option in our Calculator Application:
```markdown0
Example Addition Operation: Entering `5 + 3` yields an output of `8`. Invalid inputs, such as strings or negative numbers will trigger error handling and prompt the user for valid numeric entries.
...                         # Existing examples remain unchanged here for brevity in this example ...
Factorial Example (New): For calculating a factorial operation like entering `5!` yields an output of `120`. Non-integer inputs or negative numbers will trigger error handling and prompt the user to enter valid non-negative integer entries. 
```
## Testing (Updated Section)
The testing section has been updated with additional test cases for our new factorial operation feature, ensuring robustness in its functionality across a variety of input