# Python Inbuilt Functions Cheatsheet

# Output Functions
print("Hello, World!")  # Prints output to the console

# Type Conversion Functions
int("10")  # Converts string to integer
float("10.5")  # Converts string to float
str(100)  # Converts number to string
bool(1)  # Converts value to boolean
list("abc")  # Converts string to list
set([1, 2, 2, 3])  # Converts list to set
dict([(1, 'a'), (2, 'b')])  # Converts tuples to dictionary

# Mathematical Functions
abs(-10)  # Returns absolute value
pow(2, 3)  # Returns 2 raised to the power of 3
round(3.14159, 2)  # Rounds to 2 decimal places
min(1, 2, 3)  # Returns the minimum value
max(1, 2, 3)  # Returns the maximum value
sum([1, 2, 3])  # Returns the sum of iterable

# Iterables & Sequence Functions
len("Python")  # Returns length of object
sorted([3, 1, 2])  # Returns sorted list
reversed([1, 2, 3])  # Returns reversed iterator
enumerate(["a", "b", "c"])  # Returns index-value pairs
zip([1, 2], ["a", "b"])  # Pairs elements from two iterables

# String Functions
chr(65)  # Converts ASCII to character
ord("A")  # Converts character to ASCII
bin(10)  # Converts to binary
oct(10)  # Converts to octal
hex(10)  # Converts to hexadecimal

# Input Functions
input("Enter something: ")  # Takes user input

# Object & Type Functions
type(10)  # Returns type of object
isinstance(10, int)  # Checks if object is an instance of class
id(10)  # Returns memory address of object

# Functional Programming
map(lambda x: x * 2, [1, 2, 3])  # Applies function to iterable
filter(lambda x: x > 1, [0, 1, 2])  # Filters elements

# File Handling
open("file.txt", "r")  # Opens a file for reading

# Miscellaneous
help(print)  # Shows help documentation
dir(str)  # Lists attributes of an object
