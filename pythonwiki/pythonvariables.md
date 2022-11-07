---
layout: page
title: Python Variables
permalink: /python-wiki/variables
---

> Difficulty: Easy

Python is a dynamically typed language so it auto-assigns data types to variables. Variables are easy to get the hang of.

### Python Data Types

- str - String
- int - Integer
- float - Decimal Number
- bool - Boolean, True or False
- NoneType - No data type, None
- complex - Complex Number
- list - An array
- tuple - An array with the same data type
- range - Prints the range of two or more numbers
- dict - A list with variables declared
- set - An array with multiple items, can have values added
- frozenset - An array with multiple items, can’t have values added
- byte - Prints an immutable sequence of bytes
- bytearray - Print a mutable sequence of bytes
- memoryview - Points to where in the memory the variable is stored

As a beginner, you don’t need to know all of these. Once you become more experienced, you might use some data types over others to increase code efficiency.

Variables can be declared with the `=` operator

```python
x = 5
print(x)
```

```
>>> 5
```

They can be given a data type. This is useful especially for inputs and outputs5
int(x)

```python
x = str(5)
x = int(5)
x = float(5)
```

```
>>> "5"
>>> 5
>>> 5.0
```

`type()` can be used to find the data type

```python
x = "Hello"
y = 10
z = ["foo", "bar"]
print(type(x))
print(type(y))
print(type(z))
```

```
>>> <class 'str'>
>>> <class 'int'>
>>> <class 'list'>
```

### Immutable and Mutable Variable

**Immutable** means that the data cannot be changed after declaration, like a constant in math. **Mutable** means that the data can be changed after declaration, like a variable in math.

### Primitive Variable

**Primitive** data types represent one standard value. 
**Non-primitive** data types are made of primitive types and have to be defined.

### Data Type Table

| Data Type | Syntax | Primitive? | Mutable? | Example |
| --- | --- | --- | --- | --- | 
| String | str() | Primitive | Immutable | print(”Hello World”) |  
| Integer | int() | Primitive | Immutable | print(3) |  
| Float | float() | Primitive | Immutable | print(4.3) |  
| Complex | complex() | Non-Primitive | Immutable | print(1j) |  
| Boolean | bool() | Primitive | Immutable | isSorted = False |  
| Range | range() | Non-Primitive | Immutable | for i in range(1,6): |  
| Array/List | list() or [ ] | Non-Primitive | Mutable | [1, 2, 3, 4, 5] | 
| Tuple | tuple() | Non-Primitive | Immutable | tuple = (”red”, “green”, “blue”) | 
| Dictionary | dict() | Non-Primitive | Mutable | x = {"name" : "John", "age" : 36} |
| Set | set() | Non-Primitive | Mutable | set = {"r", "g", "b"} 
| Frozen Set | frozenset() | Non-Primitive | Immutable | frozen = frozenset({"r, "g", "b"}) 
| Byte | bytes() | Non-Primitive | Immutable | print(b”Hello”) |  
| Byte Array | bytearray() | Non-Primitive | Mutable | bytearray(5) |  
| Pointer | memoryview() | Non-Primitive | Immutable | memoryview(bytes(5)) |  
| None |  | Primitive | Immutable | return None |  