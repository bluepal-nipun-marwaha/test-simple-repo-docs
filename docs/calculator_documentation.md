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
The Calculator Application is a Python-based command-line calculator that provides basic arithmetic operations with an interactive user interface, now including the newly added factorial operation for positive integers and error handling for invalid inputs or division by zero scenarios as per recent commit changes. The application also tracks calculation history to allow users to review past calculations easily.

## Features
- **Basic Arithmetic Operations**: Addition (+), subtraction (-), multiplication (*), division (/)
- **Advanced Operations**: Power/exponentiation operation, now includes factorial for positive integers as per the recent commit changes by bluepal-nipun-marwaha. The application gracefully handles invalid inputs and zero divisions with appropriate error messages to ensure a smooth user experience. 
- **Calculation History Tracking**: Users can view their calculation history which is now enhanced due to new factorial operation, allowing users not only the ability to track basic arithmetic operations but also complex ones like factorials. This feature provides insights into past calculations and helps in understanding usage patterns over time.
- **Interactive Command-Line Interface**: The application offers an easy-to-use command-line interface for performing various mathematical tasks, now with the addition of a new operation - Factorial calculation as per recent changes made to src/calculator.py by bluepal-nipun-marwaha
- **Error Handling and Validation**: The application has been improved in its error handling mechanism which gracefully handles invalid inputs or scenarios where division is attempted with zero, ensuring a seamless user experience without abrupt termination of the program. This includes appropriate feedback messages for such cases to help users understand their mistakes easily
- **History Management and Retrieval**: The application now provides enhanced history management features allowing easy retrieval of past calculations including newly added factorial operations, providing an all-rounded user experience with a comprehensive toolset at hand. 

## Installation & Usage
(Installation instructions remain the same)
... (Usage section remains unchanged but can be updated if necessary to reflect new changes in functionality.)

## Calculator Operations and Menu Options
The calculator operations have been expanded with a newly added factorial operation. The menu options now include: 
1 | Addition (+) - Sums two floating-point numbers, returns the sum as output (Example provided). Error handling included for invalid inputs or non-numeric values is also in place to ensure smooth user experience without abrupt termination of program due to such cases.
2 | Subtraction (-) - Subts second number from first and return difference as result with appropriate error checking implemented, ensuring a seamless operation flow even when faced by invalid inputs or non-numeric values (Example provided). 
3 | Multiplication (*) - Returns the product of two floating-point numbers. Error handling included for cases where division is attempted with zero to ensure smooth user experience without abrupt termination due to such scenarios, as well as graceful error checking implemented in case invalid inputs are encountered by users (Example provided).
4 | Division (/) - Divides first number by second and returns the quotient. Error handling included for cases where division is attempted with zero or when non-numeric values entered ensures a seamless user experience without abrupt termination due to such scenarios, as well as graceful error checking implemented in case invalid inputs are encountered (Example provided).
5 | Power/Exponentiation - Raises first number to the power of second and returns result. Error handling included for cases where division is attempted with zero or when non-numeric values entered ensures a seamless user experience without abrupt termination due to such scenarios, as well as graceful error checking implemented in case invalid inputs are encountered (Example provided).
6 | Factorial - Calculates the factorial of positive integers and returns result. Error handling included for cases where non-integer or negative values entered ensures a seamless user experience without abrupt termination due to such scenarios, as well as graceful error checking implemented in case invalid inputs are encountered (Example provided).
7 | Clear - Clears the entire calculation