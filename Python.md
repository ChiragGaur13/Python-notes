# Python
<img src="https://th.bing.com/th/id/OIP.roeYpdgsxQwWdIfuoUJQEgHaFk?w=267&h=200&c=7&r=0&o=5&dpr=1.3&pid=1.7">


## Table of Contents

1. [Introduction to Python](#introduction-to-python)
2. [Variables ](#variables)
3. [Data Types](#data-types)

   a. [Mutable Datatypes](#mutable-datatypes)

   b. [Immutable Datatypes](#immutable-datatypes)

4. [Operators](#operators)
   
    a. [Arithmetic Operators](#arithmetic-operators)
   
    b. [Comparison Operators](#comparison-operators)
   
    c. [Logical Operators](#logical-operators)
   
    d. [Assignment Operators](#assignment-operators)
   
    e. [Bitwise Operators](#bitwise-operators)
   
    f. [Membership Operators](#membership-operators)
   
    g. [Identity Operators](#identity-operators)
   
5. [Conditional Statements](#conditional-statements)
6. [Loops](#loops)
7. [Functions](#functions)
8. [Modules](#modules)
9. [Conclusion](#conclusion)
10. [Refrences](#refrences)
   
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

Python has various standard datatypes that can be classified into mutable and immutable datatypes. Mutable datatypes can be changed after their creation, while immutable datatypes cannot be changed once they are created.

## Mutable Datatypes

### 1) List

A list is an ordered collection of items which can be of any type.

Lists are enclosed with square brackets.

#### Syntax

   ```python
    my_list = [1, 2, 3, "apple", "banana"]

    my_list = [1, 2, 3]
    print(my_list)  # Output: [1, 2, 3]

    # Changing an element
    my_list[1] = 20
    print(my_list)  # Output: [1, 20, 3]

    # Adding an element
    my_list.append(4)
    print(my_list)  # Output: [1, 20, 3, 4]
   ```
### 2) Dictionary

A dictionary is an unordered collection of key-value pairs. 
Each key is seprated by a colon(:).

Dictionary are enclosed with curly braces.


#### Syntax

```python
my_dict = {"name": "Alice", "age": 25}
print(my_dict)  # Output: {'name': 'Alice', 'age': 25}

# Changing a value
my_dict["age"] = 30
print(my_dict)  # Output: {'name': 'Alice', 'age': 30}

# Adding a key-value pair
my_dict["city"] = "New York"
print(my_dict)  # Output: {'name': 'Alice', 'age': 30, 'city': 'New York'}
```

### 3) Set

A set is an unordered collection of unique items. Sets are mutable.

Sets are enclosed with curly braces.


#### Syntax

```python
my_set = {1, 2, 3}
print(my_set)  # Output: {1, 2, 3}

# Adding an element
my_set.add(4)
print(my_set)  # Output: {1, 2, 3, 4}

# Removing an element
my_set.remove(2)
print(my_set)  # Output: {1, 3, 4}
```

## Immutable Datatypes

### 1) Numbers/Numeric

Numbers in Python (integers, floats, complex numbers) are immutable.

#### Syntax

```python
x = 10
print(x)  # Output: 10

# Numbers are immutable, so operations create new numbers
y = x + 5
print(y)  # Output: 15
print(x)  # Output: 10  (x is unchanged)
```


### 2) String

A string is a sequence of characters within quatation. 

#### Syntax

```python
my_string = "Hello, World!"
print(my_string)  # Output: Hello, World!

# Strings are immutable, so you cannot change a character directly
# my_string[0] = "h"  # This will raise an error

# But you can create a new string based on modifications
new_string = "h" + my_string[1:]
print(new_string)  # Output: hello, World!
```

### 3) Tuple

A tuple is an ordered collection of items which can be of any type. 

Tuple are enclosed within Parenthesis().


#### Syntax

   ```python
    my_tuple = (1, 2, 3)
    print(my_tuple)  # Output: (1, 2, 3)
    
    # Tuples are immutable, so you cannot change an element directly
    # my_tuple[1] = 20  # This will raise an error
    
    # But you can create a new tuple based on modifications
    new_tuple = my_tuple[:1] + (20,) + my_tuple[2:]
    print(new_tuple)  # Output: (1, 20, 3)
   ```


## Operators

Operators are special symbols in Python that carry out arithmetic or logical computation. Here are the different types of operators in Python:

### a) Arithmetic Operators

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

- **Division (`/`)**: Divide the first operand by the second.
   ```python
   print(x / y)  # Output: 2.0


- **Modulus (`%`)**: Returns the remainder when the first operand is divided by the second.
   ```python
   print(x % y)  # Output: 0

- **Exponentiation (`**`)**: Returns first raised to power second.
   ```python
   print(x ** y)  # Output: 100000

- **Floor division (`//`)**: Divides the first operand by the second and return integer value.
   ```python
    print(x // y)  # Output: 2

### b) Comparison Operators

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

### c) Logical Operators

Logical operators are used to combine conditional statements (either True or False).

- **AND (`and`)**: Returns True if both the operands are true
    ```python
    a = True
    b = False
    print(a and b)  # Output: False 

- **OR (`or`)**: Returns True if either of the operands is true
   ```python
   print(a or b)  # Output: True

- **NOT (`not`)**: Returns True if the operand is false
   ```python
   print(not a)  # Output: False

### d) Assignment Operators

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

- **Multiply and assign (`*=`)**: 
    ```python
    x *= 2
    print(x)  # Output: 12
- **Divide and assign (`/=`)**: 
    ```python
    x /= 3
    print(x)  # Output: 4.0

- **Modulus and assign (`%=`)**: 
    ```python
    x %= 3
    print(x)  # Output: 1.0

- **Exponentiate and assign (`**=`)**: 
    ```python
    x **= 2
    print(x)  # Output: 1.0

- **Floor divide and assign (`//=`)**: 
    ```python
    x //= 2
    print(x)  # Output: 0.0

### e) Bitwise Operators

Bitwise operators act on operands as if they were strings of binary digits.

- **Bitwise AND (`&`)**: Result bit 1, if both operand bits are 1; otherwise results bit 0.
    ```python
    a = 10  # 1010 in binary
    b = 4   # 0100 in binary
    print(a & b)  # Output: 0 (0000 in binary)

- **Bitwise OR (`|`)**: Result bit 1, if any of the operand bit is 1; otherwise results bit 0.
    ```python
    print(a | b)  # Output: 14 (1110 in binary)

- **Bitwise XOR (`^`)**: Result bit 1, if any of the operand bit is 1 but not both, otherwise results bit 0.
    ```python
    print(a ^ b)  # Output: 14 (1110 in binary)

- **Bitwise NOT (`~`)**: Inverts individual bits.
    ```python
    print(~a)  # Output: -11 (Inverts all the bits)

- **Left shift (`<<`)**: The left operand’s value is moved toward left by the number of bits. 
    ```python
    print(a << 2)  # Output: 40 (101000 in binary)

- **Right shift (`>>`)**: The left operand’s value is moved toward right by the number of bits. 
    ```python
    print(a >> 2)  # Output: 2 (10 in binary)

### f) Membership Operators

Membership operators are used to test if a sequence is present in an object.

- **`in`**: Returns True if a sequence is present in the object.
    ```python
    fruits = ["apple", "banana", "cherry"]
    print("banana" in fruits)  # Output: True

- **`not in`**: Returns True if a sequence is not present in the object.
    ```python
    print("grape" not in fruits)  # Output: True

### g) Identity Operators

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


## Conditional Statements

Conditional statements allow you to execute different blocks of code based on whether a condition is true or false.

### If Statement

The `if` statement is used to execute a block of code if a condition is true.

   ```python
    x = 10
    if x > 5:
        print("x is greater than 5")
    # Output: x is greater than 5
   ```

### Else Statment 
The else statement is used to execute a block of code if the condition in the if statement is false.

```python
if condition:
    # code block to be executed if condition is true
else:
    # code block to be executed if condition is false
```
   ```python
    x = 3
    if x > 5:
        print("x is greater than 5")
    else:
        print("x is not greater than 5")
    # Output: x is not greater than 5
   ```

### Elif Statment 
The elif (short for else if) statement is used to check multiple conditions.

```python
if condition1:
    # code block to be executed if condition1 is true
elif condition2:
    # code block to be executed if condition2 is true
else:
    # code block to be executed if all conditions are false
```
   ```python
    x = 5
    if x > 5:
        print("x is greater than 5")
    elif x == 5:
        print("x is equal to 5")
    else:
        print("x is less than 5")
    # Output: x is equal to 5
```


# Loops

Loops are used to execute a block of code repeatedly. Python provides two types of loops: `for` and `while`.

## For Loop

The `for` loop is used to iterate over a sequence (such as a list, tuple, dictionary, set, or string) or other iterable objects.

### Syntax

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
print(fruit)
# Output:
# apple
# banana
# cherry
```

## While Loop

The while loop is used to execute a block of code as long as a condition is true.

### Syntax

```python
i = 1
while i < 6:
    print(i)
    i += 1
# Output:
# 1
# 2
# 3
# 4
# 5
```

### Loop control Statment

- **Break Statment**:The break statement is used to exit the loop prematurely when a certain condition is met.

- **Continue Statment**: The continue statement is used to skip the current iteration of the loop and continue with the next iteration.

- **Pass Statment**: The pass statement is a null operation; it is used when a statement is required syntactically but you do not want any command or code to execute.


# Functions

Functions are reusable blocks of code that perform a specific task. Functions help in modularizing code and improving code readability.

## Defining a Function

A function is defined using the `def` keyword, followed by the function name and parentheses `()`.

### Syntax

```python
def function_name(parameters):
    # code block
    return value
```

```python
def greet(name):
    return f"Hello, {name}!"

print(greet("Alice"))  # Output: Hello, Alice!
```

## Function Arguments
Functions can take arguments, which are values passed to the function.

- **Positional Arguments**:
  
Positional arguments are the most common type of arguments. The values passed to the function are assigned to the parameters in order.

```python
def add(a, b):
    return a + b

print(add(2, 3))  # Output: 5
```

- **Keyword Arguments**:
  
Keyword arguments are passed to the function with their parameter names.

```python
def greet(name, message):
    return f"{message}, {name}!"

print(greet(name="Alice", message="Good morning"))  # Output: Good morning, Alice!

```

- **Default Arguments**:
  
Default arguments are specified in the function definition and are used if no value is passed for that parameter.

```python
def greet(name, message="Hello"):
    return f"{message}, {name}!"

print(greet("Alice"))           # Output: Hello, Alice!
print(greet("Bob", "Hi"))       # Output: Hi, Bob!
```


## Modules

A module is a file containing Python definitions and statements. The file name is the module name with the suffix `.py`.

### Creating a Module

To create a module, simply save the code you want in a file with a `.py` extension.

#### Example: `mymodule.py`

```python
def greet(name):
    return f"Hello, {name}!"

def add(a, b):
    return a + b
```

### Importing a Module
You can import the functions, classes, or variables from a module using the import statement.

```python
import module_name
```


## Conclusion
Python is a versatile and powerful programming language known for its simplicity and readability. This document has provided an overview of fundamental Python concepts, including variables, data types, operators, conditional statements, loops, functions, and modules. By understanding these foundational elements, you are ready to begin your journey into Python programming. Remember, practice makes perfect! Explore Python further to unlock its full potential for tasks like scripting, web development, and more.


## Refrences
https://www.python.org/doc/

https://www.w3schools.com/python/

https://www.geeksforgeeks.org/python-programming-language-tutorial/
