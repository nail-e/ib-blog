---
layout: page
title: Python Arithmetic Operators
permalink: /python-wiki/arithmetic-operators
---
> Difficulty: Easy
> 

### Arithmetic Operators

For the table, let

```python
x = 10
y = 5
z = 3
```

| Operator | Assignment | Function | Syntax | Equal to: | Result |
| --- | --- | --- | --- | --- | --- |
| + | += | Add | x + y | 10 + 5 | 15 |
| - | -= | Subtract | x - y | 10 - 5 | 5 |
| / | /= | Divide | x / y | 10 / 5 | 2 |
| * | *= | Multiply | x * y | 10 * 5 | 50 |
| % | %= | Modulus (Mod) | x % z | 10 % 3 | 1 |
| ** | **= | Exponentiation | y ** z | 5^3 | 125 |
| // | //= | Floor Division | x // z | 10 // 3 | 3 |

### Assignment of Arithmetic Operators

Instead of typing `x = x + 1` or typing `x = x / 1` to assign an existing variable with a new value, 
`x += 1` or `x /= 1` can be typed.

### Incrementing and Decrementing

Python doesn’t have a direct incrementing or decrementing function. `x += 1` increments while 
`x -= 1`  decrements.