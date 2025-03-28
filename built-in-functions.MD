# Python Inbuilt Functions Cheatsheet

## Output Functions
```python
print("Hello, World!")  # Prints output to the console
```

## Type Conversion Functions
```python
int("10")  # Converts string to integer
float("10.5")  # Converts string to float
str(100)  # Converts number to string
bool(1)  # Converts value to boolean
list("abc")  # Converts string to list
set([1, 2, 2, 3])  # Converts list to set
dict([(1, 'a'), (2, 'b')])  # Converts tuples to dictionary
tuple([1, 2, 3])  # Converts list to tuple
frozenset([1, 2, 3])  # Converts list to immutable set
complex(1, 2)  # Creates a complex number (1 + 2j)
```

## Mathematical Functions
```python
abs(-10)  # Returns absolute value
pow(2, 3)  # Returns 2 raised to the power of 3
round(3.14159, 2)  # Rounds to 2 decimal places
min(1, 2, 3)  # Returns the minimum value
max(1, 2, 3)  # Returns the maximum value
sum([1, 2, 3])  # Returns the sum of iterable
divmod(10, 3)  # Returns quotient and remainder as tuple
```

## Iterables & Sequence Functions
```python
len("Python")  # Returns length of object
sorted([3, 1, 2])  # Returns sorted list
reversed([1, 2, 3])  # Returns reversed iterator
enumerate(["a", "b", "c"])  # Returns index-value pairs
zip([1, 2], ["a", "b"])  # Pairs elements from two iterables
all([True, True, False])  # Returns True if all elements are True
any([False, False, True])  # Returns True if any element is True
```

## String Functions
```python
chr(65)  # Converts ASCII to character
ord("A")  # Converts character to ASCII
bin(10)  # Converts to binary
oct(10)  # Converts to octal
hex(10)  # Converts to hexadecimal
ascii("Hello 😊")  # Returns ASCII representation of string
```

## Input Functions
```python
input("Enter something: ")  # Takes user input
```

## Object & Type Functions
```python
type(10)  # Returns <class 'int'>
type(10.5)  # Returns <class 'float'>
type("Hello")  # Returns <class 'str'>
type([1, 2, 3])  # Returns <class 'list'>
type((1, 2, 3))  # Returns <class 'tuple'>
type({"a": 1, "b": 2})  # Returns <class 'dict'>
type({1, 2, 3})  # Returns <class 'set'>
type(True)  # Returns <class 'bool'>
type(None)  # Returns <class 'NoneType'>
isinstance(10, int)  # Checks if object is an instance of class
isinstance(10.5, (int, float))  # Checks if object is int or float
id(10)  # Returns memory address of object
hash("hello")  # Returns hash value of object
callable(len)  # Checks if object is callable
```

## Functional Programming
```python
map(lambda x: x * 2, [1, 2, 3])  # Applies function to iterable
filter(lambda x: x > 1, [0, 1, 2])  # Filters elements
reduce(lambda x, y: x + y, [1, 2, 3])  # Reduces iterable to single value
```

## File Handling
```python
open("file.txt", "r")  # Opens a file for reading
```

## Miscellaneous
```python
help(print)  # Shows help documentation
dir(str)  # Lists attributes of an object
repr("Hello")  # Returns string representation of object
eval("2 + 3")  # Evaluates expression in string format
exec("print('Hello')")  # Executes a Python command from string
globals()  # Returns global symbol table
locals()  # Returns local symbol table
```

## System & OS Functions
```python
import sys
sys.exit()  # Exits the script
sys.version  # Returns Python version

import os
os.getcwd()  # Returns current working directory
os.listdir()  # Lists files in directory
```
