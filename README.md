# 0x00. Pascal's Triangle

## Algorithm | Python

### Project Overview
This project involves generating Pascal's Triangle using Python. Pascal’s Triangle is a mathematical structure where each number is the sum of the two directly above it. The goal is to implement a function that takes an integer `n` and returns a list of lists representing the first `n` rows of Pascal’s Triangle.


## Learning Objectives
To successfully complete this project, you should have a solid understanding of the following Python concepts:

- **Lists and List Comprehensions**:
  - How to create, access, modify, and iterate over lists.
  - Using list comprehensions for concise and readable code, particularly for generating rows of Pascal’s Triangle.

- **Functions**:
  - Defining and calling functions.
  - Passing parameters and returning values, especially lists of lists representing Pascal’s Triangle.

- **Loops**:
  - Using `for` and `while` loops to iterate through sequences.
  - Utilizing nested loops for generating each row and calculating values.

- **Conditional Statements**:
  - Implementing `if`, `elif`, and `else` conditions to handle edge cases (e.g., the edges of the triangle always being 1).

- **Recursion (Optional)**:
  - While not strictly necessary, recursion can provide an alternative approach to generating Pascal’s Triangle.

- **Arithmetic Operations**:
  - Performing addition to calculate each element of Pascal’s Triangle as the sum of the two elements directly above it.

- **Indexing and Slicing**:
  - Accessing elements and slices of lists, crucial for identifying and summing the correct elements when constructing each row.

- **Memory Management**:
  - Understanding how lists are stored and copied, especially when creating new rows based on values of the previous row.

- **Error and Exception Handling (Optional)**:
  - Using `try-except` blocks as needed to handle potential errors, such as invalid input types or values.

- **Efficiency and Optimization**:
  - Evaluating time and space complexity of different approaches.
  - Applying optimizations to improve the performance of the solution.

By revisiting these concepts, you will be well-prepared to implement Pascal’s Triangle using Python, combining your mathematical understanding with programming skills to develop an efficient and effective solution.

---

## Resources
- [What is Pascal’s Triangle](https://en.wikipedia.org/wiki/Pascal%27s_triangle)
- [Pascal’s Triangle - Numberphile](https://www.youtube.com/watch?v=XMriWTvPXHI)
- [What are Python Algorithms](https://realpython.com/tutorials/algorithms/)

### Additional Resources
- [Mock Technical Interview](#)
- **Must Know Concepts**: See the learning objectives above for a detailed breakdown.

---

## Task: Pascal's Triangle

### Task 0: Pascal's Triangle
Create a function `def pascal_triangle(n):` that returns a list of lists of integers representing the Pascal’s triangle of `n`:

- **Returns an empty list if `n <= 0`.**
- **Assume `n` is always an integer.**

Example:

```bash
guillaume@ubuntu:~/0x00$ cat 0-main.py
#!/usr/bin/python3
"""
0-main
"""
pascal_triangle = __import__('0-pascal_triangle').pascal_triangle

def print_triangle(triangle):
    """
    Print the triangle
    """
    for row in triangle:
        print("[{}]".format(",".join([str(x) for x in row])))


if __name__ == "__main__":
    print_triangle(pascal_triangle(5))
