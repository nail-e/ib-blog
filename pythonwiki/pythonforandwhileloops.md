---
layout: page
title: Python For and While Loops
permalink: /python-wiki/loops
---
> Difficulty: Easy
> 

FOR loops are one of the two types of loops. FOR loops will repeat the statement a number of times or until the condition is satisfied or broken.

WHILE loops are one of the two types of loops. WHILE loops will repeat the statement indefinitely until the condition is satisfied or broken.

### FOR Loops

For loops will loop a statement for a set number of times within a set range.

```python
for i in range(1, 5) #Will loop 5 times, starting from 1
	print(i)
```

```
>>> 1
>>> 2
>>> 3
>>> 4
>>> 5
```

### WHILE Loops

For loops will loop a statement indefinitely until a condition is met.

```python
i = 1 #Flag/Sentinel, will "flag down" the code if the loop meets the condition.
while i <= 5:
	print(i)
	i += 1
```

```
>>> 1
>>> 2
>>> 3
>>> 4
>>> 5
```

As a general rule, for loops are faster and more optimized than while loops but while loops are better for times you loop code an unknown amount of times.

### Nested Loops

Nested loops are loops within a loop. The first loop will continuously loop until the loop inside stops.

```python
#Selection Sort
while i < len(array) - 1: #Loop one
	for j in range(i + 1, len(array)): #Loop two
		if array[j] < array[i]:
			array[j], array[i] = array[j], array[i]
while += 1 
```