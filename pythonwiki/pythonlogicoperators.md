---
layout: page
title: Python Logic Operators
permalink: /python-wiki/arithmetic-operators
---
> Difficulty: Medium
> 

### Comparison Operators

Comparison operators compare two values to return a Boolean result. If the Boolean result is true, then the statement will execute

| Operator | Function | Syntax | Example | Boolean Result |
| --- | --- | --- | --- | --- |
| == | Equal to | x == y | 10 == 5 | False |
| > | Greater Than | x > y | 10 > 5 | True |
| < | Less Than | x < y | 10 < 5 | False |
| >= | Greater Than or Equal To | x >= y | 10 >= 5 | True |
| <= | Less Than or Equal To | x <= y | 10 <= 5 | False |
| != | Not Equal To | x != y | 10 != 5 | True |

### Logic Operators

Logic operators combines two conditional statements

| Operator | Function | Syntax | Example |
| --- | --- | --- | --- |
| and | AND | x and y | 10 and 5 |
| or | OR | x or y | 10 or 5 |
| not | NOT | x not y | 10 not 5 |

```python
"""
This is a common mistake!
Each conditional statement should have a comparison after it before writing a logic
operator!
"""
if x and y == z:
	statement
#This condition is wrong! 

if x == z and y == z:
	statement
#This condition is correct
```

### Identity Operators

Identity operators compare if two objects are the same object, not if they have the same values.

| Operator | Function | Syntax |
| --- | --- | --- |
| is | is it the object? | x is y |
| is not | is it not the object? | x is not y |

```python
a = ["r", "g", "b"]
b = ["r", "g", "b"]
c = a

print(a is c) 
#Will print 'true' because a is the same as c.

print(a is b) 
#Will print 'false' because a is not the same as b but has the same values.

print(a is not c)
#Will print 'false' because a is the same as b.

print(a is not b) 
#Will print 'true' because a is not the same as b but has the same values.
```

### Membership Operators

Membership operators check if a value is in an object

| Operator | Function | Syntax |
| --- | --- | --- |
| in | is it in the object? | x in y |
| not in | is it not in the object? | x not in y |

```python
x = ["r", "g", "b"]

print("r" in x) 
#Will print 'true' because r is in array x.

print("c" in x) 
#Will print 'false' because r is not in array x.

print("r" not in x)
#Will print 'false' because r is in array x.

print("c" not in x) 
#Will print 'true' because r is not in array x.
```

### Bitwise (Binary) Operators

Bitwise operators compare binary numbers. They are called bitwise because one digit of binary is called a bit

| Operator | Function | Syntax | Example |
| --- | --- | --- | --- |
| & | AND | x & y | 10 == 5 |
| | | OR | x | y | 10 > 5 |
| ^ | XOR | x ^ y | 10 < 5 |
| ~ | NOT | x ~ y | 10 >= 5 |
| << | Shift Left | x << y | 10 <= 5 |
| >> | Shift Right | x >> y | 10 != 5 |