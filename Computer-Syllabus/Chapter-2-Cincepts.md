# Chapter 2: User Interface

## Detailed Concepts

### 2.1 Input and Output (I/O) Operations
To interact with a computer program, we need a way to provide input and display output. Each programming language has its own keywords or standard built-in functions for I/O operations.

- **printf**: A built-in function in the C programming language. The name comes from "print formatted" and is used to display formatted output on the screen.
- **scanf**: A built-in function in C that takes input from the user and stores it in variables.

### 2.2 Format Specifiers
Format specifiers are used to specify the format of data during input and output operations. They are always preceded by a percentage (%) sign.

### 2.3 getch Function
The `getch()` function is used to read a character from the user. This function accepts characters only, and the character entered by the user is not displayed on the screen.

### 2.4 Statement Terminator
A **statement terminator** helps the compiler identify the end of a statement. In C language, a semicolon (;) is used as the statement terminator.

### 2.5 Escape Sequences
Escape sequences allow `printf()` to escape from its normal behavior. They are combinations of an escape character and another character associated with special functionality.

- **\n**: Moves the cursor to the start of the next line. Used to display output on multiple lines.
- **\t**: Moves the cursor to the next tab stop horizontally. A tab stop is the collection of 8 spaces.

### 2.6 Basic Operators
Operators are symbols used to perform operations on data. Some basic types of operators include:
- **Arithmetic Operators**: Used to perform arithmetic operations such as addition, subtraction, multiplication, division, and modulus.
    - Arithmetic operators are `+`, `-`, `*`, `/`, and `%`.
    - The **modulus operator** `%` returns the remainder of a division and works on integer data types.
- **Relational Operators**: Compare two values to determine the relationship between them.
- **Logical Operators**: Perform operations on Boolean expressions and return Boolean values (`true` or `false`).
    - **Logical AND (`&&`)**: Returns `true` if both expressions are true.
    - **Logical OR (`||`)**: Returns `true` if either of the two expressions is true.
    - **Logical NOT (`!`)**: Returns `true` if the expression is false, and vice versa.

### 2.7 Short Circuiting
Short circuiting allows deducing the result of an operation without computing the entire expression. It is commonly used with logical operators.

### 2.8 Types of Operators
- **Unary Operator**: Requires one operand to perform an operation.
- **Binary Operator**: Requires two operands.
- **Ternary Operator**: Requires three operands.

### 2.9 Operator Precedence
Operator precedence determines which operation should be performed first when multiple operators are used in an expression. Operators with higher precedence are evaluated first, while those with lower precedence are evaluated last.
