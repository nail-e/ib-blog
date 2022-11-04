---
layout: post
permalink: /blog/04-11-2022-getting-the-complexity-mark-in-the-computer-science-ia/
title:  Getting the 'complexity' mark in the Computer Science IA 
---
The complex complexity mark in the IA is a really hard topic to get a grasp on. In order to successfully get that 12 marks in the IA, you need 8/16 aspects in HL and 10/15 aspects in SL. If you're not Elian and are someone else whose using this as a guide, this post is formatted in such a way so you can keep track of what you're doing while coding.

---

## Table of Contents
- [Table of Contents](#table-of-contents)
- [**HL Criteria**](#hl-criteria)
- [**SL Criteria**](#sl-criteria)


## **HL Criteria**
1. Adding/deleting data to an instance of the RandomAccessFile class by direct manipulation of the file pointer using the seek method
2. Searching for specified data in a file
3. Recursion
4. Merging two or more sorted data structures
5. Polymorphism
6. Inheritance
7. Encapsulation
8. Parsing a text file or other data stream
9.  Hirearchal data structures
10.  Inserting/deleting data into an ordered sequential file without reading the entire file into RAM
11.  2D (or more) Arrays
    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;12 to 16. Requires at least one Abstract Data Types (ADTs) with methods that can be called.

| Abstract Data Type   |  1 Aspect | 2 Aspects  |  3 Aspects |  4 Aspects |  Probable Methods | 
| ------------ | ------------ | ------------ | ------------ | ------------ | ------------ |
 *General Criteria*  | *An incomplete ADT is implemented* |  *An ADT is implemented with all key methods implemented.* | *An ADT is implemented thatincludes some error checking*  |  A*n ADT is implemented completely and robust*  | -  |
  **Lists** |  A node style class with appropriate constructors and methods to set and get data elements. |  Methods are implemented to add at / remove from the tail and the head of the list. |  Proper checks are made for errors such as attempting to get an element from an empty list or inserting the same element twice. | All error conditions are checked for, and all appropriate methods are implemented.  | `size, isEmpty, first, last, before, after, insertHead, insertTail, insertBefore, insertAfter`  |
   **Tree**| A class or interface with appropriate constructors and methods to set and get data elements.  | Methods are implemented to add at / remove from the correct point in the tree.  |  Proper checks are made for errors such as attempting to get an element from an empty tree or not inserting the same element twice. | All error conditions are checked for, all appropriate methods are implemented.  | `size, isEmpty, root, parent, leftChild, rightChild`  |
  **Stack** |  A class or interface with appropriate constructors and methods to push and pop items. |  Methods to test for full and empty stack are added. | Proper checks are made for errors such as attempting to get an element from an empty stack.  |   |  `push, pop, top, isEmpty, isFull, size`  |
  **Queue** | A class or interface with appropriate constructors and methods to enqueue and dequeue items.  | Methods to test for full and empty queue are added.  |   Proper checks are made for errors such as attempting to get an element from an empty queue. |   | `enqueue, dequeue, front, rear, isEmpty, isFull, size`  |
   **Hash Table**| A class or interface with appropriate constructors and methods to insert and remove items.  |  Methods to test for full table and duplicate keys are added. | Proper checks are made for errors such as attempting to get a non-existent key, clashes are dealt with properly  |   | `hashFunction, insertKey, removeKey, isDuplicate, isEmpty, isFull, size`  |


## **SL Criteria**
1. Arrays
2. Objects
3. Objects as data records
4. Selection (If-Else) statements
5. Selection Statements with operators and nests or Switch/Cases 
6. Loops
7. Nested loops
8. Methods
9. Methods with parameters (the parameters have to be useful and used within the method body)
10. User-defined methods with appropriate return values (primitives or objects)
11. Sorting
12. Searching
13. File I/O
14. Importing libraries
15. Flags/Sentinels