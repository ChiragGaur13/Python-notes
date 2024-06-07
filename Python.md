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

### Arithmetic Operators

Arithmetic operators are used to perform mathematical operations.

- Addition (`+`)
- Subtraction (`-`)
- Multiplication (`*`)
- Division (`/`)
- Modulus (`%`)
- Exponentiation (`**`)
- Floor division (`//`)

### Comparison Operators

Comparison operators are used to compare values. They return either True or False.

- Equal to (`==`)
- Not equal to (`!=`)
- Greater than (`>`)
- Less than (`<`)
- Greater than or equal to (`>=`)
- Less than or equal to (`<=`)

### Logical Operators

Logical operators are used to combine conditional statements.

- AND (`and`)
- OR (`or`)
- NOT (`not`)

### Assignment Operators

Assignment operators are used to assign values to variables.

- Assign (`=`)
- Add and assign (`+=`)
- Subtract and assign (`-=`)
- Multiply and assign (`*=``)
- Divide and assign (`/=``)
- Modulus and assign (`%=``)
- Exponentiate and assign (`**=``)
- Floor divide and assign (`//=``)

### Bitwise Operators

Bitwise operators act on operands as if they were strings of binary digits.

- Bitwise AND (`&`)
- Bitwise OR (`|`)
- Bitwise XOR (`^`)
- Bitwise NOT (`~`)
- Left shift (`<<`)
- Right shift (`>>`)

### Membership Operators

Membership operators are used to test if a sequence is present in an object.

- `in`: Returns True if a sequence is present in the object.
- `not in`: Returns True if a sequence is not present in the object.

### Identity Operators

Identity operators compare the memory locations of two objects.

- `is`: Returns True if both variables point to the same object.
- `is not`: Returns True if both variables do not point to the same object.

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
