---
layout: page
title: Python Exception Handling
permalink: /python-wiki/exception-handling
---
>Difficulty: Hard

Exception handling is the process when Python will generate a custom error written by the programmer during the running of the program.

### How do we catch exceptions?

Exceptions are any errors that are produced. Of course, Python can’t check every single piece of code written then create a custom error message, hence the existence of `try` . Any code under `try` will be ran. If an error is encountered, then code under `except` will run.

```python
#Exception Handling
try:
print(10/0)
except:
print("You cannot divide by zero")
```

Without exception handling, it’ll print

```
>> Traceback (most recent call last):
>>  File "<pyshell#0>", line 1, in <module>
>>    10/0
>> ZeroDivisionError: division by zero
```

But with exception handling, it’ll print

```
>> "You cannot divide by zero"
```

After any execution of `except` blocks, the code will run continuously.

### Catching specific errors

Keep in mind, the “You cannot divide by zero” error message will always print even if the error is different. 

```python
try:
print(10/"zero")
except:
print("You cannot divide by zero")
```

```
>> "You cannot divide by zero"
```

Normally, this will give a TypeError rather than a ZeroDivisionError, yet the custom error is printed. We can change this by adding the error code after `except` .

```python
try:
print(10/"zero")
except ZeroDivisionError:
print("You cannot divide by zero")
except TypeError:
print("You divided two different types of Data Types")
```

So now, if we try to run the code above,

```
>> "You divided two different types of Data Types"
```

### `finally` …

Any code under `finally` always prints.

```python
try:
print(10/0)
except ZeroDivisionError:
print("You cannot divide by zero")
except TypeError:
print("You divided two different types of Data Types")
finally:
print("Change the divisor")
```

```
>> "You cannot divide by zero"
>> "Change the divisor"
```

### Table of possible errors

| Exception | Description      |
| --- | --- |
| AssertionError | Raised when the assert statement fails. |
| AttributeError | Raised on the attribute assignment or reference fails.
                         |
| EOFError                         | Raised when the input() function hits the end-of-file condition. |
| FloatingPointError
                         | Raised when a floating point operation fails.
                         |
| GeneratorExit
                         | Raised when a generator's close() method is called.
                         |
| ImportError
                         | Raised when the imported module is not found.
                         |
| IndexError
                         | Raised when the index of a sequence is out of range.
                         |
| KeyError
                         | Raised when a key is not found in a dictionary.
                         |
| KeyboardInterrupt
                         | Raised when the user hits the interrupt key (Ctrl+c or delete).
                         |
| MemoryError
                         | Raised when an operation runs out of memory.
                         |
| NameError
                         | Raised when a variable is not found in the local or global scope.
                         |
| NotImplementedError
                         | Raised by abstract methods.
                         |
| OSError
                         | Raised when a system operation causes a system-related error.
                         |
| OverflowError
                         | Raised when the result of an arithmetic operation is too large to be represented.
                         |
| ReferenceError
                         | Raised when a weak reference proxy is used to access a garbage collected referent.
                         |
| RuntimeError
                         | Raised when an error does not fall under any other category.
                         |
| StopIteration
                         | Raised by the next() function to indicate 
that there is no further item to be returned by the iterator.
                         |
| SyntaxError
                         | Raised by the parser when a syntax error is encountered.
                         |
| IndentationError
                         | Raised when there is an incorrect indentation.
                         |
| TabError
                         | Raised when the indentation consists of inconsistent tabs and spaces.
                         |
| SystemError
                         | Raised when the interpreter detects internal error.
                         |
| SystemExit
                         | Raised by the sys.exit() function.
                         |
| TypeError
                         | Raised when a function or operation is applied to an object of an incorrect type.
                         |
| UnboundLocalError
                         | Raised when a reference is made to a local 
variable in a function or method, but no value has been bound to that 
variable.
                         |
| UnicodeError
                         | Raised when a Unicode-related encoding or decoding error occurs.
                         |
| UnicodeEncodeError
                         | Raised when a Unicode-related error occurs during encoding.
                         |
| UnicodeDecodeError
                         | Raised when a Unicode-related error occurs during decoding.
                         |
| UnicodeTranslateError
                         | Raised when a Unicode-related error occurs during translation.
                         |
| ValueError
                         | Raised when a function gets an argument of correct type but improper value.
                         |
| ZeroDivisionError
                         | Raised when the second operand of a division or module operation is zero.
                         |