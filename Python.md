# Python

## Table of Contents

1. [Introduction to Python](#introduction-to-python)
2. [Variables ](#variables)
3. [Data Types](#data-types)
4. [Operators](#operators)
5. [Control Flow](#control-flow)
6. [Functions](#functions)
7. [Lists, Tuples, and Dictionaries](#lists-tuples-and-dictionaries)
8. [Modules and Packages](#modules-and-packages)

## Introduction to Python

Python is a high-level, interpreted programming language known for its simplicity and readability. It supports multiple programming paradigms, including procedural, object-oriented, and functional programming. Python's syntax allows developers to write clear and concise code, making it suitable for both beginners and experienced programmers.

## Variables

In Python, variables are used to store data values. Python has no command for declaring a variable, so you can simply assign a value to a variable to create one.

### Variable Naming Rules

- Variable names can contain letters, numbers, and underscores.
- Variable names must begin with a letter or an underscore.
- Variable names are case-sensitive (`myVariable`, `myvariable`, and `MyVariable` are all different variables).


Variables are created when they are first assigned a value.

```python
x = 5
y = "Hello, World!"
```

### Variable Scope

The scope of a variable refers to the places where you can access it. Variables in Python have global and local scope.

- Global variables: Variables declared outside of any function or class. They can be accessed from anywhere within the program.
- Local variables: Variables declared inside a function. They can only be accessed from within that function.

```python
global_var = "I am a global variable"

def my_function():
    local_var = "I am a local variable"
    print(global_var)
    print(local_var)
```

## Data Types

## Operators

Operators are special symbols in Python that carry out arithmetic or logical computation. Here are the different types of operators in Python:

- **Addition (`+`)**: Adds two operands.
  ```python
  x = 10
  y = 5
  print(x + y)  # Output: 15

- **Subtraction (`-`)**: Subtracts the second operand from the first.
  ```python
  print(x - y)  # Output: 5

- **Multiplication (`*`)**: Multiplies two operands.
   ```python
   print(x * y)  # Output: 50

- **Division (`/`)**: 
   ```python
   print(x / y)  # Output: 2.0


- **Modulus (`%`)**: 
   ```python
   print(x % y)  # Output: 0

- **Exponentiation (`**`)**: 
   ```python
   print(x ** y)  # Output: 100000

- **Floor division (`//`)**: 
   ```python
    print(x // y)  # Output: 2

### Comparison Operators

Comparison operators are used to compare values. They return either True or False.

- **Equal to (`==`)**: 
    ```python
    x = 10
    y = 10
    print(x == y)  # Output: True

- **Not equal to (`!=`)**: 
   ```python
   y = 5
   print(x != y)  # Output: True

- **Greater than (`>`)**: 
   ```python
   print(x > y)  # Output: True

- **Less than (`<`)**: 
   ```python
   print(x < y)  # Output: False

- **Greater than or equal to (`>=`)**: 
   ```python
   print(x >= y)  # Output: True

- **Less than or equal to (`<=`)**: 
   ```python
   print(x <= y)  # Output: False

### Logical Operators

Logical operators are used to combine conditional statements.

- **AND (`and`)**: 
    ```python
    a = True
    b = False
    print(a and b)  # Output: False 

- **OR (`or`)**: 
   ```python
   print(a or b)  # Output: True

- **NOT (`not`)**: 
   ```python
   print(not a)  # Output: False

### Assignment Operators

Assignment operators are used to assign values to variables.

- **Assign (`=`)**: 
   ```python
   x = 5
   print(x)  # Output: 5

- **Add and assign (`+=`)**: 
    ```python
    x += 3
    print(x)  # Output: 8

- **Subtract and assign (`-=`)**: 
    ```python
    x -= 2
    print(x)  # Output: 6

- **Multiply and assign (`*=``)**: 
    ```python
    x *= 2
    print(x)  # Output: 12
- **Divide and assign (`/=``)**: 
    ```python
    x /= 3
    print(x)  # Output: 4.0

- **Modulus and assign (`%=``)**: 
    ```python
    x %= 3
    print(x)  # Output: 1.0

- **Exponentiate and assign (`**=``)**: 
    ```python
    x **= 2
    print(x)  # Output: 1.0

- **Floor divide and assign (`//=``)**: 
    ```python
    x //= 2
    print(x)  # Output: 0.0

### Bitwise Operators

Bitwise operators act on operands as if they were strings of binary digits.

- **Bitwise AND (`&`)**: 
    ```python
    a = 10  # 1010 in binary
    b = 4   # 0100 in binary
    print(a & b)  # Output: 0 (0000 in binary)

- **Bitwise OR (`|`)**: 
    ```python
    print(a | b)  # Output: 14 (1110 in binary)

- **Bitwise XOR (`^`)**: 
    ```python
    print(a ^ b)  # Output: 14 (1110 in binary)

- **Bitwise NOT (`~`)**: 
    ```python
    print(~a)  # Output: -11 (Inverts all the bits)

- **Left shift (`<<`)**: 
    ```python
    print(a << 2)  # Output: 40 (101000 in binary)

- **Right shift (`>>`)**: 
    ```python
    print(a >> 2)  # Output: 2 (10 in binary)

### Membership Operators

Membership operators are used to test if a sequence is present in an object.

- **`in`**: Returns True if a sequence is present in the object.
    ```python
    fruits = ["apple", "banana", "cherry"]
    print("banana" in fruits)  # Output: True

- **`not in`**: Returns True if a sequence is not present in the object.
    ```python
    print("grape" not in fruits)  # Output: True

### Identity Operators

Identity operators compare the memory locations of two objects.

- **`is`**: Returns True if both variables point to the same object.
    ```python
    x = ["apple", "banana", "cherry"]
    y = x
    print(x is y)  # Output: True

- **`is not`**: Returns True if both variables do not point to the same object.
    ```python
    z = ["apple", "banana", "cherry"]
    print(x is not z)  # Output: True


## Control Flow in Python

Control flow statements in Python allow you to control the execution flow of your program based on certain conditions. Here are the main control flow constructs in Python:

### Conditional Statements

Conditional statements allow you to execute different blocks of code based on whether a condition is true or false.

### If Statement

The `if` statement is used to execute a block of code if a condition is true.

    ```python
    x = 10
    if x > 5:
        print("x is greater than 5")
    # Output: x is greater than 5

### Else Statment 
The else statement is used to execute a block of code if the condition in the if statement is false.
    ```python
    if condition:
        # code block to be executed if condition is true
    else:
        # code block to be executed if condition is false

    ```python
    x = 3
    if x > 5:
        print("x is greater than 5")
    else:
        print("x is not greater than 5")
    # Output: x is not greater than 5

### Elif Statment 
The elif (short for else if) statement is used to check multiple conditions.

    ```python
    if condition1:
        # code block to be executed if condition1 is true
    elif condition2:
        # code block to be executed if condition2 is true
    else:
        # code block to be executed if all conditions are false

    ```python
    x = 5
    if x > 5:
        print("x is greater than 5")
    elif x == 5:
        print("x is equal to 5")
    else:
        print("x is less than 5")
    # Output: x is equal to 5
