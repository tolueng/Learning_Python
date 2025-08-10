# Basics of Python: Data Types and Numbers

Welcome to the first chapter of Python basics! In this section, you'll learn about data types and how to work with numbers in Python.

## What are Data Types?

Data types define the kind of value a variable can hold. Understanding data types is important because it affects how you use and manipulate data in your programs.

### Main Data Types in Python

- **int** (Integer): Whole numbers, positive or negative, without decimals.
	- Examples: `5`, `-3`, `42`
	- Usage: Counting, indexing, math operations.
	- Tip: You can use underscores in large numbers for readability. For example, `1_000` is the same as `1000`, and `1_000_000` is the same as `1000000`.

- **float** (Floating Point): Numbers with decimals.
	- Examples: `3.14`, `-0.5`, `2.0`
	- Usage: Measurements, scientific calculations, division results.

- **str** (String): Text, enclosed in quotes (single or double).
	- Examples: `'hello'`, `"123"`, `'Python is fun!'`
	- Usage: Messages, names, any textual data.

- **bool** (Boolean): Represents True or False values.
	- Examples: `True`, `False`
	- Usage: Logic, conditions, decision making.

### How to Check Data Types
You can use the `type()` function to check the type of a value or variable:
```python
print(type(5))        # <class 'int'>
print(type(3.14))     # <class 'float'>
print(type("hello")) # <class 'str'>
print(type(True))     # <class 'bool'>
```

### Why Data Types Matter
Each data type behaves differently. For example, you can add two integers, but you cannot add an integer and a string directly:
```python
print(2 + 3)      # Valid, outputs 5
print("2" + "3")  # Valid, outputs '23' (string concatenation)
print(2 + "3")    # Error! Cannot add int and str
```

If you need to convert between types, use functions like `int()`, `float()`, or `str()`:
```python
num = "5"
print(int(num) + 2)  # Converts string to int, outputs 7
```

## Working with Numbers
Python can perform arithmetic with integers and floats:
```python
# Addition
print(2 + 3)  # Output: 5

# Subtraction
print(5 - 2)  # Output: 3

# Multiplication
print(4 * 3)  # Output: 12

# Division
print(10 / 2)  # Output: 5.0

# Integer Division
print(10 // 3)  # Output: 3

# Modulus (remainder)
print(10 % 3)  # Output: 1

# Exponentiation
print(2 ** 3)  # Output: 8
```

## Quick Exercise
Write a Python program that calculates the sum, difference, product, and quotient of two numbers (for example, 8 and 2) and prints the results.

### Solution
```python
num1 = 8
num2 = 2
print("Sum:", num1 + num2)
print("Difference:", num1 - num2)
print("Product:", num1 * num2)
print("Quotient:", num1 / num2)
```

---


## Strings in Python
Strings are sequences of characters used to represent text. You can create strings using single or double quotes:
```python
greeting = "Hello, world!"
name = 'Elif'
```

You can join (concatenate) strings, repeat them, and access individual characters:
```python
first = "Hello"
second = "World"
combined = first + ", " + second + "!"  # Output: Hello, World!
print(combined)
print(first * 3)  # Output: HelloHelloHello
print(first[0])   # Output: H
```

Strings also have many useful methods:
```python
text = "python is fun"
print(text.upper())  # Output: PYTHON IS FUN
print(text.capitalize())  # Output: Python is fun
print(text.replace("fun", "awesome"))  # Output: python is awesome
```

---


## Other Data Types

### List
A list is an ordered collection of items. Lists are mutable, meaning you can change, add, or remove items after creation.

```python
numbers = [1, 2, 3, 4]
fruits = ["apple", "banana", "cherry"]
print(fruits[1])  # Output: banana
fruits.append("orange")  # Adds 'orange' to the end
print(fruits)  # Output: ['apple', 'banana', 'cherry', 'orange']
fruits[0] = "grape"  # Change first item
print(fruits)  # Output: ['grape', 'banana', 'cherry', 'orange']
```

### Tuple
A tuple is like a list, but it is immutable (cannot be changed after creation). Useful for fixed collections of items.

```python
point = (3, 4)
print(point[0])  # Output: 3
# point[0] = 5  # Error! Tuples cannot be changed
coordinates = (1, 2, 3)
```

### Dictionary
A dictionary stores data as key-value pairs. Keys must be unique and immutable (like strings or numbers). Values can be any type.

```python
person = {"name": "Elif", "age": 25}
print(person["name"])  # Output: Elif
person["age"] = 26  # Update value
person["city"] = "Istanbul"  # Add new key-value pair
print(person)  # Output: {'name': 'Elif', 'age': 26, 'city': 'Istanbul'}
```

### Set
A set is an unordered collection of unique items. Useful for removing duplicates and performing set operations.

```python
unique_numbers = {1, 2, 3, 3, 2}
print(unique_numbers)  # Output: {1, 2, 3}
unique_numbers.add(4)  # Add new item
unique_numbers.remove(2)  # Remove item
print(unique_numbers)  # Output: {1, 3, 4}
```

---


## Cheatsheet & Tips

### Data Types
- Use `type(value)` to check the type of any variable.
- Convert between types with `int()`, `float()`, `str()`, `bool()`.
- Strings must be in quotes; numbers do not need quotes.

### Numbers
- `/` always returns a float, even if dividing two integers.
- `//` returns integer division (drops the decimal part).
- `%` gives the remainder after division.
- `**` is used for powers (exponentiation).

### Strings
- Use `+` to join strings, `*` to repeat them.
- Access characters with square brackets: `text[0]`.
- Common methods: `.upper()`, `.lower()`, `.replace()`, `.strip()`, `.split()`.

### Lists
- Lists are mutable: you can change, add, or remove items.
- Use `.append()` to add, `.remove()` to delete, `.sort()` to sort.
- Access items by index: `my_list[2]`.

### Tuples
- Tuples are immutable: you cannot change their contents.
- Useful for fixed data (coordinates, RGB colors).

### Dictionaries
- Access values by key: `my_dict['key']`.
- Add or update with `my_dict['new_key'] = value`.
- Use `.keys()`, `.values()`, `.items()` to get keys, values, or both.

### Sets
- Sets automatically remove duplicates.
- Use `.add()` to add, `.remove()` to delete.
- Useful for membership tests: `item in my_set`.

---

Use this section as a quick reference while practicing or solving problems!
