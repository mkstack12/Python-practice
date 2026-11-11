# Division of Two Numbers

![Python](https://img.shields.io/badge/Language-Python%203.10-blue?logo=python)
![Difficulty](https://img.shields.io/badge/Difficulty-Easy-success)
![Topic](https://img.shields.io/badge/Topic-Arithmetic%20Operations-orange)
![Status](https://img.shields.io/badge/Status-Solved-brightgreen)

## 1. Problem Statement

Write a Python program that reads two numbers A and B and prints the division of the two numbers (A / B).

The program should calculate the result using the division operator and display the result as a floating-point number.

## 2. Input Format

- The first line of input contains an integer A.
- The second line of input contains an integer B.

## 3. Output Format

Print a single line containing the floating-point result obtained by dividing the first number by the second number.

## 4. Sample Test Cases

### Sample Input 1

```text
15
3
```

### Sample Output 1

```text
5.0
```

**Explanation:**

The given numbers are 15 and 3.

\[
15 \div 3 = 5.0
\]

### Sample Input 2

```text
5
2
```

### Sample Output 2

```text
2.5
```

**Explanation:**

\[
5 \div 2 = 2.5
\]

## 5. Approach

1. Take the first number as input.
2. Convert the input into an integer using `int()`.
3. Take the second number as input.
4. Convert it into an integer.
5. Divide the first number by the second number using `/`.
6. Print the result.

## 6. Python Concepts Used

| Concept | Description |
|---|---|
| `input()` | Accepts user input |
| `int()` | Converts input into an integer |
| `/` | Performs division |
| `print()` | Displays the result |

## 7. Python Solution

The complete implementation is available in `solution.py`.

```python
a = int(input())
b = int(input())

print(a / b)
```

## 8. Code Explanation

**Line 1:**
```python
a = int(input())
```
Takes the first number and converts it into an integer.

**Line 2:**
```python
b = int(input())
```
Takes the second number and converts it into an integer.

**Line 3:**
```python
print(a / b)
```
Divides both numbers and prints the result.

In Python, the `/` operator returns a floating-point result.

## 9. Complexity Analysis

- **Time Complexity:** O(1)
- **Space Complexity:** O(1)

The program performs a fixed number of operations, regardless of the input size.

## 10. Key Learnings

- Taking multiple inputs in Python.
- Converting strings into integers.
- Using arithmetic operators.
- Performing division using `/`.
- Understanding floating-point output.

## 11. Important Note

The second number must not be zero because division by zero raises a `ZeroDivisionError`.

---

**Problem:** Division of Two Numbers

**Language:** Python 3.10

**Difficulty:** Easy

**Status:** Solved

*Part of my daily Python coding practice and problem-solving journey.*
