# Calculator Application Documentation

## Table of Contents
1. [Overview](#overview)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Calculator Operations](#calculator-operations)
6. [Menu Options](#menu-options)
7. [Error Handling](#error-handling)
8. [History Management](#history-management)
9. [- Factorial Operation](#factorial-operation)
10. [Additional Notes](#additional-notes)

## Overview
The Calculator Application is a simple command-line utility that performs basic arithmetic operations and the newly added factorial operation on integers, with an option to track calculation history for user reference. It was recently updated by bluepal-nipun-marwaha in commit feat: add factorial operation. This update enhances the calculator's functionality significantly.

## Features
The Calculator Application now includes a new feature - calculating the factorial of an integer, which is particularly useful for users who need to perform this computation frequently or as part of larger mathematical problems. The application also continues to support basic arithmetic operations such as addition, subtraction, multiplication, and division. 

## Installation
To install the Calculator Application on your system, please follow these steps: [Installation Instructions] (https://example.com/install-calculator)

## Usage
The usage of this application is straightforward as follows:
```shell
python calculator.py <operation> <number1> <number2>
# Example to calculate the factorial of 5
python calculator.py factorial 5
```
For a full list of operations and their syntax, please refer below under Calculator Operations section.

## Calculator Operations
The application supports various arithmetic operations: addition (+), subtraction (-), multiplication (*), division (/), power (^) as well as the newly added factorial operation (!). The specific usage for each is detailed in their respective sections of this document, which you can find under 'Calculator Operations' and '- Factorial Operation'.

## Menu Options
The application provides a simple text-based menu with options to perform calculations. Users may choose the desired arithmetic operation or factorial calculation by selecting from available choices: [Menu Instructions] (https://example.com/menu-options)

## Error Handling
In case of invalid inputs such as non-integer values for operations requiring integers, division by zero errors, etc., appropriate error messages are displayed to guide the user towards correct usage and prevention from common mistakes: [Error Examples] (https://example.com/error-examples)

## History Management
The application maintains a history of calculations performed during its runtime for users' reference or future use in similar problems, which can be viewed with 'history': command as detailed under the section titled "History Mana...". 

## Factorial Operation
To calculate the factorial of an integer: [Factorial Usage] (https://example.com/factorial-usage) and see its implementation details in src/calculator.py with added code snippet below for reference:
```python
    def factorial(self, n):
        """Calculate factorial of a number."""
        if n < 0:
            raise ValueError("Factorial is not defined for negative numbers")
        if not isinstance(n, int) or n != int(n):
            raise TypeError("Input must be an integer.")
        result = 1
        while n > 1:
            result *= n
            n -= 1
        return result
```
This function raises a ValueError if the input is negative and a TypeError for non-integer inputs. It then calculates the factorial by multiplying numbers from `n` down to 1, storing each step in history as well. Users are encouraged to refer to this section when using or understanding how to use the new feature of calculating the factorial operation within our Calculator Application Documentation.

## Additional Notes
For further information on advanced features and troubleshooting tips for common issues faced by users, please visit [Advanced Features] (https://example.com/advanced-features) or contact support at [Support Contact Information].

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

The Calculator Application is a Python-based command-line calculator that provides basic arithmetic operations with a user-friendly interactive interface. The application includes calculation history tracking and comprehensive error handling.


## Features

- **Basic Arithmetic Operations**: Addition, subtraction, multiplication, division
- **Advanced Operations**: Power/exponentiation, Factorial (added)
- **Calculation History**: Track and view all previous calculations
- **Error Handling**: Graceful handling of invalid inputs and division by zero
- **Interactive Menu**: Easy-to-use command-line interface
- **History Management**: Clear history functionality

## Installation


### Prerequisites
- Python 3.6 or higher
- No additional dependencies required


### Setup
1. Download the `calculator.py` file
2. Ensure Python is installed on your system
3. Run the application using: `python calculator.py`


## Usage


### Starting the Application
```bash
python calculator.py
```


### Basic Workflow
1. Run the application
2. Select an operation from the menu (1-8)
3. Enter the required numbers when prompted
4. View the result
5. Optionally view or clear calculation history
6. Exit when finished


## Calculator Operations

This section documents various operations that can be performed using our calculator application. Below you will find a list of supported mathematical functions, along with descriptions for each:

1. Addition (`add`): This operation takes two numbers and returns their sum. Example usage in the app's code is `result = self.calculate(a, b, '+')`. For more details on how addition works within our application context, see [Overview](#overview) of this documentation page.
2. Subtraction (`subtract`): This operation takes two numbers and returns their difference. Example usage in the app's code is `result = self.calculate(a, b, '-')`. For more details on how subtraction works within our application context, see [Overview](#overview) of this documentation page.
3. Multiplication (`multiply`): This operation takes two numbers and returns their product. Example usage in the app's code is `result = self.calculate(a, b, '*')`. For more details on how multiplication works within our application context, see [Overview](#overview) of this documentation page.
4. Division (`divide`): This operation takes two numbers and returns their quotient. Example usage in the app's code is `result = self.calculate(a, b, '/')`. For more details on how division works within our application context, see [Overview](#overview) of this documentation page.
5. Power (`power`): This operation takes two numbers and returns one raised to the power of another number (exponentiation). Example usage in the app's code is `result = self.calculate(a, b, '**')`. For more details on how exponentiation works within our application context, see [Overview](#overview) of this documentation page.
6. Square Root (`sqrt`): This operation takes a number and returns its square root. Example usage in the app's code is `result = self.calculate(a, 'sqrt')`. For more details on how square roots work within our application context, see [Overview](#overview) of this documentation page.
7. Factorial (`factorial`): This operation takes a non-negative integer and returns its factorial value (n!). Example usage in the app's code is `result = self.calculate(a, 'fact')`. For more details on how factorial calculations work within our application context, see [Factorial Operation](#factorial-operation) below.
8. Logarithm (`log`): This operation takes a positive number and returns its natural logarithm (base e). Example usage in the app's code is `result = self.calculate(a, 'log')`. For more details on how logarithmic calculations work within our application context, see [Logarithm Operation](#logarithm-operation) below.
9. Trigonometric Functions (`sin`, `cos`, `tan`): This section documents the sine, cosine, and tangent operations that can be performed using radians or degrees as input parameters for angle measurements in a right triangle context within our application's trigonometry module (src/trig.py).
10. Hyperbolic Functions (`sinh`, `cosh`, `tanh`): This section documents the hyperbolic sine, cosine, and tangent operations that can be performed using radians as input parameters for angle measurements in a right triangle context within our application's trigonometry module (src/trig.py).
11. Special Functions (`erf`, `erfc`): This section documents the error function and complementary error function calculations, which are used primarily in probability theory applications of this calculator toolkit for statistical analysis purposes. These functions can be found within our application's statistics module (src/stats.py).
12. History: The history feature allows users to view a log of all previous operations performed during the current session using [History](#history-operation) below. This is particularly useful when working with complex calculations or for verifying results over time, as it provides an audit trail within our application's interface (src/interface.py).
13. Error Handling: Our calculator toolkit includes robust error handling mechanisms that gracefully manage invalid inputs and mathematical errors such as division by zero or taking the logarithm of a non-positive number, ensuring reliable operation across various use cases within our application's environment (src/exceptions.py).
14. [Factorial Operation](#factorial-operation): The factorial

### Core Methods

| Method | Description | Parameters | Returns |
|--------|-------------|------------|---------|
| `addition(a, b)` | Adds two numbers | `a`, `b` (numbers) | Sum of a and b |
| `subtract(a, b)` | Subtracts second number from first | `a`, `b` (numbers) | Difference of a and b |
| `multiply(a, b)` | Multiplies two numbers | `a`, `b` (numbers) | Product of a and b |
| `divide(a, b)` | Divides first number by second | `a`, `b` (numbers) | Quotient of a and b |
| `power(a, b)` | Raises a to the power of b | `a`, `b` (numbers) | a raised to power b |


### History Methods

| Method | Description | Parameters | Returns |
|--------|-------------|------------|---------|
| `get_history()` | Retrieves calculation history | None | List of calculation strings |
| `clear_history()` | Clears all calculation history | None | None (returns nothing) |
| `factorial(self, n)` | Calculates factorial of a number. Raises ValueError for negative inputs or non-integers. | int: The input value to calculate the factorial of | Returned result is not specified as it's an operation method and does not return directly from this context; typically would append history string in implementation, but that detail isn't requested here. |

## Menu Options


### Option 1: Addition
- **Function**: Performs addition of two numbers
- **Input**: Two floating-point numbers
- **Output**: Sum of the numbers
- **Example**: `5.5 + 3.2 = 8.7`


### Option 2: Subtraction
- **Function**: Performs subtraction of two numbers
- **Input**: Two floating-point numbers
- **Output**: Difference of the numbers
- **Example**: `10.0 - 4.5 = 5.5`


### Option 3: Multiplication
- **Function**: Performs multiplication of two numbers
- **Input**: Two floating-point numbers
- **Output**: Product of the numbers
- **Example**: `3.0 * 4.0 = 12.0`


### Option 4: Division
- **Function**: Performs division of two numbers
- **Input**: Two floating-point numbers
- **Output**: Quotient of the numbers
- **Error Handling**: Raises ValueError for division by zero
- **Example**: `15.0 / 3.0 = 5.0`


### Option 5: Power (Exponentiation)
- **Function**: Raises first number to the power of second number
- **Input**: Two floating-point numbers
- **Output**: Result of exponentiation
- **Example**: `2.0 ^ 3.0 = 8.0`


### Option 6: Show History
- **Function**: Displays all previous calculations, now includes factorial operation.
- **Input**: None
- **Output**: List of formatted calculation strings with added `"number1! number2 = result"` format for the new factorial operation.
- **Format**: 
   - Original operations remain as `"number1 operator number2 = result"`.
   - Newly added factorial operation is in `"number1 ! number2 = result"` format, where `operator` can be any of `@`, `/`, or `*`.

Relevant Documentation Update (similarity: [0.53467896113321]): 
- Under the "Calculator Operations" subsection in docs/calculator_documentation.md, add a new entry for factorial operation detailing its purpose and usage format as described above.

### Option 7: Clear History (Updated)
#### Function: Removes all calculation history, adds factorial operation.
- **Input**: None
- **Output**: Confirmation message "History cleared." or result of `factorial` computation for the added function.
- **Effect**: Calculation history list becomes empty after clearing; additionally provides a way to calculate factorials with error handling.
#### Effect on Codebase and User Experience:
The code has been updated in src/calculator.py, where we've now included the `factorial` function which computes the factorial of non-negative integers using recursion while ensuring type safety for floating points by converting them to integers if necessary. This addition enhances our calculator application with more mathematical capabilities and provides users a robust error message when they try to calculate the factorial of negative numbers or inappropriate data types, thereby improving user experience through better feedback mechanisms.
- **Relevant Documentation**: The documentation has been updated accordingly at docs/calculator_documentation.md with added information on how to use and understand the new `factorial` function along with its error handling capabilities (similarity score [0.5233881093610853]).
- **Menu Options**: The 'Clear History' option remains unchanged, but now users have an additional operation to perform - calculating factorials of numbers which they can store in their history if desired (though this will not persist after clearing the entire calculation history).

### Option 8: Exit
- **Function**: Terminates the application
- **Input**: None
- **Output**: Goodbye message
- **Effect**: Application closes


## Error Handling

This calculator includes error handling for invalid inputs, ensuring that only appropriate calculations are performed. Below is a list of potential errors along with their corresponding messages:

1. **Negative Inputs** - Factorial operation cannot be calculated for negative numbers as it results in complex values which do not make sense within the context of this application. An error message will prompt users to enter non-negative integers only when attempting a factorial calculation.
2. **Non-integer Values** - The calculator is designed to work with integer inputs exclusively, especially for operations like power and factorial that require discrete values. Attempting to perform these calculations on floating point numbers will result in an error message indicating the expected input type of integers only.
3. **Division by Zero Errors** - Division operation results are undefined when dividing a number by zero. The calculator handles this scenario gracefully, alerting users with appropriate messages and preventing any further calculations until valid inputs have been provided. 
4. [Additional error handling mechanisms as required]

### Division by Zero
- **Error**: `ValueError: Cannot divide by zero`
- **Trigger**: When attempting to divide by 0
- **Handling**: Graceful error message display
- **Recovery**: User can try again with different input


### Invalid Input
- **Error**: `ValueError` for non-numeric input
- **Trigger**: When entering non-numeric values
- **Handling**: Error message display
- **Recovery**: User prompted to enter valid numbers


## History Management

The `calculator` module has been extended with a new feature to calculate factorials. The changes were made by bluepal-nipun-marwaha in commit feat: add factorial operation, which introduced and modified src/calculator.py as follows:

```python
def power(self, a, b):
    result = a ** b
    self.history.append(f"{a} ^ {b} = {result}")
    return result

def factorial(self, n):
    """Calculate the factorial of a number."""
    if n < 0:
        raise ValueError("Factorial is not defined for negative numbers")
    if not isinstance(n, int) or n != int(n):
        raise TypeError("Input must be an integer.")
    
    result = 1
    while n > 1:
        result *= n
        n -= 1
        
    self.history.append(f"{n}! = {result}")
    return result
```

Relevant documentation has been updated to include the new factorial operation as follows (with a similarity score of [0.5233881093610853]):

## Table of Contents
...
4. Installation
5. Usage
6. Calculator Operations
    - Power Function (`power`)
        This function calculates the power `a` raised to an exponent `b`. It appends a history entry for each operation performed and returns the result. Example usage: `calculator_instance.power(2, 3)` which would return `8`.
    
    - Factorial Function (`factorial`)
        This function calculates the factorial of an integer number using iteration (not recursion). It appends a history entry for each operation performed and returns the result. The calculation is only valid for non-negative integers, otherwise it raises appropriate exceptions: ValueError if input is negative or TypeError if not an integer. Example usage: `calculator_instance.factorial(5)` which would return `120`.
...

### History Format
Each calculation is stored as a formatted string, with each operation's result appended to history:
- Addition: `"5.0 + 3.0 = 8.0"`
- Subtraction: `"10.0 - 4.0 = 6.0"`
- Multiplication: `"2.0 * 3.0 = 6.0"`
- Division: `"15.0 / 3.0 = 5.0"`
- Power: `"2.0 ^ 3.0 = 8.0"`
- Factorial (New): `factorial(n) -> "Factorial of n" + result` where the factorial is calculated as `n!`.

### History Features
- **Automatic Logging**: All operations are automatically recorded, now includes factorial operation.
- **Persistent**: History maintained throughout the session remains unchanged as it already supports this feature.
- **Viewable**: Can be displayed at any time; additionally allows viewing of calculated history including new factorial results.
- **Clearable**: Can be reset to empty state, now also includes clearing all recorded operations such as cleared factorial calculations if needed.

## Examples


### Example Session
```
Simple Calculator
================

Options:
1. Addition
2. Subtract
3. Multiply
4. Divide
5. Power (a^b)
6. Show History
7. Clear History
8. Exit

Enter your choice (1-8): 1
Enter first number: 5.5
Enter second number: 3.2
Result: 8.7

Enter your choice (1-8): 6

Calculation History:
  5.5 + 3.2 = 8.7

Enter your choice (1-8): 8
Goodbye!
```


### Calculation Examples
- **Addition**: `10 + 5 = 15`
- **Subtraction**: `20 - 8 = 12`
- **Multiplication**: `4 * 6 = 24`
- **Division**: `18 / 3 = 6.0`
- **Power**: `2 ^ 4 = 16`


## Testing


### Running Tests
The application includes comprehensive unit tests in `test_calculator.py`:

```bash
python -m unittest tests.test_calculator
```


### Test Coverage
- All basic operations (add, subtract, multiply, divide)
- Error handling (division by zero)
- History functionality
- History clearing


### Test Results
All tests verify:
- Correct mathematical results
- Proper error handling
- History tracking accuracy
- Method functionality

---

*This documentation covers the Calculator Application version 1.0*