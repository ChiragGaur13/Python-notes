# Python

## Table of Contents

1. [Introduction to Python](#introduction-to-python)
2. [Variables and Data Types](#variables-and-data-types)
3. [Operators](#operators)
4. [Control Flow](#control-flow)
5. [Functions](#functions)
6. [Lists, Tuples, and Dictionaries](#lists-tuples-and-dictionaries)
7. [Modules and Packages](#modules-and-packages)

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

