## Calculator Application Documentation - Updated Version 1.0 (Updated on [Date of Update])

---

**Table of Contents:**

- [Overview](#overview)
    ...
    
- [Features](#features)
    ...
    * **Factorial Operation**: Calculates the factorial of a number using recursion. The user can input integers only, and negative numbers are not accepted to prevent complex calculations that may lead to stack overflow errors in recursive calls. Error handling ensures graceful degradation if non-integer inputs or out-of-range values (e.g., too large for practical computation) are provided by the user.
    ...
    
- [Installation](#installation)
    ...
    
- [Usage](#usage)
    To use this calculator, run `python src/calculator.py` from your command line interface (CLI). Follow on-screen prompts to select operations or enter a calculation directly into the CLI window. The factorial operation is accessible via option number 3 in our menu options: Factorial Operation
    ...
    
- [Calculator Operations](#calculator-operations)
    - **Factorial**: Calculates `n!` (factorial of n), where `n` must be a non-negative integer. If an invalid input is provided, the application will prompt for correct usage and terminate gracefully without crashing or producing incorrect results. The factorial function uses recursion to compute values efficiently up to 10!.
    ...
    
- [Menu Options](#menu-options)
    === Sheet: Menu Options ===
    Option Number | Option Name                   | Function           | Input Required       | Output               | Example          | Error Handling
    ------------|------------------------------|--------------------|---------------------|----------------------|------------------|---------------
    1           | Addition                      | Adds two numbers.  | Two floating-point...| Sum of the numbers   | `5.5 + 3.2 =`... | Handles invalid input gracefully
    ...          | Factorial Operation         | Calculates factorial...| A non-negative integer..| Result as an integer..| Input: `5`, Output:`120`.| Non-integer inputs or negative numbers are not accepted, and the user is prompted for correct usage. Exceeding practical computation limits results in a message advising of potential stack overflow risks with large factorials
    ...          | Subtraction                   | Subts...           | Two floating-point...| Difference as an integer..| `5 - 3 =`...     | Handles invalid input gracefully and ensures non-negative results. Negative outcomes are not possible due to the nature of subtraction
    ...          | Multiplication               | Multiples two numbers.| Two floating-point...| Product as an integer..| `5 * 3 =`...     | Handles invalid input gracefully and ensures non-negative results, with no negative outcomes possible due to the nature of multiplication
    ...          | Division                     | Divides first number by second.| Two floating-point numbers....| Quotient as a float..| `5 / 2 =`...      | Handles invalid input gracefully and ensures non-negative results, with no negative outcomes possible due to the nature of division
    ...          | Power/Exponentiation         | Raises first number to power of second.| Two floating-point numbers....| Result as an integer..| `5 ^ 2 =`...     | Handles invalid input gracefully and ensures non-negative results, with no negative outcomes possible due to the nature of exponentiation
    ...          | Calculation History Tracking | Tracks all previous calculations.| None                   | Display history as a list..| See past entries for `5 + 3 =`...`.| Error handling ensures that only valid calculation histories are displayed, with no negative or non-integer results possible
    ...          | Clear Calculation History     | Clears the recorded calculations.| None                   | Empty history display..| All previous entries cleared from view.`Clearing is confirmed by user input before proceeding`.`Error handling ensures that only valid clear operations are performed, with no negative or non-integer results possible
    ...          | Exit Application             | Closes the application.| None                   | Exits to command line..| `exit()` invoked...`, prompts for confirmation of exit before proceeding`.`Error handling ensures that only valid exits