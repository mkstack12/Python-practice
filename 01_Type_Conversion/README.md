# Python Type Conversion

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Topic](https://img.shields.io/badge/Topic-Type%20Conversion-orange)
![Level](https://img.shields.io/badge/Level-Beginner-success)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

## 1. Introduction

Type Conversion is the process of changing a value from one data type to another data type.

It is also known as **Type Casting**.

Python provides built-in functions to convert values between different data types, such as integers, floats, strings, and booleans.

**Example:**

```python
a = "100"
b = int(a)

print(b)
print(type(b))
```

**Output:**

```text
100
<class 'int'>
```

Here, the string `"100"` is converted into an integer using the `int()` function.

---

## 2. Learning Objectives

After completing this topic, you will be able to:

- Understand the concept of Type Conversion.
- Check the data type using `type()`.
- Convert strings into integers.
- Convert integers into floats.
- Convert numbers into strings.
- Understand invalid type conversions.
- Use type conversion with user input.
- Perform arithmetic operations on converted values.

---

## 3. Checking Data Types

Python provides the built-in `type()` function to identify the data type of a variable or value.

**Syntax:**

```python
type(variable)
```

**Example:**

```python
a = 10
b = 4.2
c = "Hello"
d = True

print(type(a))
print(type(b))
print(type(c))
print(type(d))
```

**Output:**

```text
<class 'int'>
<class 'float'>
<class 'str'>
<class 'bool'>
```

**Explanation:**

| Value | Data Type |
|---|---|
| `10` | Integer |
| `4.2` | Float |
| `"Hello"` | String |
| `True` | Boolean |

---

## 4. Types of Type Conversion

Python supports two main types of conversion:

### 4.1 Implicit Type Conversion

Implicit conversion happens automatically when Python converts one data type into another compatible data type.

**Example:**

```python
a = 10
b = 2.5

result = a + b

print(result)
print(type(result))
```

**Output:**

```text
12.5
<class 'float'>
```

Here, Python automatically converts the integer into a float during the operation.

### 4.2 Explicit Type Conversion

Explicit conversion happens when the programmer manually converts a value using built-in functions.

**Example:**

```python
a = "25"
b = int(a)

print(b)
print(type(b))
```

**Output:**

```text
25
<class 'int'>
```

Here, the programmer manually converts a string into an integer.

---

## 5. Important Type Conversion Functions

Python provides several built-in functions for converting data types.

| Function | Description | Example |
|---|---|---|
| `int()` | Converts to integer | `int("10")` |
| `float()` | Converts to float | `float("5.5")` |
| `str()` | Converts to string | `str(100)` |
| `bool()` | Converts to boolean | `bool(1)` |

---

## 6. String to Integer Conversion

The `int()` function converts a valid integer string into an integer.

**Example:**

```python
a = "5"
a = int(a)

print(type(a))
print(a)
```

**Output:**

```text
<class 'int'>
5
```

**Explanation:**

- Initially, `a` contains a string.
- The `int()` function converts the string into an integer.
- The converted value can now be used in mathematical operations.

### Invalid Integer Conversion

A string containing non-numeric characters cannot be directly converted into an integer.

**Example 1:**

```python
a = "Five"
a = int(a)

print(a)
```

**Output:**

```text
ValueError
```

**Example 2:**

```python
a = "5.0"
a = int(a)

print(a)
```

**Output:**

```text
ValueError
```

**Important:** The `int()` function does not directly convert a decimal string such as `"5.0"` into an integer.

---

## 7. Integer to Float Conversion

The `float()` function converts an integer into a floating-point number.

**Example:**

```python
a = 10
a = float(a)

print(a)
print(type(a))
```

**Output:**

```text
10.0
<class 'float'>
```

---

## 8. Float to Integer Conversion

The `int()` function converts a float into an integer by removing its decimal part. It does not round the number.

**Example:**

```python
a = 5.9
b = int(a)

print(b)
```

**Output:**

```text
5
```

---

## 9. Integer to String Conversion

The `str()` function converts a value into a string.

**Example:**

```python
a = 100
a = str(a)

print(type(a))
print(a)
```

**Output:**

```text
<class 'str'>
100
```

---

## 10. Adding Two Numbers Using Type Conversion

The `input()` function always returns user input as a string.

Therefore, we use `int()` to convert the input into integers before performing addition.

**Example:**

```python
a = input()
a = int(a)

b = input()
b = int(b)

result = a + b

print(result)
```

**Input:**

```text
2
3
```

**Output:**

```text
5
```

**Explanation:**

1. Take the first number as input.
2. Convert it into an integer.
3. Take the second number as input.
4. Convert it into an integer.
5. Add both numbers.
6. Print the result.

---

## 11. Using String Conversion with Output

Sometimes we need to combine numbers and strings.

The `str()` function helps convert a number into a string before concatenation.

**Example:**

```python
a = int(input())
b = int(input())

result = a + b

print("Sum: " + str(result))
```

**Input:**

```text
2
3
```

**Output:**

```text
Sum: 5
```

---

## 12. Boolean Conversion

The `bool()` function converts a value into either `True` or `False`.

**Example:**

```python
print(bool(1))
print(bool(0))
print(bool("Hello"))
print(bool(""))
```

**Output:**

```text
True
False
True
False
```

**Important Points:**

- Zero is converted to `False`.
- Non-zero numbers are converted to `True`.
- An empty string is converted to `False`.
- A non-empty string is converted to `True`.

---

## 13. Common Mistakes

| Mistake | Correct Understanding |
|---|---|
| `int("Five")` | Invalid conversion |
| `int("5.0")` | Invalid direct conversion |
| Adding two input values directly | Convert them first |
| `int(5.9)` gives 6 | It actually gives 5 |
| `bool("False")` gives False | It actually gives True |

---

## 14. Practice Questions

Try solving these questions without looking at the solutions.

1. Convert the string `"100"` into an integer.
2. Convert an integer into a float.
3. Convert a float into an integer.
4. Convert an integer into a string.
5. Check the data type of four different variables.
6. Take two numbers as input and print their sum.
7. Take a decimal number as input and convert it into an integer.
8. Check the boolean values of `0`, `1`, `""`, and `"Python"`.

---

## 15. Quick Revision

| Function | Purpose |
|---|---|
| `type()` | Checks the data type |
| `int()` | Converts into integer |
| `float()` | Converts into float |
| `str()` | Converts into string |
| `bool()` | Converts into boolean |

### Key Takeaways

- Type Conversion changes one data type into another.
- `type()` identifies the data type of a value.
- `input()` returns data as a string.
- Explicit conversion is performed using functions like `int()` and `float()`.
- Invalid conversions may raise a `ValueError`.

---

## 16. Repository Files

The following Python files contain practical examples of this topic:

```text
01_Type_Conversion/
│
├── README.md
├── type_conversion.py
├── type_checking.py
├── invalid_conversion.py
└── add_two_numbers.py
```

---

**Topic:** Python Type Conversion  
**Difficulty:** Beginner  
**Learning Status:** Completed

*This documentation is part of my daily Python learning and practice journey.*
