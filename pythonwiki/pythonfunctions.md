---
layout: page
title: Creating a Function
permalink: /python-wiki/functions
---
> Difficulty: Medium
> 

In Python, functions is a callable section of code with parameters and arguments that can be reused multiple times in a program.

### ********************************Initializing a Function********************************

A function can be created with the `def` keyword. Function names follow the naming convention of variables.

```python
def function():
	print("Hello world")
```

A function needs to be called in order to print

```python
def function():
	print("Hello world")

function()
```

```
>>> "Hello World"
```

### `print` vs `return`

Printing at the end of the function is different from returning a function. `return` can return a value while `print` can print any value automatically.

```python
def printing():
	print("This is a printed function")

def returning():
	return "This is a returned function"   #Returning doesn't require brackets

printing()
print(returning())   #A returning function needs to be printed than just called
```

```
>>> "This is a printed function"
>>> "This is a returned function"
```

### Parameters and Arguments

Parameters are the required values to be passed into the function, while arguments are when the parameters are given a value within a function. In other words, arguments are passed into the parameter.

```python
def account(creationYear, userName):    #These are the parameters
	creationYear = int(input("What year was the account created? "))   #These are the arguments
	userName = str(input("What is your username? "))    #Replaces 0
	return userName, "was created on ", creationYear 

print(account(0, 0))    #0, 0 are placeholders, they are replaced within the code
```

```
>>> What year was the account created? 2022
>>> What is your username? fortnite.jimmy
>>> ('fortnite.jimmy', 'was created on ', 2022)
```

Parameters need to be the correct amount.

`print(account(0,0,0))` will print an error because there are three arguments

`print(account(0,0))` will print because there are two arguments

### Default Parameters

If no arguments are passed, default parameters will be input instead 

```python
def account(creationYear = 2021, userName = "placeholder"):
	#The default parameters are 2021 and "placeholder"
	#There are no given arguments in this function
	return userName, "was created on ", creationYear 

print(account(0, 0))    #0, 0 are placeholders, they are replaced within the code
```

```
>>> What year was the account created? 2021
>>> What is your username? placeholder
>>> ('placeholder', 'was created on ', 2021)
```

### Pass Statement

Pass statements can be written instead of return to avoid errors

```python
def funcction():
	pass    #With pass
function()
```

```
>>> 
#There should be no error here
```

An EOF error will occur with no pass

```python
def funcction(): 
function()   #Without pass
```

```
>>> SyntaxError: unexpected EOF while parsing
```