---
layout: page
title: Python Inputs
permalink: /python-wiki/inputs
---
### Basic Inputs

Variables can be assigned inputs

```python
age = input()
print(age)
```

```
>>> 16
>>> 16
```

Text can be assigned in between the input brackets

```python
age = input("What is your age")
print(age)
```

```
>>> "What is your age?" 16
>>> 16
```

### Giving Inputs a Data Type

Inputs can be given a specific data type 

```python
ageString = str(input("What is your age in words?"))
ageInt = int(input("What is your age in numbers?"))
ageFloat = float(input("What is your age in decimal?"))
print(ageString, ageInt, ageFloat)
```

```
>>> What is your age in words? Sixteen
>>> What is your age in numbers? 16
>>> What is your age in decimal? 16.0
>>> Sixteen 16 16.0
```

For bool, if any input is given a value, it’s automatically true. If no input is given, it’s automatically false.

```python
print(bool(input("Are you older than 18?")))
print(bool(input("Are you older than 18?")))
```

```
>>> "Are you older than 18?" Yes
>>> True
>>> "Are you older than 18?"
>>> False
```