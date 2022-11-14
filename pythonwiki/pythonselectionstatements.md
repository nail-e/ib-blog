---
layout: page
title: Python Selection Statements (If-Else)
permalink: /python-wiki/selection-statements
---
> Difficulty: Easy
> 

```python
x = 3
if x = 1:
	print("1")
elif x = 2:
	print("2")
else:
	print("Not 1 and 2")
```

```
>>> "Not 1 and 2"
```

`if` statements will run if the condition is met.

`elif` statements will run if the if condition isn’t met.

`else` statements will run if no conditions are met.

### Shorthand If Else statements

Can be used to replace if else blocks with a simple, single line code in the syntax

```python
print("a") if a > b else print("b")
```

### Nested Selections

A nested selection is a selection statement within a selection statement

```python
x = 3
y = 1
if x = 3:
	print("x is 3")
	if y = 2:
		print("y is 2")
	else:
		print("y is not 2")
else:
	print("x is not 1")
```

```
>>> "x is 3"
>>> "y is not 2"
```