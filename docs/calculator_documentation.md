## Calculator Application Documentation - Version Updated with Factorial Operation Feature

---

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Calculator Operations](#calculator-operations)
6. [Menu Options](#menu-options)
7. [Error Handling](#error-handling)
8. [History Management](#history-management)
9. [Examples](#examples)
10. [Testing](#testing)

## Overview
The Calculator Application is a Python-based command-line calculator that provides basic arithmetic operations with an interactive menu, comprehensive error handling, and now includes the new factorial operation feature for calculating large numbers efficiently using recursion or iterative methods. The application also tracks calculation history to review past computations easily. 

## Features
- **Basic Arithmetic Operations**: Addition, subtraction, multiplication, division
- **Advanced Operations**: Power/exponentiation and Factorial Operation (calculates the factorial of a number)
- **Calculation History**: Track and view all previous calculations including new operations like factorials. 
- **Error Handling**: Graceful handling of invalid inputs, division by zero errors with appropriate messages for user guidance.
- **Interactive Menu**: Easy-to-use command-line interface to select the desired operation from a list or enter custom calculations including complex expressions and factorials. 
- **History Management**: Maintain an accessible log of all operations performed, providing users with quick recall for past results without repetitive input.

## Installation
(Installation instructions remain unchanged.)

## Usage
(Usage guide remains mostly the same but includes guidance on using factorial operation and accessing history management features.)

## Calculator Operations
- (Existing operations descriptions with addition, subtraction, multiplication, division now include new sections for power/exponentiation and Factorial Operation)
  - **Factorial Operation**: The application can calculate the factorial of a number using either recursive or iterative methods. For example, `5!` (factorial of 5) is calculated as `5 * 4 * 3 * 2 * 1 = 120`.
- Factorials are handled efficiently and memory usage optimized for large numbers to prevent stack overflow errors in recursive approaches or manage long computation times with iterative methods.

## Menu Options (Updated)
(Existing menu options now include the factorial operation.)
6 | Calculate Factorial | Computes the factorial of a number using recursion/iteration method provided by user choice, Input Required: Number to calculate its factorial Output Displayed as 'Result' or Error Message if invalid input is given. Example for 5! would be displayed as "The factorial of 5 is 120".

## Error Handling (Updated)
- The error handling section now includes messages specific to the new operations, such as:
  - For Factorial Operation: If a non-integer or negative number input for calculating the factorial was provided. Example message could be "Error: Please enter a positive integer."
  
## History Management (Updated)
(Additional information on how history includes entries from new operations, such as factorials.)
8 | View Calculation History | Allows users to view their calculation history including the newly added Factorial Operation. Users can navigate through different calculations and see results for each operation performed in chronological order of entry with options like 'View Latest', 'Search by Operator/Number' etc. 

## Examples (Updated)
(Include examples demonstrating factorial operations, e.g., `5! = 120`)
9 | Example Calculations | Showcases various example calculations including the application of Factorial Operation with inputs like 'Factorial of 6' and their respective outputs such as "The factorial of 6 is 720". Additional examples for power/exponentiation are also included.

## Testing (Updated)
(Test cases now include scenarios where the user attempts to calculate a factorial, including edge cases like zero or negative inputs.)
10 | Unit Tests and Edge Cases | Detailed list of unit tests that cover all features with special attention on Factorial Operation. This includes testing for typical use-cases (positive integers), boundary conditions (e.g., 0! = 1, factorial results