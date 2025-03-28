# Python List, Tuple, and Dictionary Cheat Sheet


# Python List Operations

## Creating a List
```python
lst = [1, 2, 3, 4, 5]
```

## Accessing Elements
```python
print(lst[0])  # First element
print(lst[-1]) # Last element
print(lst[1:4])  # Slicing (index 1 to 3)
print(lst[:3])  # First three elements
print(lst[::2])  # Every second element
print(lst[::-1])  # Reverse the list using slicing
```

## Modifying Elements
```python
lst[1] = 10  # Change element at index 1
lst[2:4] = [20, 30]  # Modify multiple elements
```

## Adding Elements
```python
lst.append(6)  # Add at end
lst.insert(2, 15)  # Insert at index 2
lst.extend([7, 8, 9])  # Add multiple elements at the end
lst += [10, 11]  # Alternative way to extend a list
```

## Removing Elements
```python
lst.remove(3)  # Remove by value
popped = lst.pop()  # Remove last element
popped_index = lst.pop(2)  # Remove element at index 2
del lst[1]  # Delete element at index 1
del lst[2:4]  # Delete multiple elements
lst.clear()  # Clear all elements
```

## Copying Lists
```python
copy_lst = lst.copy()  # Create a copy
copy_lst2 = list(lst)  # Alternative way to copy
```

## Searching in Lists
```python
count_2 = lst.count(2)  # Count occurrences of 2
if 3 in lst:
    index_3 = lst.index(3)  # Find index of 3
```

## Sorting and Reversing
```python
lst = [5, 3, 8, 1, 2]
lst.sort()  # Sort in ascending order
lst.sort(reverse=True)  # Sort in descending order
lst.reverse()  # Reverse the list
```

## List Comprehension
```python
squared = [x**2 for x in lst]  # Create a list of squares
filtered = [x for x in lst if x % 2 == 0]  # Filter even numbers
```

## Using `map`, `filter`, and `reduce`
```python
from functools import reduce
mapped = list(map(lambda x: x * 2, lst))  # Double each element
filtered = list(filter(lambda x: x > 3, lst))  # Keep numbers >3
summed = reduce(lambda x, y: x + y, lst)  # Sum of all elements
```

## Splitting and Joining
```python
string = "apple,banana,grape"
split_list = string.split(",")  # Convert string to list
joined_string = "-".join(split_list)  # Convert list to string
```

## Nested Lists
```python
nested_lst = [[1, 2, 3], [4, 5, 6]]
print(nested_lst[1][2])  # Access nested list elements
```

## Enumerate (Index with Value)
```python
for index, value in enumerate(lst):
    print(f"Index: {index}, Value: {value}")
```

## Zipping Lists
```python
list1 = [1, 2, 3]
list2 = ['a', 'b', 'c']
zipped = list(zip(list1, list2))  # [(1, 'a'), (2, 'b'), (3, 'c')]
```

## Unzipping
```python
unzipped1, unzipped2 = zip(*zipped)
```

## Set Operations with Lists
```python
unique_lst = list(set(lst))  # Remove duplicates
intersection = list(set(list1) & set(list2))  # Find common elements
```

## Min, Max, and Sum
```python
min_val = min(lst)
max_val = max(lst)
sum_val = sum(lst)
```

## All and Any
```python
all_true = all([True, True, False])  # False (all must be true)
any_true = any([False, False, True])  # True (at least one must be true)
```



# Tuple (Ordered, Immutable)

## Creating a Tuple
```python
# Creating a Tuple
tpl = (1, 2, 3, 4, 5)
```

## Accessing Elements
```python
print(tpl[0])  # First element
print(tpl[-1]) # Last element
```

## Tuple Packing & Unpacking
```python
a, b, c = (10, 20, 30)
print(a, b, c)
```

## Immutable Nature (Causes Error)
```python
# tpl[1] = 10  # TypeError: 'tuple' object does not support item assignment
```

## Inbuilt Functions
```python
length = len(tpl)  # Get length
count_2 = tpl.count(2)  # Count occurrences of 2
index_3 = tpl.index(3)  # Find index of 3
```

## Converting Tuple to List
```python
tpl_list = list(tpl)  # Convert tuple to list
```

## Creating Tuple from Iterable
```python
tpl_from_list = tuple([10, 20, 30])  # Convert list to tuple
tpl_from_str = tuple("hello")  # Convert string to tuple
```

## Concatenation
```python
tpl2 = (6, 7, 8)
new_tpl = tpl + tpl2  # Merging tuples
```

## Repetition
```python
repeated_tpl = tpl * 2  # (1, 2, 3, 4, 5, 1, 2, 3, 4, 5)
```

## Checking Membership
```python
is_present = 3 in tpl  # True
is_absent = 10 not in tpl  # True
```

## Iterating through Tuple
```python
for item in tpl:
    print(item)
```

## Slicing Tuples
```python
sub_tpl = tpl[1:4]  # (2, 3, 4)
```

## Finding Min and Max
```python
min_value = min(tpl)  # 1
max_value = max(tpl)  # 5
```

## Summing Elements
```python
sum_of_elements = sum(tpl)  # 15
```

## Sorting (Returns a List)
```python
sorted_tpl = sorted(tpl, reverse=True)  # [5, 4, 3, 2, 1]
```

## Nested Tuples
```python
nested_tpl = ((1, 2), (3, 4), (5, 6))
print(nested_tpl[1][1])  # 4
```

## Tuple with Single Element (Comma Required)
```python
single_element_tpl = (42,)  
print(type(single_element_tpl))  # <class 'tuple'>
```

## Using `zip` with Tuples
```python
tuple1 = (1, 2, 3)
tuple2 = ('a', 'b', 'c')
zipped = tuple(zip(tuple1, tuple2))  # ((1, 'a'), (2, 'b'), (3, 'c'))
```

## Tuple Comprehension (Using Generator Expression)
```python
squared_tpl = tuple(x**2 for x in tpl)  # (1, 4, 9, 16, 25)
```


## Python Dictionary Basics and Advanced Operations

### Creating a Dictionary
```python
dct = {"name": "Alice", "age": 25, "city": "New York"}
```

### Accessing Elements
```python
print(dct["name"])  # Direct access
print(dct.get("age"))  # Safe access
```

### Modifying Elements
```python
dct["age"] = 26  # Update value
dct["country"] = "USA"  # Add new key-value pair
```

### Removing Elements
```python
del dct["city"]  # Remove key
age = dct.pop("age")  # Remove and return value
```

### Iterating Over a Dictionary
```python
for key, value in dct.items():
    print(key, value)
```

### Dictionary Methods
```python
keys = dct.keys()  # Get all keys
values = dct.values()  # Get all values
items = dct.items()  # Get all key-value pairs
copy_dct = dct.copy()  # Create a copy
dct.clear()  # Clear all elements
default_value = dct.setdefault("gender", "Female")  # Get value or set default
```

## Advanced Dictionary Operations in Python

### Creating a Dictionary with `dict()` and `fromkeys()`
```python
# Using dict()
dct = dict(name="Alice", age=25, city="New York")

# Using fromkeys() to create a dictionary with default values
default_dct = dict.fromkeys(["name", "age", "city"], "Unknown")
```

### Merging Dictionaries (Python 3.9+)
```python
d1 = {"a": 1, "b": 2}
d2 = {"b": 3, "c": 4}
merged_dct = d1 | d2  # { 'a': 1, 'b': 3, 'c': 4 }
```

### Updating Dictionary
```python
d1.update(d2)  # d1 now contains merged values
```

### Dictionary Comprehensions
```python
squared = {x: x**2 for x in range(5)}  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
conditional_dct = {k: v for k, v in d1.items() if v > 2}  # Filtering
```

### Nested Dictionary
```python
nested_dct = {
    "person1": {"name": "Alice", "age": 25},
    "person2": {"name": "Bob", "age": 30}
}
print(nested_dct["person1"]["name"])  # Alice
```

### Using `defaultdict` (from `collections`)
```python
from collections import defaultdict
dd = defaultdict(int)  # Default value is 0 for missing keys
dd["x"] += 5  # No KeyError
```

### Using `Counter` (from `collections`)
```python
from collections import Counter
counter_dct = Counter("mississippi")  # {'i': 4, 's': 4, 'p': 2, 'm': 1}
```

### Using `OrderedDict` (Maintains Order of Insertion)
```python
from collections import OrderedDict
od = OrderedDict()
od["a"] = 1
od["b"] = 2
od["c"] = 3  # Ordered insertions
```

### Using `setdefault()` for Nested Updates
```python
d = {}
d.setdefault("students", []).append("Alice")
d.setdefault("students", []).append("Bob")  # Only first call initializes key
```

### Dictionary Packing & Unpacking
```python
data = {"x": 10, "y": 20}
def func(x, y):
    return x + y

result = func(**data)  # Unpacks dictionary into function arguments
```

### Swapping Keys and Values
```python
swapped = {v: k for k, v in d1.items()}  # {1: 'a', 3: 'b', 4: 'c'}
```

### Removing Elements Safely
```python
d1.pop("b", "Not Found")  # Removes 'b', returns 'Not Found' if absent
```

### Iterating with `enumerate()`
```python
for i, (key, value) in enumerate(d1.items()):
    print(i, key, value)
```

### Sorting Dictionary
```python
sorted_dct = dict(sorted(d1.items(), key=lambda item: item[1], reverse=True))
```

### Using `max()` and `min()` on Dictionary
```python
max_key = max(d1, key=d1.get)  # Key with max value
min_key = min(d1, key=d1.get)  # Key with min value
```

### Dictionary with Lambda Functions
```python
operations = {
    "add": lambda x, y: x + y,
    "mul": lambda x, y: x * y
}
print(operations["add"](5, 3))  # 8
```

### Merging Dictionaries (Python <3.9)
```python
merged = {**d1, **d2}  # Merging dicts
```

### Creating Dictionary with `zip()`
```python
keys = ["name", "age", "city"]
values = ["Alice", 25, "New York"]
zipped_dct = dict(zip(keys, values))  # {'name': 'Alice', 'age': 25, 'city': 'New York'}
```

### Deep Copy of Dictionary
```python
import copy
deep_copy_dct = copy.deepcopy(nested_dct)
```

### Reversing Dictionary
```python
reversed_dct = {k: v[::-1] if isinstance(v, str) else v for k, v in dct.items()}
```

