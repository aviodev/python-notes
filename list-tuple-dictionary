# Python List, Tuple, and Dictionary Cheat Sheet

## List (Ordered, Mutable)
```python
# Creating a List
lst = [1, 2, 3, 4, 5]

# Accessing Elements
print(lst[0])  # First element
print(lst[-1]) # Last element

# Modifying Elements
lst[1] = 10

# Adding Elements
lst.append(6)  # Add at end
lst.insert(2, 15)  # Insert at index 2

# Removing Elements
lst.remove(3)  # Remove by value
popped = lst.pop()  # Remove last element

# List Comprehension
squared = [x**2 for x in lst]

# Inbuilt Functions
lst.sort()  # Sort the list
lst.reverse()  # Reverse the list
length = len(lst)  # Get length
lst.clear()  # Clear all elements
copy_lst = lst.copy()  # Create a copy
count_2 = lst.count(2)  # Count occurrences of 2
index_3 = lst.index(3)  # Find index of 3
```

## Tuple (Ordered, Immutable)
```python
# Creating a Tuple
tpl = (1, 2, 3, 4, 5)

# Accessing Elements
print(tpl[0])  # First element
print(tpl[-1]) # Last element

# Tuple Packing & Unpacking
a, b, c = (10, 20, 30)
print(a, b, c)

# Immutable Nature (Causes Error)
tpl[1] = 10  # TypeError: 'tuple' object does not support item assignment

# Inbuilt Functions
length = len(tpl)  # Get length
count_2 = tpl.count(2)  # Count occurrences of 2
index_3 = tpl.index(3)  # Find index of 3
```

## Dictionary (Key-Value Pairs, Mutable)
```python
# Creating a Dictionary
dct = {"name": "Alice", "age": 25, "city": "New York"}

# Accessing Elements
print(dct["name"])  # Get value by key
print(dct.get("age"))  # Safe way to get value

# Modifying Elements
dct["age"] = 26  # Update value
dct["country"] = "USA"  # Add new key-value pair

# Removing Elements
del dct["city"]  # Remove key
age = dct.pop("age")  # Remove and return value

# Iterating Over Dictionary
for key, value in dct.items():
    print(key, value)

# Inbuilt Functions
keys = dct.keys()  # Get all keys
values = dct.values()  # Get all values
items = dct.items()  # Get all key-value pairs
copy_dct = dct.copy()  # Create a copy
dct.clear()  # Clear all elements
default_value = dct.setdefault("gender", "Female")  # Get value or set default
```
