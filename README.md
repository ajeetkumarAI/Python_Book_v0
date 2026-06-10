# Python: The Definitive Guide — From Zero to Data Science and AI

### *A Comprehensive, Illustrative Academic Textbook with Extensive Practice, Assignments, and Certification Preparation*

**Chapters:** 75 | **Target Audience:** Beginners to Advanced Learners

---

**Preface**

This book is a structured, comprehensive, and in-depth guide to the Python programming language, written in an academic tone for educational purposes. It is designed for:

- **Students** preparing for Python programming courses and examinations
- **Self-learners** building skills for careers in Data Science, Machine Learning, and AI
- **Professionals** preparing for Python certification exams (PCEP, PCAP, PCPP)
- **Educators** seeking a reference textbook for Python instruction

Every concept is explained from first principles with:
- **Detailed theory** explaining what each concept is, why it exists, and how Python implements it
- **Formal syntax** shown before every concept
- **Extensive practice examples** with expected outputs (taken directly from classroom notebooks)
- Visual diagrams and comparison tables
- **⚠️ Key Insights & Common Mistakes** sections after every topic
- **📝 Assignment questions (3–5) after every topic** for self-assessment
- Practical insights bridging theory to Data Science and AI applications
- Certification exam tips and common interview questions

**How to Use This Book:**
1. Read each chapter sequentially — concepts build on previous chapters
2. **Type and execute every code example yourself** — do not just read
3. Pay special attention to the ⚠️ Key Insights boxes — they highlight mistakes that even experienced programmers make
4. Attempt all 📝 Assignment questions before checking answers
5. Complete the certification practice questions at the end

---

## Table of Contents

**Part I: Getting Started with Python** — Chapters 1–8
**Part II: Operators and Expressions** — Chapters 9–15
**Part III: Strings — Text Processing Mastery** — Chapters 16–19
**Part IV: Control Flow** — Chapters 20–25
**Part V: Core Data Structures** — Chapters 26–32
**Part VI: Functions — The Building Blocks** — Chapters 33–39
**Part VII: Modules, Packages, and Virtual Environments** — Chapters 40–44
**Part VIII: File Handling and Data Persistence** — Chapters 45–47
**Part IX: Error and Exception Handling** — Chapters 48–50
**Part X: Regular Expressions** — Chapters 51–52
**Part XI: Object-Oriented Programming** — Chapters 53–61
**Part XII: Advanced Python** — Chapters 62–69
**Part XIII: Python for Data Science — A Bridge** — Chapters 70–72
**Part XIV: Professional Python** — Chapters 73–75
**Appendices** — A through E

---

# Part I: Getting Started with Python

---

## Chapter 1: Introduction to Python

### 1.1 Theory

Python is a **high-level, interpreted, general-purpose programming language** created by **Guido van Rossum** in 1991. It is named after the British comedy group *Monty Python*. Python emphasises **readability** and **simplicity**, making it one of the best languages for beginners.

**Why Python?**
- Python is used in **Data Science, Machine Learning, Artificial Intelligence, Web Development, Automation, and Scientific Computing**
- It has a massive ecosystem of libraries: NumPy, Pandas, Scikit-learn, TensorFlow, PyTorch, Django, Flask
- It is the #1 language in Stack Overflow Developer Surveys for learning and data-related work
- It has a simple, English-like syntax that reduces development time

**Key Features of Python:**

| Feature | Description |
|---------|------------|
| High-Level | Abstracted from hardware; no memory management needed |
| Interpreted | Executed line by line (no compilation step needed) |
| Dynamically Typed | No need to declare variable types; determined at runtime |
| Object-Oriented | Supports classes, inheritance, encapsulation, polymorphism |
| Platform Independent | Same code runs on Windows, macOS, Linux |
| Extensive Libraries | NumPy, Pandas, TensorFlow, Scikit-learn, etc. |
| Open Source | Free to use, modify, and distribute |
| Community Support | Millions of developers and resources worldwide |

**Python vs. Other Languages:**

| Feature | Python | Java | C++ |
|---------|--------|------|-----|
| Typing | Dynamic | Static | Static |
| Syntax | Simple, concise | Verbose | Complex |
| Compilation | Interpreted | Compiled to bytecode | Compiled to machine code |
| Memory Management | Automatic (garbage collected) | Automatic (GC) | Manual |
| Speed | Slower (interpreted) | Faster | Fastest |
| Learning Curve | Easy | Moderate | Steep |

> **⚠️ Key Insights & Common Mistakes**
> - Python is **interpreted**, meaning it is executed line by line. If there is an error on line 10, lines 1–9 will still execute.
> - Python is **dynamically typed** — you don't declare types, but this can lead to unexpected `TypeError`s at runtime.
> - Python uses **indentation** (whitespace) to define code blocks, NOT curly braces like Java or C++. This is not optional — wrong indentation causes `IndentationError`.
> - Python 2 and Python 3 are **not fully compatible**. Always use Python 3 (Python 2 is officially deprecated since January 2020).

---

### 📝 Assignment Questions — Chapter 1

1. List five key features of Python that make it suitable for Data Science.
2. What does "dynamically typed" mean? How is it different from "statically typed"?
3. What is the difference between an interpreted and a compiled language?
4. Why is Python slower than C++ despite being easier to write?
5. Who created Python and in what year?

---

## Chapter 2: Setting Up the Python Environment

### 2.1 Theory

Before you can write Python code, you need to install Python on your computer. Python can be installed directly from [python.org](https://www.python.org) or through the **Anaconda distribution** (recommended for Data Science because it includes NumPy, Pandas, Jupyter Notebook, and 250+ packages pre-installed).

**Installation Options:**

| Method | Best For | Includes |
|--------|---------|----------|
| python.org | General development | Python + pip |
| Anaconda | Data Science / AI | Python + 250+ packages + Jupyter + conda |
| Google Colab | Quick experimentation | Browser-based, no install needed |

### 2.2 Verifying Installation

**Syntax:**
```bash
python --version
# or
python3 --version
```

**Example Output:**
```
Python 3.12.0
```

### 2.3 Running Python

There are three ways to run Python code:

**1. Interactive Mode (Python Shell/REPL):**
```bash
$ python3
>>> print('Hello, World!')
Hello, World!
>>> 2 + 3
5
>>> exit()
```

**2. Script Mode (saving to a .py file):**
```bash
# Create a file called hello.py
# Run it:
$ python3 hello.py
```

**3. Jupyter Notebook (recommended for learning and Data Science):**
```bash
$ jupyter notebook
# Opens in browser, create a new notebook, write code in cells
```

> **⚠️ Key Insights & Common Mistakes**
> - On some systems, `python` refers to Python 2 and `python3` refers to Python 3. Always check with `python --version`.
> - For Data Science, **Anaconda** is the recommended installation because it includes all essential packages.
> - **Google Colab** (colab.research.google.com) is free and requires no installation — excellent for beginners.

---

### 📝 Assignment Questions — Chapter 2

1. What is the difference between installing Python from python.org vs. Anaconda?
2. How do you verify which version of Python is installed on your system?
3. What are the three ways to run Python code?
4. What is the advantage of using Jupyter Notebook for Data Science?
5. What is Google Colab and when would you use it?

---

## Chapter 3: Introduction to Jupyter Notebook

### 3.1 Theory

**Jupyter Notebook** is an open-source web application that allows you to create documents containing **live code, equations, visualisations, and narrative text**. It is the most popular tool for Data Science and Machine Learning.

The name "Jupyter" comes from three languages: **Ju**lia, **Py**thon, **R**.

**Key Features:**
- Write and execute code **cell by cell** (not all at once)
- See output immediately below each cell
- Mix code with **Markdown** text, images, and LaTeX equations
- Export to PDF, HTML, slides
- Share notebooks easily (`.ipynb` files)

### 3.2 Notebook Interface

| Element | Description |
|---------|------------|
| Cell | A container for code or text |
| Code Cell | Contains executable Python code |
| Markdown Cell | Contains formatted text, headings, lists |
| Kernel | The Python engine running your code |

### 3.3 Essential Keyboard Shortcuts

| Shortcut | Action |
|----------|--------|
| `Shift + Enter` | Run cell and move to next |
| `Ctrl + Enter` | Run cell and stay |
| `Alt + Enter` | Run cell and insert new below |
| `Esc + A` | Insert cell above |
| `Esc + B` | Insert cell below |
| `Esc + DD` | Delete cell |
| `Esc + M` | Change cell to Markdown |
| `Esc + Y` | Change cell to Code |

> **⚠️ Key Insights & Common Mistakes**
> - Cells can be run **out of order** in Jupyter. This can cause confusion if you run cell 5 before cell 3. Always use **Kernel → Restart & Run All** to verify your notebook works from top to bottom.
> - Variables persist across cells in the same session. If you define `x = 5` in one cell, you can use `x` in any cell below.
> - Don't forget to save your notebook (`Ctrl + S`). Jupyter does autosave, but save manually before closing.

---

### 📝 Assignment Questions — Chapter 3

1. What does the name "Jupyter" stand for?
2. What is the difference between a Code cell and a Markdown cell?
3. What keyboard shortcut runs the current cell and moves to the next one?
4. Why is it important to use "Restart & Run All" in Jupyter?
5. What is the file extension of a Jupyter Notebook?

---

## Chapter 4: Comments, Indentation, and Code Style (PEP 8)

### 4.1 Theory — Comments

**Comments** are lines in code that Python ignores during execution. They are written for **humans** — to explain what the code does, why certain decisions were made, or to temporarily disable code during debugging.

### 4.2 Syntax

```python
# Single-line comment (starts with #)

'''
Multi-line comment
using triple single quotes
'''

"""
Multi-line comment
using triple double quotes
"""
```

### 4.3 Practice Examples

```python
# This is a single line comment
print('Hello')    # This is an inline comment

# Output:
# Hello
```

```python
'''
This is a multi-line comment.
It can span multiple lines.
Python ignores everything inside triple quotes
(when not assigned to a variable).
'''
print('Data Science')

# Output:
# Data Science
```

```python
"""
Author: x Academy
Date: 2025
Purpose: Python fundamentals
"""
x = 10
print(x)

# Output:
# 10
```

### 4.4 Theory — Indentation

**Indentation** in Python is **not optional** — it is part of the syntax. Python uses indentation (whitespace at the beginning of a line) to define code blocks. Other languages use curly braces `{}`, but Python uses indentation.

**Rules:**
- Standard indentation is **4 spaces** (recommended by PEP 8)
- All statements within a block must have the **same** indentation level
- Mixing **tabs and spaces** causes `TabError`
- Incorrect indentation causes `IndentationError`

### 4.5 Indentation Examples

```python
# Correct indentation
if True:
    print('Inside if block')    # 4 spaces indent
    print('Still inside')       # Same 4 spaces

# Output:
# Inside if block
# Still inside
```

```python
# WRONG — inconsistent indentation
if True:
    print('Line 1')
      print('Line 2')    # IndentationError! Extra spaces
```

```python
# WRONG — missing indentation
if True:
print('Hello')    # IndentationError! Expected an indented block
```

### 4.6 Theory — PEP 8 Style Guide

**PEP 8** is the official Python style guide. Following PEP 8 makes your code readable and consistent.

**Key PEP 8 Rules:**

| Rule | Example |
|------|---------|
| Use 4 spaces per indentation level | `if True:` then 4 spaces |
| Maximum line length: 79 characters | Break long lines |
| Use `snake_case` for variables/functions | `my_variable`, `calculate_total()` |
| Use `PascalCase` for class names | `MyClass`, `StudentRecord` |
| Use `UPPER_CASE` for constants | `MAX_SIZE = 100` |
| Two blank lines before function/class definitions | — |
| One blank line between methods inside a class | — |
| Spaces around operators: `x = 5`, not `x=5` | — |

> **⚠️ Key Insights & Common Mistakes**
> - **Indentation is mandatory in Python** — it defines code blocks. Forgetting indentation or using inconsistent indentation causes `IndentationError`.
> - **Never mix tabs and spaces** — this causes `TabError`. Configure your editor to use 4 spaces when you press Tab.
> - Comments should explain **why**, not **what**. `# increment x` is useless; `# retry after timeout` is useful.
> - Triple-quoted strings are technically **string literals**, not comments. If assigned to a variable, they create a string object in memory.

---

### 📝 Assignment Questions — Chapter 4

1. What is the difference between a single-line comment and a multi-line comment?
2. What error does Python raise if indentation is incorrect?
3. What is PEP 8? Name five rules from PEP 8.
4. Why should you never mix tabs and spaces in Python?
5. What is the recommended number of spaces for indentation?

---

## Chapter 5: The `print()` Function and Output Formatting

### 5.1 Theory

The `print()` function is the **most fundamental output function** in Python. It displays text, variables, and expressions to the console (standard output). Understanding `print()` is essential because it is the primary way to see the results of your code.

### 5.2 Syntax

```python
print(value1, value2, ..., sep=' ', end='\n', file=sys.stdout, flush=False)
```

| Parameter | Description | Default |
|-----------|------------|---------|
| `value1, value2, ...` | Values to print (any number) | — |
| `sep` | Separator between values | `' '` (single space) |
| `end` | What to print at the end | `'\n'` (newline) |
| `file` | Output stream | `sys.stdout` (console) |
| `flush` | Force flush the stream | `False` |

### 5.3 Extensive Practice Examples 

#### Basic Printing

```python
a = 100
b = 200
c = 'Data Science'
d = 'Machine Learning'

print(c)
print(d)
```
**Output:**
```
Data Science
Machine Learning
```

#### Printing Multiple Values

```python
a = 100
b = 200
x = 300
print(a, b, x)
```
**Output:**
```
100 200 300
```

#### Using `sep` Parameter — Changing the Separator

```python
a, b, x = 100, 200, 300

print(a, b, x, sep=' ')      # Default separator (space)
# Output: 100 200 300

print(a, b, x, sep='+')
# Output: 100+200+300

print(a, b, x, sep='-')
# Output: 100-200-300

print(a, b, x, sep='---')
# Output: 100---200---300

print(a, b, x, sep=' , ')
# Output: 100 , 200 , 300

print(a, b, x, sep='\n')
# Output:
# 100
# 200
# 300

print(a, b, x, sep='\t')
# Output: 100	200	300
```

#### Using `end` Parameter — Changing the Line Ending

```python
print(100, end=' ')
print(200, end=' ')
print(300)
# Output: 100 200 300

print('Hello', end='...')
print('World')
# Output: Hello...World

print('A', end=' -> ')
print('B', end=' -> ')
print('C')
# Output: A -> B -> C
```

#### Escape Sequences

```python
print('Hello\nWorld')          # \n = Newline
# Output:
# Hello
# World

print('Hello\tWorld')          # \t = Tab
# Output: Hello	World

print('It\'s Python')          # \' = Single quote
# Output: It's Python

print("She said \"Hello\"")   # \" = Double quote
# Output: She said "Hello"

print('C:\\Users\\Desktop')    # \\ = Backslash
# Output: C:\Users\Desktop
```

#### Common Escape Sequences Table

| Escape | Meaning |
|--------|---------|
| `\n` | Newline |
| `\t` | Tab |
| `\\` | Backslash |
| `\'` | Single quote |
| `\"` | Double quote |
| `\r` | Carriage return |
| `\b` | Backspace |

#### Printing with No Arguments

```python
print()    # Prints a blank line (just \n)
print('Above')
print()
print('Below')
# Output:
# Above
#
# Below
```

#### String Formatting with f-strings

```python
name = 'Alice'
age = 25
salary = 50000.5

print(f'Name: {name}, Age: {age}')
# Output: Name: Alice, Age: 25

print(f'Salary: {salary:.2f}')
# Output: Salary: 50000.50

print(f'{name!r}')
# Output: 'Alice'

# f-string with expressions
print(f'2 + 3 = {2 + 3}')
# Output: 2 + 3 = 5

# Debugging with = (Python 3.8+)
x = 42
print(f'{x = }')
# Output: x = 42
```

#### Old-Style Formatting (for reference)

```python
# % formatting
print('Name: %s, Age: %d' % ('Alice', 25))
# Output: Name: Alice, Age: 25

# .format() method
print('Name: {}, Age: {}'.format('Alice', 25))
# Output: Name: Alice, Age: 25

print('Name: {0}, Age: {1}, Name again: {0}'.format('Alice', 25))
# Output: Name: Alice, Age: 25, Name again: Alice
```

> **⚠️ Key Insights & Common Mistakes**
> - `print()` with no arguments prints a **blank line** (just the default `\n`).
> - The default `sep` is a single space `' '`, NOT no separator. `print(1, 2)` outputs `1 2`, not `12`.
> - The default `end` is `'\n'` (newline). Change it with `end=''` to print on the same line.
> - Use **f-strings** (f'...') for formatting — they are the most readable and fastest method. **Forgetting the `f` before the string** is a very common mistake: `'{name}'` prints the literal text `{name}`, not the value!
> - `\n` inside a string creates a newline. `\\n` prints the literal characters `\n`.
> - `print(a, b, c)` prints with spaces. `print(str(a) + str(b) + str(c))` prints with no spaces (concatenation).

---

### 📝 Assignment Questions — Chapter 5

1. What is the default value of `sep` and `end` in `print()`?
2. Write a `print()` statement that outputs: `10->20->30->40` (using `sep`).
3. What is the difference between `\n`, `\t`, and `\\`?
4. Write three different ways to format the string "Hello, Alice! You are 25 years old."
5. What happens if you forget the `f` prefix in an f-string?

---

## Chapter 6: Variables, Identifiers, and Memory Model

### 6.1 Theory

A **variable** is a name that refers to a value stored in memory. In Python, variables are **labels** (references) pointing to objects in memory — they don't store the value directly.

**Key Concept:** In Python, **everything is an object**. When you write `x = 5`, Python creates an integer object `5` in memory, and `x` becomes a label pointing to that object.

### 6.2 Syntax

```python
variable_name = value
```

**Rules for Variable Names (Identifiers):**
1. Must start with a **letter** (a–z, A–Z) or **underscore** (`_`)
2. Can contain letters, digits (0–9), and underscores
3. **Cannot start with a digit**
4. **Cannot be a Python keyword** (reserved word)
5. **Case-sensitive**: `name`, `Name`, and `NAME` are different variables
6. No spaces allowed in variable names
7. No special characters except underscore (`_`)

### 6.3 Practice Examples 

```python
# Valid variable names
student_name = 'Alice'
_count = 10
myAge = 25
MAX_SIZE = 100
x1 = 5.0

# Invalid variable names (will cause errors)
# 1name = 'Alice'       # SyntaxError: cannot start with digit
# my name = 'Alice'     # SyntaxError: spaces not allowed
# class = 'Python'      # SyntaxError: 'class' is a reserved keyword
# my-var = 10           # SyntaxError: hyphens not allowed
```

```python
# Variables are case-sensitive
name = 'Alice'
Name = 'Bob'
NAME = 'Charlie'

print(name)    # Alice
print(Name)    # Bob
print(NAME)    # Charlie
```

```python
# Multiple assignment
a, b, c = 10, 20, 30
print(a, b, c)    # 10 20 30

# Same value to multiple variables
x = y = z = 100
print(x, y, z)    # 100 100 100

# Swapping values (Python's elegant way)
a, b = 10, 20
a, b = b, a
print(a, b)    # 20 10
```

```python
# Dynamic typing — type changes when value changes
x = 10
print(type(x))    # <class 'int'>

x = 'Hello'
print(type(x))    # <class 'str'>

x = [1, 2, 3]
print(type(x))    # <class 'list'>
```

### 6.4 Python Keywords (Reserved Words)

```python
import keyword
print(keyword.kwlist)
```

| Keywords | | | | |
|----------|--|--|--|--|
| `False` | `True` | `None` | `and` | `or` |
| `not` | `if` | `elif` | `else` | `for` |
| `while` | `break` | `continue` | `pass` | `return` |
| `def` | `class` | `import` | `from` | `as` |
| `try` | `except` | `finally` | `raise` | `with` |
| `yield` | `lambda` | `global` | `nonlocal` | `del` |
| `in` | `is` | `assert` | `async` | `await` |

### 6.5 Memory Model — `id()` and `is`

```python
a = 256
b = 256
print(a is b)       # True (Python caches integers -5 to 256)
print(id(a), id(b)) # Same id!

a = 257
b = 257
print(a is b)       # May be False (outside cache range)

# Lists always create new objects
x = [1, 2, 3]
y = [1, 2, 3]
print(x == y)    # True (same values)
print(x is y)    # False (different objects in memory!)
```

> **⚠️ Key Insights & Common Mistakes**
> - Variable names are **case-sensitive**: `Name` and `name` are different variables.
> - **Never use Python keywords as variable names** (e.g., `list = [1,2,3]`). This shadows the built-in and causes unexpected errors. If you accidentally do this, use `del list` to fix it.
> - **Never name your variable the same as a built-in function**: `int = 5` means you can't use `int()` anymore! Use `del int` to fix it.
> - `==` checks **value equality**. `is` checks **identity** (same object in memory). Use `==` for comparisons, `is` only for `None` checks (`if x is None`).
> - Python caches small integers (-5 to 256) and short strings. So `a = 256; b = 256; a is b` is `True`, but `a = 257; b = 257; a is b` may be `False`.

---

### 📝 Assignment Questions — Chapter 6

1. What are the rules for naming a variable in Python?
2. What is the difference between `==` and `is`?
3. What happens if you use `int = 5` and then try `int('10')`? How do you fix it?
4. Write code to swap two variables without a temporary variable.
5. Why is Python called "dynamically typed"? Demonstrate with an example.

---

## Chapter 7: Data Types — A Complete Overview

### 7.1 Theory

A **data type** defines the kind of value a variable holds and what operations can be performed on it. Python has a rich set of built-in data types. Understanding data types is fundamental because it determines what you can do with your data.

**Python Data Types Classification:**

| Category | Data Types |
|----------|-----------|
| **Numeric** | `int`, `float`, `complex` |
| **Text** | `str` |
| **Sequence** | `list`, `tuple`, `range` |
| **Set** | `set`, `frozenset` |
| **Mapping** | `dict` |
| **Boolean** | `bool` (`True`, `False`) |
| **Binary** | `bytes`, `bytearray`, `memoryview` |
| **None** | `NoneType` |

### 7.2 Syntax — Creating Each Data Type

```python
# Numeric Types
integer_var = variable_name = integer_value       # int
float_var = variable_name = decimal_value          # float
complex_var = variable_name = real + imaginaryj    # complex

# Text
string_var = 'text'  # or "text" or '''text''' or """text"""

# Sequence Types
list_var = [item1, item2, ...]         # list (mutable)
tuple_var = (item1, item2, ...)        # tuple (immutable)
range_var = range(start, stop, step)   # range

# Set Types
set_var = {item1, item2, ...}          # set (mutable, no duplicates)
frozenset_var = frozenset({...})       # frozenset (immutable set)

# Mapping
dict_var = {key1: value1, key2: value2}  # dict

# Boolean
bool_var = True  # or False
```

### 7.3 Extensive Practice Examples 

```python
# int
int1 = 56
print(type(int1), int1)
# Output: <class 'int'> 56
```

```python
# float
f1 = 4.56
print(type(f1), f1)
# Output: <class 'float'> 4.56
```

```python
# complex (a + bj where j is the imaginary unit)
c1 = 4.5 + 2j
print(type(c1), c1)
# Output: <class 'complex'> (4.5+2j)
```

```python
# str
str1 = 'Python'
print(type(str1), str1)
# Output: <class 'str'> Python
```

```python
# list (ordered, mutable, allows duplicates, heterogeneous)
l1 = [1, 2.3, 'data', [3,4,5], (4,5), 4+5j]
print(l1, type(l1))
# Output: [1, 2.3, 'data', [3, 4, 5], (4, 5), (4+5j)] <class 'list'>
```

```python
# tuple (ordered, immutable, allows duplicates, heterogeneous)
t1 = 1, 2.3, 'data', [3,4,5], (4,5), 4+5j
print(t1, type(t1))
# Output: (1, 2.3, 'data', [3, 4, 5], (4, 5), (4+5j)) <class 'tuple'>

t1 = (1, 2.3, 'data', [3,4,5], (4,5), 4+5j)
print(t1, type(t1))
# Output: (1, 2.3, 'data', [3, 4, 5], (4, 5), (4+5j)) <class 'tuple'>
```

```python
# set (unordered, mutable, NO duplicates)
s1 = {1, 2, 3.4, 4+5j, 'Data', 20}
print(s1, type(s1))
# Output: {1, 2, 3.4, (4+5j), 20, 'Data'} <class 'set'>
```

```python
# frozenset (immutable version of set)
fs1 = frozenset({1, 2, 3.4, 4+5j, 'Data', 20})
print(fs1, type(fs1))
# Output: frozenset({1, 2, 3.4, (4+5j), 20, 'Data'}) <class 'frozenset'>

# Can also create from a list
fs1 = frozenset([1, 2, 3.4, 4+5j, 'Data', 20])
print(fs1, type(fs1))
# Output: frozenset({1, 2, 3.4, (4+5j), 20, 'Data'}) <class 'frozenset'>
```

```python
# bool
b1 = True
print(type(b1), b1)
# Output: <class 'bool'> True

b2 = False
print(type(b2), b2)
# Output: <class 'bool'> False
```

```python
# dict (key-value pairs)
d1 = {'Virat': 18, 'Rohit': 45}
print(type(d1), d1)
# Output: <class 'dict'> {'Virat': 18, 'Rohit': 45}
```

```python
# range
print(list(range(5, 11)))       # [5, 6, 7, 8, 9, 10]
print(tuple(range(5, 11)))      # (5, 6, 7, 8, 9, 10)
```

### 7.4 The Danger of Shadowing Built-in Names

```python
# DANGER: Overwriting built-in names
int = 5
print(int)         # 5 — works, but...

int(46.79)         # TypeError: 'int' object is not callable
# You've overwritten the built-in int() function!

# FIX:
del int            # Delete the variable, restoring built-in
print(int(46.79))  # 46 — works again!
```

### 7.5 Mutable vs. Immutable Types

| Mutable (Changeable) | Immutable (Cannot Change) |
|----------------------|--------------------------|
| `list` | `int`, `float`, `complex` |
| `dict` | `str` |
| `set` | `tuple` |
| `bytearray` | `frozenset`, `bytes` |

> **⚠️ Key Insights & Common Mistakes**
> - **Never assign a value to a built-in type name**: `list = [1,2]`, `int = 5`, `str = 'hello'` — these shadow the built-in functions and break your code. Use `del list` to restore.
> - `type()` is your best friend — use it whenever you're unsure of a variable's type.
> - Empty curly braces `{}` create a **dict**, NOT a set! Use `set()` to create an empty set.
> - `True` is `1` and `False` is `0` in Python. `True + True` equals `2`. `True == 1` is `True`.
> - Tuples can be created without parentheses: `t = 1, 2, 3` creates a tuple `(1, 2, 3)`.
> - Sets only accept **immutable** (hashable) elements. You cannot put a list, set, or dict inside a set.

---

### 📝 Assignment Questions — Chapter 7

1. Create one variable for each of the following types: `int`, `float`, `complex`, `str`, `list`, `tuple`, `set`, `frozenset`, `dict`, `bool`. Print each with `type()`.
2. What is the difference between mutable and immutable types? Give three examples of each.
3. Why does `{} ` create a dict and not a set? How do you create an empty set?
4. What happens if you write `int = 5` and then try `int('100')`? How do you fix it?
5. Can you store a list inside a set? Why or why not?

---

## Chapter 8: Type Conversion and Type Checking

### 8.1 Theory

**Type conversion** (also called **type casting**) is the process of converting a value from one data type to another. Python supports two kinds:

1. **Implicit Type Conversion (Coercion):** Python automatically converts types during operations.
2. **Explicit Type Conversion (Casting):** The programmer explicitly converts using built-in functions.

### 8.2 Syntax

```python
int(value)       # Convert to integer
float(value)     # Convert to float
str(value)       # Convert to string
bool(value)      # Convert to boolean
list(value)      # Convert to list
tuple(value)     # Convert to tuple
set(value)       # Convert to set
```

### 8.3 Practice Examples

#### Implicit Conversion

```python
# Python automatically promotes int to float
x = 5       # int
y = 2.0     # float
result = x + y
print(result, type(result))    # 7.0 <class 'float'>

# bool is a subclass of int
print(True + 1)     # 2
print(False + 5)    # 5
```

#### Explicit Conversion

```python
# String to int
print(int('42'))        # 42
print(int('100'))       # 100
# print(int('abc'))     # ValueError: invalid literal for int() with base 10: 'abc'
# print(int('3.14'))    # ValueError! Can't convert '3.14' directly to int

# String to float
print(float('3.14'))    # 3.14
print(float('42'))      # 42.0

# Float to int (truncates, does NOT round)
print(int(46.79))       # 46 (not 47!)
print(int(-3.7))        # -3 (truncates toward zero)

# Number to string
print(str(42))          # '42'
print(str(3.14))        # '3.14'

# Sequence conversions
print(list('Python'))           # ['P', 'y', 't', 'h', 'o', 'n']
print(tuple([1, 2, 3]))        # (1, 2, 3)
print(set([1, 2, 2, 3, 3]))    # {1, 2, 3}
print(list(range(5)))           # [0, 1, 2, 3, 4]
```

#### What is "Truthy" and "Falsy"?

```python
# Falsy values (evaluate to False in boolean context)
print(bool(0))         # False
print(bool(0.0))       # False
print(bool(''))        # False (empty string)
print(bool([]))        # False (empty list)
print(bool({}))        # False (empty dict)
print(bool(()))        # False (empty tuple)
print(bool(set()))     # False (empty set)
print(bool(None))      # False

# Truthy values (everything else is True)
print(bool(1))         # True
print(bool(-1))        # True (non-zero)
print(bool('hello'))   # True (non-empty string)
print(bool([1]))       # True (non-empty list)
```

### 8.4 The `input()` Function

```python
# input() ALWAYS returns a string!
name = input('Enter your name: ')
print(type(name))    # <class 'str'>

age = input('Enter your age: ')
print(type(age))     # <class 'str'> — NOT int!

# Must convert explicitly
age = int(input('Enter your age: '))
print(type(age))     # <class 'int'>
```

> **⚠️ Key Insights & Common Mistakes**
> - `int()` **truncates** toward zero, it does NOT round: `int(3.9)` → `3`, `int(-3.9)` → `-3`.
> - `int('3.14')` raises `ValueError`! You must do `int(float('3.14'))` to convert "3.14" to 3.
> - `input()` **always returns a string**. You must explicitly convert: `int(input())` for integers.
> - `bool(0)`, `bool('')`, `bool([])`, `bool(None)` are all `False`. Non-zero, non-empty values are `True`.
> - `str(value)` never fails — you can convert anything to string.

---

### 📝 Assignment Questions — Chapter 8

1. What is the difference between implicit and explicit type conversion?
2. What is the output of `int(3.99)`? Why?
3. Why does `int('3.14')` raise an error? How do you correctly convert it to an integer?
4. List all the "falsy" values in Python.
5. Write a program that takes two numbers as input, adds them, and prints the result. (Remember: `input()` returns strings!)

---

# Part II: Operators and Expressions

---

## Chapter 9: Arithmetic Operators

### 9.1 Theory

**Arithmetic operators** perform mathematical operations on numeric values. Python supports all standard arithmetic operations plus some special ones like floor division (`//`) and exponentiation (`**`).

### 9.2 Syntax and Operators

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `+` | Addition | `5 + 3` | `8` |
| `-` | Subtraction | `5 - 3` | `2` |
| `*` | Multiplication | `5 * 3` | `15` |
| `/` | Division (float) | `7 / 2` | `3.5` |
| `//` | Floor Division (int) | `7 // 2` | `3` |
| `%` | Modulus (remainder) | `7 % 2` | `1` |
| `**` | Exponentiation | `2 ** 3` | `8` |

### 9.3 Extensive Practice Examples 

```python
print(5 + 3)      # 8
print(5 - 3)      # 2
print(5 * 3)      # 15
print(7 / 2)      # 3.5 (always returns float!)
print(7 // 2)     # 3 (floor division — rounds DOWN)
print(7 % 2)      # 1 (remainder)
print(2 ** 3)     # 8 (2 to the power of 3)
```

```python
# Division ALWAYS returns float
print(10 / 2)     # 5.0 (not 5!)
print(10 / 5)     # 2.0

# Floor division with negative numbers
print(7 // 2)     # 3
print(-7 // 2)    # -4 (rounds toward NEGATIVE infinity, not toward zero!)

# Modulus with negative numbers
print(7 % 2)      # 1
print(-7 % 2)     # 1 (in Python, result has same sign as divisor)
```

```python
# Operator precedence example
print(2 + 3 * 4)      # 14 (not 20! — multiplication first)
print((2 + 3) * 4)    # 20 (parentheses change order)
```

> **⚠️ Key Insights & Common Mistakes**
> - `/` (division) **always returns a float**: `10 / 2` gives `5.0`, not `5`.
> - `//` (floor division) rounds toward **negative infinity**, not toward zero: `-7 // 2` gives `-4`, not `-3`.
> - `%` (modulus) result has the **same sign as the divisor** in Python: `-7 % 2` gives `1`.
> - `**` has higher precedence than `-`: `-2**2` gives `-4` (not `4`), because it's `-(2**2)`.
> - Integer overflow does NOT exist in Python — integers can be arbitrarily large: `2**1000` works fine.

---

### 📝 Assignment Questions — Chapter 9

1. What is the difference between `/` and `//`?
2. What is the output of `-7 // 2`? Explain why.
3. What is the output of `2 + 3 * 4`? How do you change it to `20`?
4. Calculate `2 ** 10` and explain what `**` does.
5. What is modulus (`%`)? Give a practical use case (e.g., checking if a number is even).

---

## Chapter 10: Comparison (Relational) Operators

### 10.1 Theory

**Comparison operators** compare two values and return a **boolean** result (`True` or `False`). They are essential for conditional statements and loops.

### 10.2 Syntax and Operators

| Operator | Name | Example | Result |
|----------|------|---------|--------|
| `==` | Equals | `5 == 5` | `True` |
| `!=` | Not equals | `5 != 3` | `True` |
| `>` | Greater than | `5 > 3` | `True` |
| `<` | Less than | `3 < 5` | `True` |
| `>=` | Greater than or equal | `5 >= 5` | `True` |
| `<=` | Less than or equal | `3 <= 5` | `True` |

### 10.3 Extensive Practice Examples 

```python
print(5 == 5)        # True
print(5 == 5.0)      # True (int and float comparison works!)
print(5 == 5.1)      # False
# print(5 = = 5.0)   # SyntaxError: spaces in operator!

print('Rohit' == 'ROHIT')    # False (case-sensitive!)
print('Rohit' == 'Rohit')    # True
print('Rohit' != 'ROHIT')    # True

print(5 != 5)        # False
print(4 > 5)         # False
print(4 < 5)         # True

# String comparisons (lexicographic — uses Unicode values)
print('abc' > 'd')       # False (compares first character: 'a' < 'd')
print('abc' > 'aba')     # True (first difference at index 2: 'c' > 'a')

print(14 > 11)       # True
print(750 > 750)     # False
print(750 >= 750)    # True
print(750 <= 750)    # True
```

```python
a = 5
b = 4
print(a > b)     # True
print(a < b)     # False
print(a >= b)    # True
print(a == b)    # False
print(a != b)    # True
```

```python
# Chained comparisons (Python's special feature!)
x = 15
print(10 < x < 20)      # True (same as: 10 < x and x < 20)
print(1 < 2 < 3 < 4)    # True
print(1 < 2 > 3)        # False (2 > 3 is False)
```

> **⚠️ Key Insights & Common Mistakes**
> - `==` is comparison, `=` is assignment. Writing `if x = 5:` causes `SyntaxError`.
> - String comparisons are **case-sensitive**: `'Python' == 'python'` is `False`.
> - `5 == 5.0` is `True` because Python compares the values, not the types.
> - Python supports **chained comparisons**: `1 < x < 10` is valid and means `1 < x and x < 10`.
> - For floating-point comparisons, beware: `0.1 + 0.2 == 0.3` is `False` due to floating-point precision!

---

### 📝 Assignment Questions — Chapter 10

1. What is the difference between `=` and `==`?
2. Why is `'Python' == 'python'` `False`?
3. What is the output of `0.1 + 0.2 == 0.3`? Explain why.
4. Write a chained comparison to check if a number is between 1 and 100 (inclusive).
5. How does Python compare strings? What does `'abc' > 'abd'` return?

---

## Chapter 11: Logical Operators

### 11.1 Theory

**Logical operators** combine multiple boolean expressions. They are essential for complex conditions in `if` statements and loops.

### 11.2 Syntax

| Operator | Description | Example |
|----------|------------|---------|
| `and` | True if BOTH are True | `True and True` → `True` |
| `or` | True if AT LEAST ONE is True | `True or False` → `True` |
| `not` | Reverses the boolean | `not True` → `False` |

### 11.3 Truth Tables

**AND Truth Table:**

| A | B | A and B |
|---|---|---------|
| True | True | **True** |
| True | False | False |
| False | True | False |
| False | False | False |

**OR Truth Table:**

| A | B | A or B |
|---|---|--------|
| True | True | True |
| True | False | **True** |
| False | True | **True** |
| False | False | False |

### 11.4 Extensive Practice Examples 

```python
print(50 > 40 and 50 > 30)    # True and True → True
print(50 > 40 and 50 > 60)    # True and False → False
print(50 > 40 and 50 > 60 and 50 >= 50)    # True and False and True → False
print(50 > 40 and 50 < 60 and 50 >= 50)    # True and True and True → True

print(not 5 < 7)     # not True → False
print(not 5 > 7)     # not False → True
print(not False)      # True
print(not True)       # False
```

```python
# Short-circuit evaluation
# 'and' stops at first False
# 'or' stops at first True

x = 5
print(x > 0 and x < 10)    # True (both checked)
print(x > 10 and x < 20)   # False (stops at x > 10, doesn't check x < 20)

print(x > 0 or x > 100)    # True (stops at x > 0, doesn't check x > 100)
```

```python
# Practical example: checking multiple conditions
age = 25
has_license = True
has_insurance = True

can_drive = age >= 18 and has_license and has_insurance
print(can_drive)    # True
```

> **⚠️ Key Insights & Common Mistakes**
> - `and` returns `False` if **any** condition is False. `or` returns `True` if **any** condition is True.
> - **Short-circuit evaluation**: `and` stops evaluating at the first `False`. `or` stops at the first `True`. This means the second expression may never execute!
> - Use `and`/`or`/`not` in Python, NOT `&&`/`||`/`!` (those are from C/Java).
> - In Pandas/NumPy, use `&` and `|` instead of `and`/`or` for element-wise boolean operations.

---

### 📝 Assignment Questions — Chapter 11

1. Write the truth table for `and`, `or`, and `not`.
2. What is short-circuit evaluation? Give an example.
3. Write a condition that checks: age is between 18 and 65 AND has a valid ID.
4. What is the output of `not not True`?
5. Why can't you use `and`/`or` with Pandas DataFrames? What should you use instead?

---

## Chapter 12: Assignment Operators

### 12.1 Theory

**Assignment operators** are used to assign values to variables. The basic assignment operator is `=`. Python also provides **compound assignment operators** that perform an operation and assignment in one step.

### 12.2 Syntax 

| Operator | Example | Equivalent |
|----------|---------|-----------|
| `=` | `x = 5` | Assign 5 to x |
| `+=` | `x += 2` | `x = x + 2` |
| `-=` | `x -= 2` | `x = x - 2` |
| `*=` | `x *= 2` | `x = x * 2` |
| `/=` | `x /= 2` | `x = x / 2` |
| `//=` | `x //= 2` | `x = x // 2` |
| `%=` | `x %= 2` | `x = x % 2` |
| `**=` | `x **= 2` | `x = x ** 2` |

### 12.3 Practice Examples

```python
x = 10
print(x)        # 10

x += 5          # x = x + 5
print(x)        # 15

x -= 3          # x = x - 3
print(x)        # 12

x *= 2          # x = x * 2
print(x)        # 24

x /= 4          # x = x / 4
print(x)        # 6.0 (note: float!)

x //= 2         # x = x // 2
print(x)        # 3.0

x **= 3         # x = x ** 3
print(x)        # 27.0
```

> **⚠️ Key Insights & Common Mistakes**
> - `x /= 2` changes `x` to a **float** even if x was an integer. `10 /= 2` gives `5.0`, not `5`.
> - There is no `++` or `--` in Python! Use `x += 1` and `x -= 1` instead.
> - `=` is assignment, `==` is comparison. Confusing them is one of the most common beginner mistakes.

---

### 📝 Assignment Questions — Chapter 12

1. What is a compound assignment operator? List all of them.
2. What is the value of `x` after: `x = 10; x += 5; x *= 2; x -= 3`?
3. Why does Python not have `++` and `--` operators?
4. What type does `x` become after `x = 10; x /= 2`?
5. What is the difference between `=` and `==`?

---

## Chapter 13: Bitwise Operators

### 13.1 Theory

**Bitwise operators** operate on the **binary representation** of integers. They are important for low-level programming, cryptography, and certain algorithm optimisations. In Data Science, they are used with Pandas for element-wise boolean operations.

### 13.2 Syntax 

| Operator | Name | Rule |
|----------|------|------|
| `&` | Bitwise AND | 1 & 1 = 1, all others = 0 |
| `\|` | Bitwise OR | 0 \| 0 = 0, all others = 1 |
| `^` | Bitwise XOR | Same = 0, Different = 1 |
| `~` | Bitwise NOT | Inverts all bits |
| `<<` | Left Shift | Shifts bits left (multiplies by 2) |
| `>>` | Right Shift | Shifts bits right (divides by 2) |

**Bitwise AND Truth Table:**
```
1 & 1 → 1
1 & 0 → 0
0 & 1 → 0
0 & 0 → 0
```

**Bitwise OR Truth Table:**
```
1 | 1 → 1
1 | 0 → 1
0 | 1 → 1
0 | 0 → 0
```

### 13.3 Practice Examples

```python
a = 5    # binary: 0101
b = 3    # binary: 0011

print(a & b)     # 1  (0101 & 0011 = 0001)
print(a | b)     # 7  (0101 | 0011 = 0111)
print(a ^ b)     # 6  (0101 ^ 0011 = 0110)
print(~a)        # -6 (inverts all bits)
print(a << 1)    # 10 (0101 → 1010, shift left = multiply by 2)
print(a >> 1)    # 2  (0101 → 0010, shift right = divide by 2)
```

```python
# Converting to binary to verify
print(bin(5))        # 0b101
print(bin(3))        # 0b11
print(bin(5 & 3))    # 0b1  → 1
print(bin(5 | 3))    # 0b111 → 7
```

> **⚠️ Key Insights & Common Mistakes**
> - Don't confuse `&` (bitwise AND) with `and` (logical AND). `&` works on bits; `and` works on booleans.
> - In **Pandas**, use `&` and `|` (not `and`/`or`) for combining conditions: `df[(df['age'] > 20) & (df['city'] == 'Pune')]`.
> - `~` (bitwise NOT) of `n` equals `-(n+1)`: `~5` is `-6`, `~0` is `-1`.
> - Left shift `<<` multiplies by 2^n. Right shift `>>` divides by 2^n (integer division).

---

### 📝 Assignment Questions — Chapter 13

1. What is the binary representation of 10 and 7? What is `10 & 7`?
2. Explain the difference between `and` and `&`.
3. What is the result of `5 << 2`? Explain.
4. When would you use bitwise operators in Data Science?
5. What is the output of `~0`? Explain why.

---

## Chapter 14: Identity and Membership Operators

### 14.1 Theory

**Identity operators** check if two variables refer to the **same object** in memory (not just the same value).
**Membership operators** check if a value **exists within** a sequence (string, list, tuple, set, dict).

### 14.2 Syntax 

| Operator | Type | Description |
|----------|------|------------|
| `is` | Identity | True if same object in memory |
| `is not` | Identity | True if different objects |
| `in` | Membership | True if value found in sequence |
| `not in` | Membership | True if value NOT found in sequence |

### 14.3 Practice Examples

```python
# Identity operators
a = [1, 2, 3]
b = [1, 2, 3]
c = a

print(a == b)       # True (same values)
print(a is b)       # False (different objects in memory!)
print(a is c)       # True (c points to the same object as a)
print(a is not b)   # True

# is should be used for None checks
x = None
print(x is None)       # True (correct way)
print(x == None)       # True (works but not recommended)
```

```python
# Membership operators
fruits = ['apple', 'banana', 'mango']
print('apple' in fruits)       # True
print('grape' in fruits)       # False
print('grape' not in fruits)   # True

# Works with strings too
print('Py' in 'Python')       # True
print('py' in 'Python')       # False (case-sensitive!)

# Works with dicts (checks KEYS, not values)
d = {'name': 'Alice', 'age': 25}
print('name' in d)       # True (checks keys)
print('Alice' in d)      # False (doesn't check values!)
print('Alice' in d.values())    # True (check values explicitly)
```

> **⚠️ Key Insights & Common Mistakes**
> - `==` checks **value equality**. `is` checks **identity** (same object in memory). Always use `is` for `None` checks: `if x is None`.
> - `in` with dictionaries checks **keys**, not values! `'Alice' in {'name': 'Alice'}` is `False` because `'Alice'` is a value, not a key.
> - `in` is case-sensitive for strings: `'py' in 'Python'` is `False`.
> - Never use `is` to compare numbers or strings (except with `None`): `x is 5` may give unexpected results due to Python's caching.

---

### 📝 Assignment Questions — Chapter 14

1. What is the difference between `is` and `==`? When should you use each?
2. Why does `[1,2] is [1,2]` return `False`?
3. How do you check if a value exists in a dictionary's values (not keys)?
4. Write code to check if the letter 'a' exists in the string 'Data Science'.
5. Why should you use `x is None` instead of `x == None`?

---

## Chapter 15: Operator Precedence and Associativity

### 15.1 Theory

When an expression has multiple operators, Python uses **operator precedence** (priority) and **associativity** (direction) to determine the order of evaluation.

### 15.2 Precedence Table (Highest to Lowest)

| Priority | Operator | Description |
|----------|----------|------------|
| 1 (Highest) | `()` | Parentheses |
| 2 | `**` | Exponentiation |
| 3 | `+x`, `-x`, `~x` | Unary plus, minus, NOT |
| 4 | `*`, `/`, `//`, `%` | Multiplication, division |
| 5 | `+`, `-` | Addition, subtraction |
| 6 | `<<`, `>>` | Bitwise shifts |
| 7 | `&` | Bitwise AND |
| 8 | `^` | Bitwise XOR |
| 9 | `\|` | Bitwise OR |
| 10 | `==`, `!=`, `<`, `>`, `>=`, `<=`, `is`, `in` | Comparisons |
| 11 | `not` | Logical NOT |
| 12 | `and` | Logical AND |
| 13 (Lowest) | `or` | Logical OR |

### 15.3 Practice Examples

```python
# Precedence matters!
print(2 + 3 * 4)        # 14 (not 20!) — * before +
print((2 + 3) * 4)      # 20 — parentheses override

print(2 ** 3 ** 2)       # 512 (not 64!) — ** is right-associative: 2 ** (3**2) = 2**9
print((2 ** 3) ** 2)     # 64

print(-2 ** 2)           # -4 (not 4!) — ** before unary minus: -(2**2)
print((-2) ** 2)         # 4

print(True or True and False)    # True — 'and' before 'or': True or (True and False) = True or False = True
```

> **⚠️ Key Insights & Common Mistakes**
> - When in doubt, **use parentheses**! They make code more readable and prevent precedence bugs.
> - `**` is **right-associative**: `2 ** 3 ** 2` = `2 ** (3**2)` = `2 ** 9` = `512`.
> - `and` has higher precedence than `or`: `True or True and False` = `True or (True and False)` = `True`.
> - `-2**2` is `-4` (not `4`!) because `**` has higher precedence than unary minus.

---

### 📝 Assignment Questions — Chapter 15

1. What is the output of `2 + 3 * 4 - 1`? Explain step by step.
2. What is the output of `2 ** 3 ** 2`? Why?
3. Why is `-2 ** 2` equal to `-4` and not `4`?
4. What is the output of `True or False and False`? Explain the precedence.
5. Why should you always use parentheses in complex expressions?

---

# Part III: Strings — Text Processing Mastery

---

## Chapter 16: String Creation, Properties, and Escape Sequences

### 16.1 Theory

A **string** (`str`) is a sequence of characters enclosed in quotes. Strings are one of the most commonly used data types in Python and are essential for text processing, data cleaning, and natural language processing.

**Key Properties:**
- **Immutable**: Once created, a string cannot be changed (individual characters cannot be modified)
- **Ordered**: Characters have a defined position (index)
- **Iterable**: You can loop through characters one by one
- **Duplicates allowed**: Same characters can appear multiple times

### 16.2 Syntax — Four Ways to Create Strings

```python
str1 = 'Single quotes'        # Most common
str2 = "Double quotes"        # Same as single quotes
str3 = '''Triple single quotes
for multi-line strings'''
str4 = """Triple double quotes
for multi-line strings"""
```

### 16.3 Practice Examples

```python
# Different quote types
s1 = 'Hello Python'
s2 = "Hello Python"
s3 = '''Hello Python'''
s4 = """Hello Python"""

print(s1)    # Hello Python
print(type(s1))    # <class 'str'>
```

```python
# When to use which quotes
s1 = "It's Python"              # Double quotes to include single quote
s2 = 'He said "Hello"'          # Single quotes to include double quotes
s3 = '''It's a "beautiful" day'''  # Triple quotes for both
s4 = "It\'s Python"             # Or use escape character
```

```python
# Multi-line strings
address = """
123 Python Street
Data Science City
AI Country - 400001
"""
print(address)
```

```python
# String length
s = 'Python'
print(len(s))    # 6
```

```python
# String is immutable
s = 'Python'
# s[0] = 'J'    # TypeError: 'str' object does not support item assignment
# You must create a new string instead:
s = 'J' + s[1:]
print(s)    # Jython
```

> **⚠️ Key Insights & Common Mistakes**
> - Strings are **immutable** — you cannot change individual characters. `s[0] = 'X'` raises `TypeError`.
> - Single quotes `'...'` and double quotes `"..."` are identical in Python (unlike some other languages).
> - Triple-quoted strings preserve line breaks and are often used for **docstrings**.
> - An empty string `''` is **falsy**: `bool('')` is `False`. A non-empty string is **truthy**.

---

### 📝 Assignment Questions — Chapter 16

1. What are the four ways to create a string in Python?
2. Why are strings called "immutable"? What error occurs if you try to change a character?
3. How do you include both single and double quotes in a string?
4. What is the output of `len('Hello\nWorld')`? (Hint: `\n` is ONE character)
5. What is a docstring and how is it created?

---

## Chapter 17: String Indexing and Slicing

### 17.1 Theory

**Indexing** allows you to access individual characters in a string using their position number. **Slicing** allows you to extract a substring (a portion of the string).

Python uses **zero-based indexing** (the first character is at index 0). Python also supports **negative indexing** (the last character is at index -1).

### 17.2 Syntax

```python
string[index]                   # Single character
string[start:stop]              # Slice from start to stop-1
string[start:stop:step]         # Slice with step
string[:stop]                   # From beginning to stop-1
string[start:]                  # From start to end
string[:]                       # Copy of entire string
string[::-1]                    # Reverse the string
```

### 17.3 Index Diagram

```
String:     P   y   t   h   o   n
Pos Index:  0   1   2   3   4   5
Neg Index: -6  -5  -4  -3  -2  -1
```

### 17.4 Extensive Practice Examples 

```python
s = 'Python'

# Positive indexing
print(s[0])      # P
print(s[1])      # y
print(s[5])      # n
# print(s[6])    # IndexError: string index out of range

# Negative indexing
print(s[-1])     # n (last character)
print(s[-6])     # P (first character)
```

```python
s = 'Python Programming'

# Slicing [start:stop] — includes start, excludes stop
print(s[0:6])        # Python
print(s[7:18])       # Programming
print(s[:6])         # Python (from beginning)
print(s[7:])         # Programming (to end)
print(s[:])          # Python Programming (entire string)

# Slicing with step [start:stop:step]
print(s[::2])        # Pto rgamn (every 2nd character)
print(s[::3])        # Ph oai (every 3rd character)

# Reverse a string
print(s[::-1])       # gnimmargorP nohtyP
```

```python
# Slicing never raises IndexError (unlike indexing)
s = 'Python'
print(s[0:100])      # Python (doesn't raise error!)
print(s[100:200])    # '' (empty string, no error)
```

> **⚠️ Key Insights & Common Mistakes**
> - **Indexing** with an out-of-range index raises `IndexError`. But **slicing** with out-of-range values does NOT — it just returns what's available.
> - `string[start:stop]` includes `start` but **excludes** `stop`. `s[0:3]` gives characters at index 0, 1, 2 (not 3).
> - `s[::-1]` reverses the string — a very common Python pattern used in interviews.
> - Negative indices count from the end: `-1` is the last character, `-2` is second-to-last, etc.

---

### 📝 Assignment Questions — Chapter 17

1. What is the difference between `s[3]` and `s[3:4]`?
2. How do you reverse a string using slicing?
3. What is the output of `'Python'[1:4]`?
4. Why does `'Python'[100]` raise an error but `'Python'[0:100]` does not?
5. Write code to extract every other character from a string.

---

## Chapter 18: String Methods — A Complete Reference

### 18.1 Theory

Python provides a rich set of **built-in string methods** for text manipulation. These methods return a **new string** (because strings are immutable) — the original string is never modified.

### 18.2 Commonly Used String Methods

| Method | Description | Example | Result |
|--------|------------|---------|--------|
| `upper()` | Converts to uppercase | `'hello'.upper()` | `'HELLO'` |
| `lower()` | Converts to lowercase | `'HELLO'.lower()` | `'hello'` |
| `title()` | First letter of each word capitalised | `'hello world'.title()` | `'Hello World'` |
| `capitalize()` | First letter capitalised | `'hello'.capitalize()` | `'Hello'` |
| `strip()` | Removes leading/trailing whitespace | `' hello '.strip()` | `'hello'` |
| `lstrip()` | Removes leading whitespace | `' hello '.lstrip()` | `'hello '` |
| `rstrip()` | Removes trailing whitespace | `' hello '.rstrip()` | `' hello'` |
| `split()` | Splits string into list | `'a,b,c'.split(',')` | `['a','b','c']` |
| `join()` | Joins list into string | `','.join(['a','b'])` | `'a,b'` |
| `replace()` | Replaces substring | `'hello'.replace('l','r')` | `'herro'` |
| `find()` | Finds first occurrence (returns -1 if not found) | `'hello'.find('l')` | `2` |
| `index()` | Finds first occurrence (raises ValueError if not found) | `'hello'.index('l')` | `2` |
| `count()` | Counts occurrences | `'hello'.count('l')` | `2` |
| `startswith()` | Checks prefix | `'hello'.startswith('he')` | `True` |
| `endswith()` | Checks suffix | `'hello'.endswith('lo')` | `True` |
| `isdigit()` | All characters are digits? | `'123'.isdigit()` | `True` |
| `isalpha()` | All characters are letters? | `'abc'.isalpha()` | `True` |
| `isalnum()` | All characters are letters or digits? | `'abc123'.isalnum()` | `True` |
| `isnumeric()` | Numeric characters? | `'123'.isnumeric()` | `True` |
| `istitle()` | Title case? | `'Hello World'.istitle()` | `True` |
| `swapcase()` | Swaps upper/lower case | `'Hello'.swapcase()` | `'hELLO'` |
| `center()` | Centers string with padding | `'hi'.center(10, '*')` | `'****hi****'` |
| `zfill()` | Pads with zeros on left | `'42'.zfill(5)` | `'00042'` |

### 18.3 Practice Examples

```python
s = '   Hello, World!   '

print(s.strip())       # 'Hello, World!'
print(s.lstrip())      # 'Hello, World!   '
print(s.rstrip())      # '   Hello, World!'

s = 'Python Programming'
print(s.upper())       # 'PYTHON PROGRAMMING'
print(s.lower())       # 'python programming'
print(s.title())       # 'Python Programming'
print(s.swapcase())    # 'pYTHON pROGRAMMING'
```

```python
# split and join
csv_line = 'Alice,25,Pune,Data Scientist'
parts = csv_line.split(',')
print(parts)    # ['Alice', '25', 'Pune', 'Data Scientist']

words = ['Python', 'is', 'awesome']
sentence = ' '.join(words)
print(sentence)    # 'Python is awesome'
```

```python
# find vs index
s = 'Hello World'
print(s.find('World'))     # 6
print(s.find('Python'))    # -1 (not found, returns -1)
# print(s.index('Python'))  # ValueError! (raises error if not found)
```

```python
# replace
s = 'I love Java'
print(s.replace('Java', 'Python'))    # I love Python
print(s.replace('a', 'X'))            # I love JXvX
print(s.replace('a', 'X', 1))         # I love JXva (replace only first)
```

```python
# Checking string content
print('12345'.isdigit())       # True
print('12.34'.isdigit())       # False (dot is not a digit!)
print('hello'.isalpha())       # True
print('hello123'.isalnum())    # True
print('Python'.istitle())      # True
print('python'.istitle())      # False
print('1234567'.isnumeric())   # True
print('123.4567'.isnumeric())  # False
```

> **⚠️ Key Insights & Common Mistakes**
> - String methods return a **new string** — they do NOT modify the original! `s.upper()` returns the uppercase version but `s` stays the same. You must assign: `s = s.upper()`.
> - `find()` returns `-1` if not found. `index()` raises `ValueError`. Use `find()` when you're unsure if the substring exists.
> - `split()` without arguments splits by **any whitespace** (spaces, tabs, newlines) and removes empty strings.
> - `'123.45'.isdigit()` is `False` because `.` is not a digit. Use `try: float(s)` for decimal validation.
> - `strip()` only removes **leading and trailing** whitespace, not whitespace in the middle.

---

### 📝 Assignment Questions — Chapter 18

1. What is the difference between `find()` and `index()`?
2. Why does `s.upper()` not change the original string `s`?
3. Write code to count the number of vowels in a string.
4. Split the CSV string `'Alice,25,Pune'` and access the second element.
5. Write code to check if a string is a valid integer (handles negatives too).

---

## Chapter 19: String Formatting — `%`, `.format()`, and f-strings

### 19.1 Theory

**String formatting** allows you to embed variables and expressions inside strings. Python provides three methods, from oldest to newest.

### 19.2 Three Methods

#### Method 1: `%` Formatting (Oldest — C-style)

```python
name = 'Alice'
age = 25
print('Name: %s, Age: %d' % (name, age))
# Output: Name: Alice, Age: 25

# %s = string, %d = integer, %f = float
print('Pi = %.2f' % 3.14159)
# Output: Pi = 3.14
```

#### Method 2: `.format()` Method

```python
print('Name: {}, Age: {}'.format('Alice', 25))
# Output: Name: Alice, Age: 25

print('Name: {0}, Age: {1}, Name again: {0}'.format('Alice', 25))
# Output: Name: Alice, Age: 25, Name again: Alice

print('Name: {name}, Age: {age}'.format(name='Alice', age=25))
# Output: Name: Alice, Age: 25
```

#### Method 3: f-strings (Python 3.6+ — Recommended!)

```python
name = 'Alice'
age = 25
salary = 50000.567

print(f'Name: {name}, Age: {age}')
# Output: Name: Alice, Age: 25

# Expressions inside {}
print(f'Next year: {age + 1}')
# Output: Next year: 26

# Formatting numbers
print(f'Salary: {salary:.2f}')    # 2 decimal places
# Output: Salary: 50000.57

print(f'Salary: {salary:,.2f}')   # Comma separator
# Output: Salary: 50,000.57

print(f'Binary: {42:b}')          # Binary
# Output: Binary: 101010

print(f'Hex: {255:x}')            # Hexadecimal
# Output: Hex: ff

# Alignment
print(f'{"left":<20}|')      # Left-align
print(f'{"center":^20}|')    # Center-align
print(f'{"right":>20}|')     # Right-align

# Debugging (Python 3.8+)
x = 42
print(f'{x = }')
# Output: x = 42
```

> **⚠️ Key Insights & Common Mistakes**
> - **Always use f-strings** for new code — they are the most readable, concise, and fastest.
> - The most common mistake: **forgetting the `f` prefix**: `'{name}'` prints the literal text `{name}`, not the variable value!
> - You can put any valid Python expression inside `{}` in f-strings: `f'{2**10}'` → `'1024'`.
> - For Python versions before 3.6, use `.format()`.

---

### 📝 Assignment Questions — Chapter 19

1. What are the three string formatting methods in Python? Which is recommended?
2. Format the number `1234567.89` with comma separators and 2 decimal places.
3. What happens if you forget the `f` prefix in an f-string?
4. Use f-string to display a number in binary and hexadecimal format.
5. Write an f-string that right-aligns a name in a 30-character wide field.

---

# Part IV: Control Flow

---

## Chapter 20: Conditional Statements (`if`, `elif`, `else`)

### 20.1 Theory

**Conditional statements** (also called **decision-making statements**) allow your program to execute different blocks of code based on conditions. They are fundamental to all programming — without them, programs would execute the same instructions every time.

Python supports: `if`, `elif` (else if), and `else`.

### 20.2 Syntax 

```python
# if only
if condition:
    statement(s)    # Executes if condition is True

# if-else
if condition:
    statement(s)    # Executes if condition is True
else:
    statement(s)    # Executes if condition is False

# if-elif-else
if condition1:
    statement(s)    # Executes if condition1 is True
elif condition2:
    statement(s)    # Executes if condition2 is True
elif condition3:
    statement(s)    # Executes if condition3 is True
else:
    statement(s)    # Executes if all conditions are False
```

**Valid combinations :**
```
if
if elif
if else
if elif else
if elif elif else
if elif elif ... else
```

**Invalid (cannot standalone):**
```
elif    # SyntaxError
else    # SyntaxError
```

### 20.3 Extensive Practice Examples 

```python
# Simple if
a = 15
b = 20

if b > a:    # True
    print('a is smaller than b')
# Output: a is smaller than b
```

```python
# if — condition is False (nothing happens)
a = 25
b = 20

if b > a:    # False
    print('a is smaller than b')
# Output: (nothing printed!)
```

```python
# if-else
a = 25
b = 20

if b > a:    # False
    print('a is smaller than b')
else:
    print('b is not greater than a')
# Output: b is not greater than a
```

```python
# if-else — True case
a = 25
b = 28

if b > a:    # True
    print('a is smaller than b')
else:
    print('b is not greater than a')
# Output: a is smaller than b
```

```python
# Using string methods in conditions
str1 = 'Python'

if str1.istitle():    # True
    print('The String is in Title case')
else:
    print('The String is not in Title case')
# Output: The String is in Title case
```

```python
str1 = 'python'

if str1.istitle():    # False
    print('The String is in Title case')
else:
    print('The String is not in Title case')
# Output: The String is not in Title case
```

```python
# Checking numeric content
str1 = '1234567'

if str1.isnumeric():    # True
    print('The String contains all digits')
else:
    print('The String does not contain all digits')
# Output: The String contains all digits
```

```python
str1 = '123.4567'

if str1.isnumeric():    # False (dot is not numeric)
    print('The String contains all digits')
else:
    print('The String does not contain all digits')
# Output: The String does not contain all digits
```

```python
# if-elif-else
a = 150
b = 45

if a > b:    # True
    print('a is greater than b')
elif a == b:
    print('a is equal to b')
else:
    print('a is not greater than or equal to b')
# Output: a is greater than b
```

```python
a = 150
b = 150

if a > b:    # False
    print('a is greater than b')
elif a == b:    # True
    print('a is equal to b')
else:
    print('a is not greater than or equal to b')
# Output: a is equal to b
```

```python
a = 150
b = 151

if a > b:    # False
    print('a is greater than b')
elif a == b:    # False
    print('a is equal to b')
else:
    print('a is not greater than or equal to b')
# Output: a is not greater than or equal to b
```

```python
# Using >= in conditions
a = 150
b = 150

if a >= b:    # True — but may conflict with other conditions
    print('a is greater than or equals to b')
elif a == b:
    print('a is equal to b')
else:
    print('a is less than b')
# Output: a is greater than or equals to b
# Note: elif a == b never executes because a >= b is already True when a == b!
```

### 20.4 Practical Examples

```python
# Grade calculator
marks = 85

if marks >= 90:
    grade = 'A+'
elif marks >= 80:
    grade = 'A'
elif marks >= 70:
    grade = 'B'
elif marks >= 60:
    grade = 'C'
else:
    grade = 'F'

print(f'Grade: {grade}')    # Grade: A
```

```python
# Even/Odd checker
num = 7

if num % 2 == 0:
    print(f'{num} is Even')
else:
    print(f'{num} is Odd')
# Output: 7 is Odd
```

> **⚠️ Key Insights & Common Mistakes**
> - **Indentation is mandatory** — the code block under `if`/`elif`/`else` must be indented (4 spaces).
> - `elif` and `else` **cannot exist without** a preceding `if`. They cause `SyntaxError` on their own.
> - Don't forget the **colon** `:` after the condition! `if x > 5` without `:` causes `SyntaxError`.
> - `if a >= b:` will be `True` when `a == b`, so be careful with overlapping conditions.
> - Only **one block** executes in an if-elif-else chain — Python checks conditions top to bottom and executes the **first** True block, then skips all remaining.
> - `=` is assignment, `==` is comparison. `if x = 5:` causes `SyntaxError`.

---

### 📝 Assignment Questions — Chapter 20

1. What is the difference between `if-else` and `if-elif-else`?
2. What error occurs if you use `elif` without an `if`?
3. Write a program to check if a year is a leap year.
4. Write a grade calculator with input from user.
5. Can an `if-elif` chain work without `else`? What happens if no condition is True?

---

## Chapter 21: Nested Conditionals and Ternary Expressions

### 21.1 Theory — Nested Conditionals

A **nested conditional** is an `if` statement inside another `if` statement. This allows for more complex decision-making with multiple levels of conditions.

### 21.2 Syntax

```python
if outer_condition:
    if inner_condition:
        statement(s)
    else:
        statement(s)
else:
    statement(s)
```

### 21.3 Practice Examples

```python
# Nested if
age = 25
has_id = True

if age >= 18:
    if has_id:
        print('Entry allowed')
    else:
        print('Please bring your ID')
else:
    print('Entry not allowed — under 18')
# Output: Entry allowed
```

```python
# Number classification
num = -5

if num > 0:
    print('Positive')
elif num < 0:
    if num > -10:
        print('Negative (single digit)')
    else:
        print('Negative (large)')
else:
    print('Zero')
# Output: Negative (single digit)
```

### 21.4 Theory — Ternary (Shorthand) Conditional

Python allows a **one-line conditional expression** called the **ternary operator**.

### 21.5 Syntax

```python
result = value_if_true if condition else value_if_false
```

### 21.6 Practice Examples 

```python
# Traditional if-else
age = 20
if age >= 18:
    status = 'Adult'
else:
    status = 'Minor'
print(status)    # Adult

# Same thing in one line (ternary)
status = 'Adult' if age >= 18 else 'Minor'
print(status)    # Adult
```

```python
# Ternary for max of two numbers
a, b = 10, 20
max_val = a if a > b else b
print(max_val)    # 20
```

```python
# Ternary for even/odd
num = 7
result = 'Even' if num % 2 == 0 else 'Odd'
print(result)    # Odd
```

```python
# Nested ternary (avoid — hard to read!)
x = 0
result = 'Positive' if x > 0 else ('Negative' if x < 0 else 'Zero')
print(result)    # Zero
```

> **⚠️ Key Insights & Common Mistakes**
> - Avoid deeply nested conditionals (more than 2 levels) — they make code hard to read. Use functions or logical operators instead.
> - Ternary expressions are great for simple conditions but should **not** be nested deeply.
> - The ternary operator is an **expression** (returns a value), not a statement. You can use it inside `print()`, assignments, list comprehensions, etc.

---

### 📝 Assignment Questions — Chapter 21

1. Write a nested conditional to classify a number as positive even, positive odd, negative even, negative odd, or zero.
2. Convert `if-else` to a ternary expression: "Pass" if marks >= 40, else "Fail".
3. Why should you avoid deeply nested conditionals? What alternatives exist?
4. Write a ternary expression that returns the absolute value of a number.
5. Can you use ternary expressions inside a `print()` statement? Give an example.

---

## Chapter 22: The `for` Loop

### 22.1 Theory

A **`for` loop** is used to iterate (loop) over a sequence (string, list, tuple, set, dict, range). It executes a block of code **once for each item** in the sequence.

The `for` loop in Python is more like a "for-each" loop — it iterates directly over elements, not over indices (though you can use `range()` for index-based iteration).

### 22.2 Syntax

```python
for variable in iterable:
    statement(s)
```

### 22.3 Extensive Practice Examples 

```python
# Iterating over a string
for char in 'Python':
    print(char)
# Output:
# P
# y
# t
# h
# o
# n
```

```python
# Iterating over a list
fruits = ['apple', 'banana', 'mango']
for fruit in fruits:
    print(fruit)
# Output:
# apple
# banana
# mango
```

```python
# Using range()
for i in range(5):
    print(i, end=' ')
# Output: 0 1 2 3 4

for i in range(1, 6):
    print(i, end=' ')
# Output: 1 2 3 4 5

for i in range(0, 10, 2):     # step of 2
    print(i, end=' ')
# Output: 0 2 4 6 8

for i in range(10, 0, -1):    # counting down
    print(i, end=' ')
# Output: 10 9 8 7 6 5 4 3 2 1

for i in range(10, 0, -2):    # counting down by 2
    print(i, end=' ')
# Output: 10 8 6 4 2
```

```python
# enumerate() — get index AND value
fruits = ['apple', 'banana', 'mango']
for index, fruit in enumerate(fruits):
    print(f'{index}: {fruit}')
# Output:
# 0: apple
# 1: banana
# 2: mango

# Starting enumerate from 1
for index, fruit in enumerate(fruits, start=1):
    print(f'{index}: {fruit}')
# Output:
# 1: apple
# 2: banana
# 3: mango
```

```python
# Unpacking in for loop
students = [('Alice', 85), ('Bob', 92), ('Charlie', 78)]
for name, score in students:
    print(f'{name}: {score}')
# Output:
# Alice: 85
# Bob: 92
# Charlie: 78
```

```python
# Iterating over a dictionary
d = {'Virat': 18, 'Rohit': 45, 'Dhoni': 7}

# Keys (default)
for key in d:
    print(key)
# Output: Virat, Rohit, Dhoni

# Values
for value in d.values():
    print(value)
# Output: 18, 45, 7

# Key-value pairs
for key, value in d.items():
    print(f'{key} : {value}')
# Output:
# Virat : 18
# Rohit : 45
# Dhoni : 7
```

```python
# for-else (else executes if loop completes without break)
for i in range(5):
    print(i, end=' ')
else:
    print('\nLoop completed!')
# Output:
# 0 1 2 3 4
# Loop completed!
```

> **⚠️ Key Insights & Common Mistakes**
> - `range(5)` generates `0, 1, 2, 3, 4` — it does NOT include 5! The stop value is **exclusive**.
> - `range(start, stop, step)` — `start` is inclusive, `stop` is exclusive.
> - Don't modify a list while iterating over it — use a copy or list comprehension instead.
> - `enumerate()` is the Pythonic way to get both index and value. Don't use `range(len(list))`.
> - `for-else`: The `else` block runs **only if the loop completes normally** (not interrupted by `break`).

---

### 📝 Assignment Questions — Chapter 22

1. What is the output of `list(range(1, 10, 3))`?
2. Write a for loop to print the multiplication table of 7.
3. Use `enumerate()` to print elements of a list with their index.
4. How do you iterate over a dictionary's key-value pairs?
5. What is `for-else`? When does the `else` block execute?

---

## Chapter 23: The `while` Loop

### 23.1 Theory

A **`while` loop** repeatedly executes a block of code **as long as a condition is True**. Unlike `for` loops (which iterate over sequences), `while` loops are used when you don't know in advance how many times to loop.

### 23.2 Syntax

```python
while condition:
    statement(s)
    # Update condition (important! Prevents infinite loop)
```

### 23.3 Practice Examples

```python
# Basic while loop
count = 1
while count <= 5:
    print(count, end=' ')
    count += 1
# Output: 1 2 3 4 5
```

```python
# Sum of numbers until user enters 0
total = 0
num = int(input('Enter number (0 to stop): '))
while num != 0:
    total += num
    num = int(input('Enter number (0 to stop): '))
print(f'Total: {total}')
```

```python
# while-else
count = 1
while count <= 3:
    print(count)
    count += 1
else:
    print('Loop completed normally')
# Output:
# 1
# 2
# 3
# Loop completed normally
```

```python
# Infinite loop (be careful!)
# while True:
#     print('This runs forever!')
# Use Ctrl+C to stop, or use break:

while True:
    response = input('Type "quit" to exit: ')
    if response == 'quit':
        break
print('Goodbye!')
```

> **⚠️ Key Insights & Common Mistakes**
> - **Always update the loop variable** inside the while loop! Forgetting this creates an **infinite loop**.
> - `while True:` creates an intentional infinite loop — use `break` to exit.
> - `while-else`: The `else` runs only if the loop exits normally (not via `break`).
> - Prefer `for` loops when you know the number of iterations. Use `while` when iteration count is unknown.

---

### 📝 Assignment Questions — Chapter 23

1. What is the difference between a `for` loop and a `while` loop?
2. What causes an infinite loop? How do you prevent it?
3. Write a while loop that asks for a password until the correct one is entered.
4. What is `while-else`? When does the `else` execute?
5. Write a while loop to find the sum of digits of a number (e.g., 1234 → 10).

---

## Chapter 24: Loop Control — `break`, `continue`, `pass`

### 24.1 Theory

| Statement | Description |
|-----------|------------|
| `break` | Exits the loop immediately |
| `continue` | Skips the rest of the current iteration, goes to next iteration |
| `pass` | Does nothing (placeholder) |

### 24.2 Practice Examples

```python
# break — exit loop early
for i in range(10):
    if i == 5:
        break
    print(i, end=' ')
# Output: 0 1 2 3 4
```

```python
# continue — skip certain iterations
for i in range(10):
    if i % 2 == 0:
        continue    # Skip even numbers
    print(i, end=' ')
# Output: 1 3 5 7 9
```

```python
# pass — placeholder (does nothing)
for i in range(5):
    if i == 3:
        pass    # TODO: handle this case later
    print(i, end=' ')
# Output: 0 1 2 3 4
```

```python
# break with for-else
for i in range(5):
    if i == 3:
        break
else:
    print('Loop completed')
# Output: (nothing from else — break was triggered!)
```

> **⚠️ Key Insights & Common Mistakes**
> - `break` exits the **innermost** loop only. In nested loops, it only breaks out of the inner loop.
> - `continue` doesn't exit the loop — it skips to the next iteration.
> - `pass` is a no-op — used as a placeholder when Python syntax requires a statement but you have nothing to write yet.
> - In `for-else`/`while-else`: `else` runs only if the loop was NOT terminated by `break`.

---

### 📝 Assignment Questions — Chapter 24

1. What is the difference between `break` and `continue`?
2. What is `pass` used for? Give a practical example.
3. What happens to the `else` block in `for-else` when `break` is triggered?
4. Write a loop that prints numbers 1–100 but stops at the first multiple of 37.
5. Write a loop that prints all numbers 1–20 except multiples of 3.

---

## Chapter 25: Nested Loops and Pattern Programming

### 25.1 Theory

A **nested loop** is a loop inside another loop. The inner loop completes all its iterations for each iteration of the outer loop.

### 25.2 Practice Examples

```python
# Nested for loop — multiplication table
for i in range(1, 6):
    for j in range(1, 6):
        print(f'{i*j:4}', end='')
    print()
# Output:
#    1   2   3   4   5
#    2   4   6   8  10
#    3   6   9  12  15
#    4   8  12  16  20
#    5  10  15  20  25
```

```python
# Pattern: Right triangle
for i in range(1, 6):
    print('* ' * i)
# Output:
# *
# * *
# * * *
# * * * *
# * * * * *
```

```python
# Pattern: Number triangle
for i in range(1, 6):
    for j in range(1, i + 1):
        print(j, end=' ')
    print()
# Output:
# 1
# 1 2
# 1 2 3
# 1 2 3 4
# 1 2 3 4 5
```

> **⚠️ Key Insights & Common Mistakes**
> - Nested loops multiply iterations: outer loop runs `n` times × inner loop runs `m` times = `n × m` total iterations.
> - `break` in a nested loop only breaks the **inner loop**. Use a flag variable or function return to break out of both.
> - Avoid deep nesting (3+ levels) — refactor into functions for readability.

---

### 📝 Assignment Questions — Chapter 25

1. How many times does `print()` execute in: `for i in range(5): for j in range(3): print()`?
2. Write a nested loop to print a 5×5 identity matrix.
3. Print an inverted right triangle of stars (5 rows).
4. Write code to find all pairs (i, j) where i + j = 10, for i and j from 1 to 9.
5. How do you break out of both inner and outer loops?

---

# Part V: Core Data Structures

---

## Chapter 26: Lists — Creation, Indexing, Slicing, and Methods

### 26.1 Theory

A **list** is the most versatile and commonly used data structure in Python. It is an **ordered, mutable** collection that can hold items of **any data type** (heterogeneous).

**Key Properties :**
1. **Mutable** — can add, delete, modify, update (changeable)
2. **Ordered** — items maintain insertion order
3. **Duplicates are allowed**
4. Lists are enclosed by **square brackets** `[]`
5. List items are **comma separated**

**Types of Brackets in Python :**

| Bracket | Name | Used For |
|---------|------|----------|
| `()` | Parentheses (round brackets) | Tuples, function calls |
| `[]` | Square brackets | Lists, indexing, slicing |
| `{}` | Curly brackets (braces) | Dicts, sets, f-string placeholders |

### 26.2 Syntax

```python
# Creating lists
empty_list = []          # Empty list
empty_list = list()      # Empty list (using constructor)
numbers = [1, 2, 3, 4]  # List of integers
mixed = [1, 'hello', 3.14, True]  # Mixed types
```

### 26.3 Extensive Practice Examples 

```python
# Lists can hold any data type (heterogeneous)
l1 = [12, 23.4, 3+4j, 'data', [1,2,3], (2,3,4), {4,5,6}, frozenset((6,5,4)), {'Virat':18, 'Rohit':45}]
print(l1)
# Output: [12, 23.4, (3+4j), 'data', [1, 2, 3], (2, 3, 4), {4, 5, 6}, frozenset({4, 5, 6}), {'Virat': 18, 'Rohit': 45}]
```

```python
# Lists allow duplicates
l1 = [3, 4, 5, 5, 6, 2, 'python', 'python']
print(l1)    # [3, 4, 5, 5, 6, 2, 'python', 'python']
```

#### Indexing and Slicing

```python
# Index diagram:
# list1    = [10, 20, 30, 15, 45, 25, 76]
# pos_index:  0   1   2   3   4   5   6
# neg_index: -7  -6  -5  -4  -3  -2  -1

x = [10, 20, 30, 15, 45, 25, 76]

print(x[0])      # 10
print(x[1])      # 20
print(x[-1])     # 76
print(x[-7])     # 10
print(x[6])      # 76
# print(x[7])    # IndexError: list index out of range
```

```python
# Slicing
x = [10, 20, 30, 15, 45, 25, 76]

print(x[:])      # [10, 20, 30, 15, 45, 25, 76] — full list
print(x[4:])     # [45, 25, 76] — from index 4 to end
print(x[:4])     # [10, 20, 30, 15] — from start to index 3
print(x[4:0])    # [] — empty! (start > stop with positive step)
print(x[4:0:-1]) # [45, 15, 30, 20] — reverse from index 4 to 1
print(x[::-1])   # [76, 25, 45, 15, 30, 20, 10] — full reverse
print(x[::2])    # [10, 30, 45, 76] — every 2nd element
```

#### List Methods 

```python
# append() — add one element to end
l = [1, 2, 3]
l.append(4)
print(l)    # [1, 2, 3, 4]
l.append([5, 6])
print(l)    # [1, 2, 3, 4, [5, 6]] — appends as single element!

# extend() — add multiple elements
l = [1, 2, 3]
l.extend([4, 5, 6])
print(l)    # [1, 2, 3, 4, 5, 6] — adds each element individually

# insert() — add at specific index
l = [1, 2, 3]
l.insert(1, 'hello')
print(l)    # [1, 'hello', 2, 3]
```

```python
# remove() — remove first occurrence by value
l = [1, 2, 3, 2, 4]
l.remove(2)
print(l)    # [1, 3, 2, 4] — only first 2 is removed!
# l.remove(99)  # ValueError: list.remove(x): x not in list

# pop() — remove by index (default: last element)
l = [1, 2, 3, 4, 5]
removed = l.pop()
print(removed, l)    # 5 [1, 2, 3, 4]
removed = l.pop(1)
print(removed, l)    # 2 [1, 3, 4]

# clear() — remove all elements
l = [1, 2, 3]
l.clear()
print(l)    # []

# del — delete by index or entire list
l = [1, 2, 3, 4, 5]
del l[2]
print(l)    # [1, 2, 4, 5]
```

```python
# sort() — sort in-place (returns None!)
l = [3, 1, 4, 1, 5, 9, 2, 6]
l.sort()
print(l)    # [1, 1, 2, 3, 4, 5, 6, 9]

l.sort(reverse=True)
print(l)    # [9, 6, 5, 4, 3, 2, 1, 1]

# sorted() — returns NEW sorted list
l = [3, 1, 4, 1, 5]
new_l = sorted(l)
print(new_l)    # [1, 1, 3, 4, 5]
print(l)        # [3, 1, 4, 1, 5] — original unchanged!

# reverse() — reverse in-place
l = [1, 2, 3]
l.reverse()
print(l)    # [3, 2, 1]

# count() — count occurrences
l = [1, 2, 2, 3, 2]
print(l.count(2))    # 3

# index() — find first occurrence
l = [10, 20, 30, 20]
print(l.index(20))    # 1
```

```python
# copy() — shallow copy
l1 = [1, 2, 3]
l2 = l1.copy()    # Creates a new list
l2.append(4)
print(l1)    # [1, 2, 3] — unchanged!
print(l2)    # [1, 2, 3, 4]

# Without copy — both point to same list!
l1 = [1, 2, 3]
l2 = l1          # l2 is just an alias!
l2.append(4)
print(l1)    # [1, 2, 3, 4] — CHANGED! (same object)
```

> **⚠️ Key Insights & Common Mistakes**
> - `append()` adds ONE element; `extend()` adds EACH element from an iterable. `l.append([4,5])` adds `[4,5]` as a single nested element!
> - `sort()` sorts **in-place** and returns `None`! Do NOT write `l = l.sort()` — this sets `l` to `None`.
> - `sorted()` returns a **new list**. `sort()` modifies the original.
> - `l2 = l1` does NOT create a copy — both variables point to the **same list**. Use `l2 = l1.copy()` or `l2 = l1[:]`.
> - `remove()` removes the **first** occurrence only. `pop()` removes by **index** (default: last).
> - Lists can contain **any data type** including other lists (nested lists).
> - Set cannot contain lists (unhashable), but a list can contain sets.

---

### 📝 Assignment Questions — Chapter 26

1. What is the difference between `append()` and `extend()`? Show with examples.
2. What is the difference between `sort()` and `sorted()`?
3. What happens if you write `l2 = l1` instead of `l2 = l1.copy()`?
4. How do you remove all occurrences of a value from a list?
5. Why does `{12, 23.4, [1,2,3]}` raise `TypeError` but `[12, 23.4, {1,2,3}]` works?

---

## Chapter 27: List Comprehensions

### 27.1 Theory

**List comprehension** is a concise, Pythonic way to create lists. It replaces multi-line `for` loops with a single expression. List comprehensions are faster than equivalent `for` loops and are widely used in Data Science.

### 27.2 Syntax

```python
new_list = [expression for item in iterable]
new_list = [expression for item in iterable if condition]
new_list = [expression if condition else alternative for item in iterable]
```

### 27.3 Practice Examples 

```python
# Basic: squares of 1 to 5
squares = [x**2 for x in range(1, 6)]
print(squares)    # [1, 4, 9, 16, 25]

# With condition: even numbers
evens = [x for x in range(1, 11) if x % 2 == 0]
print(evens)    # [2, 4, 6, 8, 10]

# With if-else: even/odd labels
labels = ['Even' if x % 2 == 0 else 'Odd' for x in range(1, 6)]
print(labels)    # ['Odd', 'Even', 'Odd', 'Even', 'Odd']

# String processing
words = ['hello', 'world', 'python']
upper_words = [w.upper() for w in words]
print(upper_words)    # ['HELLO', 'WORLD', 'PYTHON']
```

```python
# Nested list comprehension — flattening
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
flat = [num for row in matrix for num in row]
print(flat)    # [1, 2, 3, 4, 5, 6, 7, 8, 9]
```

```python
# Set comprehension
unique_lengths = {len(word) for word in ['hello', 'world', 'hi', 'bye']}
print(unique_lengths)    # {2, 3, 5}

# Dict comprehension
squares_dict = {x: x**2 for x in range(1, 6)}
print(squares_dict)    # {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

# Generator expression (lazy — doesn't create list in memory)
gen = (x**2 for x in range(1000000))
print(sum(gen))    # Efficient — doesn't store 1M items in memory
```

> **⚠️ Key Insights & Common Mistakes**
> - List comprehension is **faster** than a for loop — use it when possible.
> - The `if` condition comes **after** the `for` (for filtering). The `if-else` comes **before** the `for` (for transformation).
> - Don't make comprehensions too complex — if it's hard to read, use a regular loop.
> - Use `()` for **generator expression** (memory efficient), `[]` for list, `{}` for set/dict.

---

### 📝 Assignment Questions — Chapter 27

1. Write a list comprehension to get all even numbers from 1 to 50.
2. Write a list comprehension to convert a list of Celsius to Fahrenheit.
3. Flatten the matrix `[[1,2],[3,4],[5,6]]` using a list comprehension.
4. What is the difference between a list comprehension and a generator expression?
5. Create a dictionary comprehension that maps words to their lengths.

---

## Chapter 28: Tuples

### 28.1 Theory

A **tuple** is an **ordered, immutable** collection. Once created, a tuple cannot be modified — you cannot add, remove, or change elements. Tuples are used when data should not change (e.g., coordinates, database records, function return values).

**Key Properties :**
1. **Immutable** — cannot add, delete, or modify elements
2. **Ordered** — maintains insertion order
3. **Comma separated**
4. **Duplicates are allowed**
5. Tuples are enclosed by **parentheses** `()`

### 28.2 Syntax

```python
t = ()                    # Empty tuple
t = (1,)                  # Single element tuple (comma required!)
t = (1, 2, 3)            # Tuple with elements
t = 1, 2, 3              # Tuple without parentheses (tuple packing)
```

### 28.3 Extensive Practice Examples 

```python
# Creating tuples — WATCH the comma rule!
tup1 = ()
print(type(tup1))    # <class 'tuple'>

tup1 = (1)
print(type(tup1))    # <class 'int'> — NOT a tuple! Just parenthesised number.

tup1 = (1,)
print(type(tup1))    # <class 'tuple'> — comma makes it a tuple!

x = 3
print(type(x))       # <class 'int'>

x = 3,
print(type(x))       # <class 'tuple'> — comma creates a tuple!
```

```python
# Heterogeneous tuple
tup1 = 3, 2.4, 3+4j, 'python', [23,4,5], (5,6), {5,6}
print(type(tup1))    # <class 'tuple'>
print(tup1)          # (3, 2.4, (3+4j), 'python', [23, 4, 5], (5, 6), {5, 6})
```

```python
# Indexing and slicing (same as lists)
tup1 = 3, 2.4, 3+4j, 'python', [23,4,5], (5,6), {5,6}
print(tup1[0])       # 3
print(tup1[-1])      # {5, 6}
print(tup1[:4])      # (3, 2.4, (3+4j), 'python')

# You can index nested mutable elements inside a tuple
print(tup1[4][1])    # 4 (accessing list inside tuple)
```

```python
# Tuple is immutable — cannot assign!
tup1 = 3, 2.4, 3+4j, 'python', [23,4,5], 5, (5,6), {5,6}
# tup1[5] = 500      # TypeError: 'tuple' object does not support item assignment
# del tup1[4]         # TypeError: 'tuple' object doesn't support item deletion
```

```python
# BUT! Mutable objects INSIDE a tuple CAN be changed
tup1 = (1, 2, [3, 4, 5])
tup1[2][0] = 99
print(tup1)    # (1, 2, [99, 4, 5]) — the list inside changed!
```

```python
# Sets cannot be indexed
tup1 = 3, 2.4, 3+4j, 'python', [23,4,5], (5,6), {5,6}
# tup1[-1][0]    # TypeError: 'set' object is not subscriptable
```

```python
# Tuple has only 2 methods
x = (6, 2, 4, 8, 1, 3, 7, 2, 2)
# x.append(2)    # AttributeError: 'tuple' object has no attribute 'append'

print(x.count(2))    # 3 (count occurrences of 2)
print(x.index(8))    # 3 (index of first occurrence of 8)
```

```python
# Tuple unpacking
a, b, c = (10, 20, 30)
print(a, b, c)    # 10 20 30

# Swapping using tuple unpacking
a, b = 10, 20
a, b = b, a
print(a, b)    # 20 10

# Extended unpacking
first, *rest = (1, 2, 3, 4, 5)
print(first)    # 1
print(rest)     # [2, 3, 4, 5]
```

### 28.4 List vs Tuple 

| Feature | List | Tuple |
|---------|------|-------|
| Syntax | `[1, 2, 3]` | `(1, 2, 3)` |
| Mutable? | Yes | No |
| Methods | Many (append, sort, etc.) | Only `count()` and `index()` |
| Speed | Slower | Faster |
| Memory | More | Less |
| Use as dict key? | No | Yes |
| Use in set? | No | Yes |

> **⚠️ Key Insights & Common Mistakes**
> - `(1)` is NOT a tuple — it's just `1` in parentheses. Use `(1,)` with a trailing comma!
> - Similarly, `x = 3,` creates a tuple. Be careful with accidental trailing commas.
> - Tuples have only **2 methods**: `count()` and `index()`. No `append`, `sort`, `remove`, etc.
> - Mutable objects inside tuples (e.g., lists) CAN be changed, even though the tuple itself is immutable.
> - Tuples can be used as **dictionary keys** and **set elements** because they are hashable (if they contain only immutable elements).

---

### 📝 Assignment Questions — Chapter 28

1. What is the difference between `(1)` and `(1,)`? Check their types.
2. Why are tuples faster than lists?
3. Can you change a list that is inside a tuple? Demonstrate.
4. What methods are available for tuples?
5. When would you use a tuple instead of a list?

---

## Chapter 29: Sets and Frozensets

### 29.1 Theory

A **set** is an **unordered, mutable** collection with **no duplicate elements**. Sets are used for membership testing, removing duplicates, and mathematical set operations (union, intersection, difference).

**Key Properties :**

| Property | str | list | tuple | set |
|----------|-----|------|-------|-----|
| Ordered? | Yes | Yes | Yes | **No** |
| Mutable? | No | Yes | No | **Yes** |
| Duplicates? | Yes | Yes | Yes | **No** |
| Syntax | `''`, `""` | `[]` | `()` | `{}`, `set()` |

Sets can only store **immutable (hashable) datatypes**: `int`, `float`, `complex`, `str`, `tuple`, `frozenset`.

### 29.2 Syntax

```python
s = set()                # Empty set (NOT {}!)
s = {1, 2, 3}           # Set with elements
fs = frozenset({1,2,3}) # Immutable set
```

### 29.3 Extensive Practice Examples 

```python
# IMPORTANT: {} creates a dict, NOT a set!
d = {}
print(type(d))    # <class 'dict'>

s = set()
print(type(s))    # <class 'set'>

var = {1, 2, 3, 4}
print(type(var), var)    # <class 'set'> {1, 2, 3, 4}
```

```python
# Sets remove duplicates automatically
set1 = {2, 3, 1, 3, 2, 3, 2, 5, 6, 'data', 'Pune', 'data', 'pune', 'Data', 'Pune'}
print(len(set1), set1)
# Output: 9 {1, 2, 3, 5, 6, 'data', 'Data', 'Pune', 'pune'}
# Note: 'data', 'Data', 'pune', 'Pune' are all different (case-sensitive!)
```

```python
# Removing duplicates from a list using set
list1 = [2, 3, 1, 3, 2, 3, 2, 5, 6, 'data', 'Pune', 'data', 'pune', 'Data', 'Pune']
s1 = set(list1)
print(s1, len(s1))
# Output: {1, 2, 3, 5, 6, 'data', 'Data', 'Pune', 'pune'} 9

list2 = list(s1)
print(list2)    # Unique elements as a list
```

```python
# What can go inside a set? Only IMMUTABLE types!
# Lists CANNOT be in sets
# s1 = {1, 2.3, [1,2,3]}    # TypeError: unhashable type: 'list'

# Sets CANNOT be in sets
# s1 = {1, 2.3, {5,6,7}}    # TypeError: unhashable type: 'set'

# Dicts CANNOT be in sets
# s1 = {1, 2.3, {'a':1}}    # TypeError: unhashable type: 'dict'

# Tuples and frozensets CAN be in sets
s1 = {1, 2.3, 3+4j, 'data', (4,5,6), frozenset({7,8,9})}
print(s1)    # Works!
```

#### Set Methods

```python
s = {1, 2, 3}

# add() — add one element
s.add(4)
print(s)    # {1, 2, 3, 4}

# update() — add multiple elements
s.update([5, 6, 7])
print(s)    # {1, 2, 3, 4, 5, 6, 7}

# remove() — remove element (raises KeyError if not found)
s.remove(3)
print(s)    # {1, 2, 4, 5, 6, 7}
# s.remove(99)    # KeyError!

# discard() — remove element (NO error if not found)
s.discard(99)    # No error!
print(s)         # {1, 2, 4, 5, 6, 7}

# pop() — remove and return arbitrary element
item = s.pop()
print(item)    # Could be any element (unordered!)
```

#### Set Operations (Mathematical)

```python
A = {1, 2, 3, 4, 5}
B = {4, 5, 6, 7, 8}

# Union — all elements from both
print(A | B)               # {1, 2, 3, 4, 5, 6, 7, 8}
print(A.union(B))          # Same

# Intersection — common elements
print(A & B)               # {4, 5}
print(A.intersection(B))   # Same

# Difference — in A but not in B
print(A - B)               # {1, 2, 3}
print(A.difference(B))     # Same

# Symmetric Difference — in A or B but not both
print(A ^ B)                        # {1, 2, 3, 6, 7, 8}
print(A.symmetric_difference(B))    # Same
```

### 29.4 Frozenset

```python
# Frozenset is an immutable set
fs = frozenset([1, 2, 3, 4])
print(fs)    # frozenset({1, 2, 3, 4})

# Cannot add or remove
# fs.add(5)       # AttributeError
# fs.remove(1)    # AttributeError

# Can use as dict key or set element
d = {frozenset({1,2}): 'value'}    # Works!
s = {frozenset({1,2}), frozenset({3,4})}    # Works!
```

> **⚠️ Key Insights & Common Mistakes**
> - `{}` creates a **dict**, NOT a set! Use `set()` for an empty set.
> - Sets are **unordered** — you cannot access elements by index: `s[0]` raises `TypeError`.
> - `remove()` raises `KeyError` if element not found. Use `discard()` for safe removal.
> - Sets can only contain **immutable** (hashable) types. Lists, sets, and dicts cannot be set elements.
> - **Frozenset** is the immutable version of set — can be used as dict key or set element.
> - Converting a list to a set and back is a common trick to remove duplicates: `list(set(my_list))`.

---

### 📝 Assignment Questions — Chapter 29

1. How do you create an empty set? Why can't you use `{}`?
2. What types of objects can be stored in a set? What cannot?
3. What is the difference between `remove()` and `discard()`?
4. Write code to find common elements between two lists using sets.
5. What is a frozenset? When would you use it?

---

## Chapter 30: Dictionaries

### 30.1 Theory

A **dictionary** (`dict`) is a collection of **key-value pairs**. It is the most important mapping type in Python and is used extensively in Data Science for data manipulation, JSON handling, and API responses.

**Key Properties :**
1. Collection of **key-value pairs**: `{key: value}`
2. **Duplicate keys not allowed** (last value wins)
3. **Duplicate values are allowed**
4. Comma separated
5. Enclosed by `{}`
6. **Cannot use indexing** (access by key, not by position)
7. **Mutable** — can add, modify, delete key-value pairs
8. **Keys must be immutable**: `int`, `float`, `str`, `complex`, `tuple`, `frozenset`
9. **Values can be any type**: `int`, `float`, `str`, `list`, `dict`, `set`, etc.
10. Ordered (Python 3.7+), Unordered (Python < 3.7)

### 30.2 Syntax

```python
d = {}                            # Empty dict
d = dict()                        # Empty dict
d = {'key1': 'value1', 'key2': 'value2'}
d = dict(name='Alice', age=25)    # Using keyword arguments
```

### 30.3 Extensive Practice Examples 

```python
dict1 = {'A': 100, 'B': 200}
print(dict1)         # {'A': 100, 'B': 200}
print(len(dict1))    # 2
```

```python
# Duplicate keys — last value wins!
dict1 = {'A': 100, 'B': 200, 'C': 300, 'A': 400}
print(dict1)    # {'A': 400, 'B': 200, 'C': 300}
# 'A' appears twice — the last value (400) overwrites the first (100)!
```

```python
# Keys must be immutable (hashable)
dict2 = {1: 1, 2.0: 4, '3': 9, (1,2,3): 16}
print(dict2)    # Works!

# dict2 = {1: 1, [1,2,3]: 16}    # TypeError: unhashable type: 'list'
# dict2 = {1: 1, {1,2,3}: 16}    # TypeError: unhashable type: 'set'
```

```python
# Nested dictionary
dict3 = {
    'Employee1': {
        'Name': 'Mrunali',
        'Age': 26,
        'Location': 'Pune',
        'Salary': 34000
    },
    'Employee2': {
        'Name': 'Prathamesh',
        'Age': 22,
        'Location': 'Mumbai',
        'Salary': 12000
    }
}

print(dict3['Employee1'])              # {'Name': 'Mrunali', ...}
print(dict3['Employee2']['Salary'])    # 12000
print(len(dict3))                      # 2 (two top-level keys)

# dict3[0]    # KeyError: 0 — dicts use KEYS, not indices!
```

#### Accessing Dictionary Items

```python
dict1 = {'Name': 'Mrunali', 'Age': 26, 'Location': 'Pune'}

# Using [] — raises KeyError if key not found
print(dict1['Name'])        # Mrunali
# print(dict1['Salary'])    # KeyError: 'Salary'

# Using .get() — returns None (or default) if key not found
print(dict1.get('Name'))       # Mrunali
print(dict1.get('Salary'))     # None (no error!)
print(dict1.get('Salary', 0))  # 0 (custom default)
```

#### Dictionary Methods

```python
d = {'A': 1, 'B': 2, 'C': 3}

print(d.keys())      # dict_keys(['A', 'B', 'C'])
print(d.values())    # dict_values([1, 2, 3])
print(d.items())     # dict_items([('A', 1), ('B', 2), ('C', 3)])

# Adding / Updating
d['D'] = 4           # Add new key
d['A'] = 100         # Update existing key
print(d)             # {'A': 100, 'B': 2, 'C': 3, 'D': 4}

d.update({'E': 5, 'A': 999})
print(d)             # {'A': 999, 'B': 2, 'C': 3, 'D': 4, 'E': 5}

# Removing
del d['E']
print(d)             # {'A': 999, 'B': 2, 'C': 3, 'D': 4}

popped = d.pop('D')
print(popped)        # 4
print(d)             # {'A': 999, 'B': 2, 'C': 3}

last = d.popitem()   # Remove last inserted item
print(last)          # ('C', 3)
```

```python
# Creating dicts from lists
keys = ['name', 'age', 'city']
values = ['Alice', 25, 'Pune']

d = dict(zip(keys, values))
print(d)    # {'name': 'Alice', 'age': 25, 'city': 'Pune'}

# fromkeys — create dict with default values
d = dict.fromkeys(['a', 'b', 'c'], 0)
print(d)    # {'a': 0, 'b': 0, 'c': 0}
```

> **⚠️ Key Insights & Common Mistakes**
> - Use `d.get(key)` instead of `d[key]` to avoid `KeyError` when a key might not exist.
> - Duplicate keys are silently overwritten — the **last value wins**. This is a common source of bugs.
> - `d[key]` raises `KeyError` if key doesn't exist. `d.get(key)` returns `None`.
> - `in` checks **keys**, not values: `'Alice' in {'name': 'Alice'}` is `False`!
> - Lists, sets, and dicts **cannot be used as dictionary keys** (unhashable).
> - `d.keys()`, `d.values()`, `d.items()` return **view objects**, not lists. Wrap with `list()` if needed.

---

### 📝 Assignment Questions — Chapter 30

1. What is the difference between `d['key']` and `d.get('key')`?
2. What happens when you have duplicate keys in a dictionary?
3. What types can be used as dictionary keys? What cannot?
4. How do you create a dictionary from two lists (one for keys, one for values)?
5. Write code to merge two dictionaries.

---

## Chapters 31–32: Dictionary Comprehensions and collections Module

### 31.1 Dictionary Comprehension

```python
# Basic
squares = {x: x**2 for x in range(1, 6)}
print(squares)    # {1: 1, 2: 4, 3: 9, 4: 16, 5: 25}

# With condition
even_squares = {x: x**2 for x in range(1, 11) if x % 2 == 0}
print(even_squares)    # {2: 4, 4: 16, 6: 36, 8: 64, 10: 100}

# Swapping keys and values
d = {'a': 1, 'b': 2, 'c': 3}
swapped = {v: k for k, v in d.items()}
print(swapped)    # {1: 'a', 2: 'b', 3: 'c'}
```

### 32.1 The `collections` Module

```python
from collections import Counter, defaultdict, namedtuple, deque

# Counter — count occurrences
words = ['apple', 'banana', 'apple', 'cherry', 'banana', 'apple']
count = Counter(words)
print(count)                   # Counter({'apple': 3, 'banana': 2, 'cherry': 1})
print(count.most_common(2))    # [('apple', 3), ('banana', 2)]

# defaultdict — dict with default values
dd = defaultdict(list)
dd['fruits'].append('apple')
dd['fruits'].append('banana')
dd['vegetables'].append('carrot')
print(dict(dd))    # {'fruits': ['apple', 'banana'], 'vegetables': ['carrot']}

# namedtuple — tuple with named fields
Point = namedtuple('Point', ['x', 'y'])
p = Point(3, 4)
print(p.x, p.y)    # 3 4

# deque — double-ended queue (fast append/pop from both ends)
dq = deque([1, 2, 3])
dq.appendleft(0)
dq.append(4)
print(dq)    # deque([0, 1, 2, 3, 4])
```

> **⚠️ Key Insights & Common Mistakes**
> - `Counter` is extremely useful for word frequency analysis in NLP/Data Science.
> - `defaultdict` prevents `KeyError` — it creates a default value automatically.
> - `namedtuple` is a lightweight alternative to classes for storing structured data.

---

### 📝 Assignment Questions — Chapters 31–32

1. Write a dictionary comprehension to create a dict mapping numbers 1–10 to "even"/"odd".
2. Use `Counter` to find the most common letter in a string.
3. When would you use `defaultdict` instead of a regular dict?
4. Create a `namedtuple` called `Student` with fields: name, age, grade.
5. What is the advantage of `deque` over a regular list?

---

# Part VI: Functions — The Building Blocks

---

## Chapter 33: Defining and Calling Functions

### 33.1 Theory

A **function** is a reusable block of code that performs a specific task. Functions help you:
- **Avoid repetition** (DRY principle — Don't Repeat Yourself)
- **Organise** code into logical blocks
- **Improve readability** and maintainability
- **Enable testing** of individual units of code

### 33.2 Syntax

```python
def function_name(parameters):
    """Docstring — describes what the function does"""
    statement(s)
    return value    # Optional
```

### 33.3 Practice Examples 

```python
# Simple function with no parameters
def greet():
    print('Hello, World!')

greet()    # Hello, World!
```

```python
# Function with parameters and return
def add(a, b):
    return a + b

result = add(3, 4)
print(result)    # 7
```

```python
# Function with docstring
def calculate_area(length, width):
    """Calculate the area of a rectangle.
    
    Args:
        length: The length of the rectangle
        width: The width of the rectangle
    
    Returns:
        The area (length × width)
    """
    return length * width

print(calculate_area(5, 3))    # 15
print(calculate_area.__doc__)   # Prints the docstring
```

```python
# Multiple return values (returns a tuple)
def min_max(numbers):
    return min(numbers), max(numbers)

lo, hi = min_max([3, 1, 4, 1, 5, 9])
print(lo, hi)    # 1 9
```

```python
# Function without return returns None
def say_hello(name):
    print(f'Hello, {name}!')

result = say_hello('Alice')    # Hello, Alice!
print(result)                   # None
```

> **⚠️ Key Insights & Common Mistakes**
> - A function without a `return` statement returns `None` by default.
> - `return` immediately exits the function — code after `return` never executes.
> - Function names should use **snake_case**: `calculate_total()`, not `CalculateTotal()`.
> - Always write a **docstring** for non-trivial functions — it helps others understand your code.

---

### 📝 Assignment Questions — Chapter 33

1. What is the purpose of a function in Python?
2. What is returned by a function that has no `return` statement?
3. Write a function that checks if a number is prime.
4. What is a docstring? How do you access it?
5. Can a function return multiple values? How?

---

## Chapter 34: Function Arguments — Positional, Default, *args, **kwargs

### 34.1 Theory

Python functions support several types of arguments:

| Type | Description | Example |
|------|------------|---------|
| Positional | Required, in order | `def f(a, b):` |
| Default | Has a default value | `def f(a, b=10):` |
| `*args` | Variable positional args (tuple) | `def f(*args):` |
| `**kwargs` | Variable keyword args (dict) | `def f(**kwargs):` |

### 34.2 Extensive Practice Examples 

```python
# Positional arguments (order matters!)
def power(base, exponent):
    return base ** exponent

print(power(2, 3))    # 8
print(power(3, 2))    # 9 (different! order matters)
```

```python
# Default arguments
def greet(name, greeting='Hello'):
    print(f'{greeting}, {name}!')

greet('Alice')              # Hello, Alice!
greet('Alice', 'Hi')        # Hi, Alice!
greet('Alice', 'Welcome')   # Welcome, Alice!
```

```python
# *args — accepts any number of positional arguments (as a tuple)
def total(*args):
    print(type(args))    # <class 'tuple'>
    return sum(args)

print(total(1, 2, 3))        # 6
print(total(1, 2, 3, 4, 5))  # 15
```

```python
# **kwargs — accepts any number of keyword arguments (as a dict)
def display_info(**kwargs):
    print(type(kwargs))    # <class 'dict'>
    for key, value in kwargs.items():
        print(f'{key}: {value}')

display_info(name='Alice', age=25, city='Pune')
# Output:
# name: Alice
# age: 25
# city: Pune
```

```python
# Combining all argument types (ORDER MATTERS!)
# Order: positional → *args → default → **kwargs
def func(a, b, *args, c=10, **kwargs):
    print(f'a={a}, b={b}')
    print(f'args={args}')
    print(f'c={c}')
    print(f'kwargs={kwargs}')

func(1, 2, 3, 4, c=20, name='Alice')
# Output:
# a=1, b=2
# args=(3, 4)
# c=20
# kwargs={'name': 'Alice'}
```

> **⚠️ Key Insights & Common Mistakes**
> - **Mutable default argument trap!** `def f(lst=[]):` is dangerous — the default list is shared across all calls. Use `def f(lst=None): if lst is None: lst = []`.
> - Default arguments are evaluated **once** at function definition, not at each call.
> - `*args` receives extra positional arguments as a **tuple**. `**kwargs` receives extra keyword arguments as a **dict**.
> - Order of parameters: `positional → *args → keyword/default → **kwargs`.

---

### 📝 Assignment Questions — Chapter 34

1. What is the difference between `*args` and `**kwargs`?
2. Demonstrate the mutable default argument trap and how to fix it.
3. What is the correct order of parameters in a function definition?
4. Write a function that accepts any number of numbers and returns the average.
5. Write a function that accepts any keyword arguments and prints them formatted.

---

## Chapter 35: Lambda Functions

### 35.1 Theory

A **lambda function** is an **anonymous** (nameless), one-line function. It is used for simple, short operations that don't need a full `def` block. Lambda functions are commonly used with `map()`, `filter()`, `sorted()`, and in Data Science pipelines.

### 35.2 Syntax

```python
lambda arguments: expression
```

The lambda function automatically **returns** the result of the expression (no `return` keyword needed).

### 35.3 Extensive Practice Examples 

```python
# Basic lambda
square = lambda x: x ** 2
print(square(5))       # 25

# Multiple arguments
add = lambda a, b: a + b
print(add(3, 4))       # 7

# Conditional in lambda
is_even = lambda x: 'Even' if x % 2 == 0 else 'Odd'
print(is_even(4))      # Even
print(is_even(7))      # Odd
```

```python
# Lambda with sorted()
students = [('Alice', 85), ('Bob', 92), ('Charlie', 78)]
sorted_students = sorted(students, key=lambda s: s[1], reverse=True)
print(sorted_students)
# [('Bob', 92), ('Alice', 85), ('Charlie', 78)]

# Sorting dictionaries by value
people = [{'name': 'Alice', 'age': 25}, {'name': 'Bob', 'age': 20}]
sorted_people = sorted(people, key=lambda p: p['age'])
print(sorted_people)
# [{'name': 'Bob', 'age': 20}, {'name': 'Alice', 'age': 25}]
```

> **⚠️ Key Insights & Common Mistakes**
> - Lambda is for **single expressions** only — no multi-line logic, no statements.
> - Lambda can't contain statements (`if-else` expression is OK, but `if:` block is NOT).
> - PEP 8 discourages assigning lambda to a variable: `f = lambda x: x` — use `def` instead.

---

### 📝 Assignment Questions — Chapter 35

1. Write a lambda to check if a string starts with a vowel.
2. Use lambda with `sorted()` to sort a list of dicts by a specific key.
3. What is the limitation of lambda compared to regular functions?

---

## Chapter 36: Recursive Functions

### 36.1 Theory

**Recursion** is when a function **calls itself**. Every recursive function must have:
1. **Base case** — the condition that stops the recursion
2. **Recursive case** — the function calling itself with a smaller/simpler input

### 36.2 Syntax

```python
def recursive_function(parameters):
    if base_condition:
        return base_value        # Base case — STOP
    return recursive_function(modified_parameters)    # Recursive case
```

### 36.3 Extensive Practice Examples 

```python
# Factorial: n! = n × (n-1) × ... × 1
def factorial(n):
    if n <= 1:
        return 1                   # Base case
    return n * factorial(n - 1)    # Recursive case

print(factorial(5))    # 120 (5 × 4 × 3 × 2 × 1)
print(factorial(0))    # 1
```

```python
# Fibonacci: 0, 1, 1, 2, 3, 5, 8, 13, 21, ...
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n-1) + fibonacci(n-2)

for i in range(10):
    print(fibonacci(i), end=' ')    # 0 1 1 2 3 5 8 13 21 34
```

```python
# Sum of digits
def sum_digits(n):
    if n < 10:
        return n
    return n % 10 + sum_digits(n // 10)

print(sum_digits(1234))    # 10 (1 + 2 + 3 + 4)
```

```python
# Power (x^n)
def power(x, n):
    if n == 0:
        return 1
    return x * power(x, n - 1)

print(power(2, 10))    # 1024
```

> **⚠️ Key Insights & Common Mistakes**
> - **Every recursion MUST have a base case** — without one, you get `RecursionError: maximum recursion depth exceeded`.
> - Python's default recursion limit is **1000**. Change with `sys.setrecursionlimit()` (use cautiously!).
> - Recursive Fibonacci is **O(2^n)** — extremely slow for large n. Use memoisation or iterative approach.
> - Recursion uses more memory (call stack) than iteration. Prefer iteration for large inputs.

---

### 📝 Assignment Questions — Chapter 36

1. Write a recursive function to reverse a string.
2. Write a recursive function to check if a string is a palindrome.
3. What happens if recursion has no base case?
4. Why is recursive Fibonacci slow? How can you optimise it?
5. Write a recursive function to flatten a nested list: `[1, [2, [3, 4]], 5]` → `[1, 2, 3, 4, 5]`.

---

## Chapter 37: Scope, LEGB Rule, and Closures

### 37.1 Theory

**Scope** determines where a variable is accessible. Python uses the **LEGB rule** to resolve variable names:

| Level | Name | Description |
|-------|------|------------|
| L | Local | Inside the current function |
| E | Enclosing | Inside enclosing (outer) functions |
| G | Global | At the module (file) level |
| B | Built-in | Python's built-in names (`print`, `len`, etc.) |

### 37.2 Extensive Practice Examples 

```python
# Global vs Local
player1 = 'Virat Kohli'    # Global variable

def cricket():
    print(player1)    # Can access global

cricket()    # Virat Kohli
print(player1)    # Virat Kohli
```

```python
# Local variable shadows global
player1 = 'Virat Kohli'    # Global

def cricket():
    player1 = 'Ayush Mhatre'    # Local — shadows global
    print(player1)

cricket()    # Ayush Mhatre
print(player1)    # Virat Kohli (global unchanged!)
```

```python
# Local variable cannot be accessed outside
player1 = 'Virat Kohli'

def cricket():
    player2 = 'Ayush Mhatre'    # Local
    print(player1)
    print(player2)

cricket()
# print(player2)    # NameError: name 'player2' is not defined
```

```python
# global keyword — modify global variable from inside function
player1 = 'Virat Kohli'

def ipl_t20():
    global player1
    player1 = 'Ayush Mhatre'
    print(player1)

ipl_t20()        # Ayush Mhatre
print(player1)   # Ayush Mhatre (global is changed!)
```

```python
# The UnboundLocalError trap!
player = 'Virat Kohli'

def ipl_t20():
    print(player)           # UnboundLocalError!
    player = 'Ayush Mhatre'

# ipl_t20()
# UnboundLocalError: cannot access local variable 'player' where it is not associated with a value
# Why? Python sees 'player = ...' later, so it treats 'player' as LOCAL for the entire function.
# But you're trying to print it BEFORE it's assigned locally!
```

```python
# global keyword to declare variables accessible outside
player1 = 'Virat Kohli'

def ipl_t20():
    global player2, player3
    player2 = 'Ayush Mhatre'
    player3 = 'Vaibhav Suryawanshi'
    print(player1)
    print(player2)
    print(player3)

ipl_t20()
# Virat Kohli
# Ayush Mhatre
# Vaibhav Suryawanshi

print(player2)    # Ayush Mhatre (accessible because of global!)
print(player3)    # Vaibhav Suryawanshi
```

### 37.3 Closures

```python
def outer(x):
    def inner(y):
        return x + y    # inner "remembers" x from outer
    return inner

add5 = outer(5)
print(add5(3))     # 8
print(add5(10))    # 15
```

> **⚠️ Key Insights & Common Mistakes**
> - **UnboundLocalError** is one of the most confusing Python errors: if you assign to a variable anywhere in a function, Python treats it as local for the **entire** function, even before the assignment line.
> - Use `global` to modify global variables from inside a function (but avoid overusing it).
> - Use `nonlocal` to modify variables from an enclosing function scope.
> - A **closure** is a function that remembers variables from its enclosing scope, even after that scope has ended.
> - Avoid using `global` — it makes code harder to test and debug. Pass data through parameters and return values instead.

---

### 📝 Assignment Questions — Chapter 37

1. What is the LEGB rule? Explain each level.
2. What causes `UnboundLocalError`? How do you fix it?
3. What is the `global` keyword? When should you avoid it?
4. Write a closure that creates a multiplier function.
5. What is the difference between `global` and `nonlocal`?

---

## Chapter 38: Higher-Order Functions — map, filter, reduce

### 38.1 Theory

**Higher-order functions** are functions that take other functions as arguments or return functions. Python's built-in `map()`, `filter()`, and `functools.reduce()` are the most common.

### 38.2 Syntax

```python
map(function, iterable)           # Apply function to each element
filter(function, iterable)        # Keep elements where function returns True
reduce(function, iterable)        # Accumulate values (from functools)
```

### 38.3 Practice Examples 

```python
# map() — apply function to every element
numbers = [1, 2, 3, 4, 5]
squares = list(map(lambda x: x**2, numbers))
print(squares)    # [1, 4, 9, 16, 25]

# Celsius to Fahrenheit
celsius = [0, 20, 37, 100]
fahrenheit = list(map(lambda c: c * 9/5 + 32, celsius))
print(fahrenheit)    # [32.0, 68.0, 98.6, 212.0]
```

```python
# filter() — keep elements matching condition
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
evens = list(filter(lambda x: x % 2 == 0, numbers))
print(evens)    # [2, 4, 6, 8, 10]

words = ['hi', 'hello', 'hey', 'greetings']
long_words = list(filter(lambda w: len(w) > 3, words))
print(long_words)    # ['hello', 'greetings']
```

```python
# reduce() — accumulate values
from functools import reduce

numbers = [1, 2, 3, 4, 5]
total = reduce(lambda a, b: a + b, numbers)
print(total)    # 15

maximum = reduce(lambda a, b: a if a > b else b, numbers)
print(maximum)    # 5
```

> **⚠️ Key Insights & Common Mistakes**
> - `map()` and `filter()` return **iterators** in Python 3, not lists. Wrap with `list()` to see results.
> - List comprehensions are usually **more Pythonic** than `map()`/`filter()`.
> - `reduce()` is in `functools`, not a built-in. Prefer `sum()`, `max()`, etc. for common operations.

---

## Chapter 39: Built-in Functions — A Complete Reference

### 39.1 Key Built-in Functions

```python
# Numeric
print(abs(-7))              # 7
print(round(3.14159, 2))    # 3.14
print(round(2.5))           # 2 (banker's rounding!)
print(divmod(17, 5))        # (3, 2) → (quotient, remainder)
print(pow(2, 10))           # 1024

# Sequences
print(len([1, 2, 3]))       # 3
print(sum([1, 2, 3]))       # 6
print(min(3, 1, 2))         # 1
print(max(3, 1, 2))         # 3
print(sorted([3, 1, 2]))    # [1, 2, 3]
print(list(reversed([1,2,3])))  # [3, 2, 1]

# Boolean
print(any([False, True, False]))    # True
print(all([True, True, False]))     # False

# Type conversion
print(int('42'))        # 42
print(float('3.14'))    # 3.14
print(str(42))          # '42'
print(list('abc'))      # ['a', 'b', 'c']

# zip and enumerate
names = ['Alice', 'Bob']
ages = [25, 30]
print(list(zip(names, ages)))    # [('Alice', 25), ('Bob', 30)]

for i, name in enumerate(['Alice', 'Bob'], start=1):
    print(f'{i}. {name}')
# 1. Alice
# 2. Bob
```

> **⚠️ Key Insights & Common Mistakes**
> - `sorted()` returns a **new list**. `list.sort()` sorts **in-place** and returns `None`.
> - `round(2.5)` → `2` (not 3!) — Python uses **banker's rounding** (round half to even).
> - `zip()` stops at the **shortest** iterable. Use `itertools.zip_longest()` to keep all.
> - `reversed()` returns an **iterator**, not a list. Wrap with `list()` if needed.

---

### 📝 Assignment Questions — Chapters 38–39

1. Use `map()` to convert a list of strings to uppercase.
2. Use `filter()` to get all prime numbers from 1 to 50.
3. What is the difference between `any()` and `all()`?
4. Use `zip()` to create a dictionary from two lists.
5. Explain banker's rounding with examples.

---

# Part VII: Modules, Packages, and Virtual Environments

---

## Chapter 40: Creating and Importing Modules

### 40.1 Theory

A **module** is a Python file (`.py`) containing functions, classes, and variables that can be reused in other programs. Modules help you organise code into separate files and avoid putting everything in one giant file.

### 40.2 Syntax

```python
import module_name                          # Import entire module
import module_name as alias                 # Import with alias
from module_name import function_name       # Import specific function
from module_name import *                   # Import everything (not recommended)
```

### 40.3 Practice Examples

```python
import math
print(math.pi)          # 3.141592653589793
print(math.sqrt(16))    # 4.0
print(math.factorial(5))    # 120

import math as m
print(m.pi)    # 3.141592653589793

from math import pi, sqrt
print(pi)          # 3.141592653589793
print(sqrt(25))    # 5.0
```

```python
import random
print(random.randint(1, 100))    # Random int between 1 and 100
print(random.choice(['apple', 'banana', 'mango']))    # Random choice
print(random.random())    # Random float between 0 and 1

import os
print(os.getcwd())    # Current working directory
print(os.listdir())   # List files in current directory
```

> **⚠️ Key Insights & Common Mistakes**
> - Avoid `from module import *` — it pollutes the namespace and makes it unclear where names come from.
> - **Never name your file the same as a standard library module** (e.g., don't create `math.py` or `random.py`) — Python will import your file instead of the built-in!
> - Use aliases for long module names: `import numpy as np`, `import pandas as pd`.

---

### 📝 Assignment Questions — Chapter 40

1. What is a module in Python?
2. What is the difference between `import math` and `from math import pi`?
3. Why should you avoid `from module import *`?
4. What happens if you name your file `random.py` and then `import random`?
5. List five commonly used built-in Python modules.

---

## Chapters 41–44: Packages, Virtual Environments, datetime, math/random

### 41: Packages

A **package** is a directory containing multiple modules and an `__init__.py` file.

```
my_package/
    __init__.py
    module1.py
    module2.py
```

### 42: Virtual Environments and pip

```bash
# Create virtual environment
python -m venv myenv

# Activate
source myenv/bin/activate        # Linux/Mac
myenv\Scripts\activate           # Windows

# Install packages
pip install numpy pandas matplotlib
pip install -r requirements.txt

# Freeze requirements
pip freeze > requirements.txt

# Deactivate
deactivate
```

### 43: datetime Module

```python
from datetime import datetime, date, timedelta

now = datetime.now()
print(now)                              # 2025-12-15 10:30:45.123456
print(now.strftime('%Y-%m-%d'))         # 2025-12-15
print(now.strftime('%d/%m/%Y %H:%M'))   # 15/12/2025 10:30

tomorrow = date.today() + timedelta(days=1)
print(tomorrow)
```

### 44: math and random

```python
import math
print(math.pi)          # 3.141592653589793
print(math.e)           # 2.718281828459045
print(math.ceil(4.2))   # 5
print(math.floor(4.8))  # 4
print(math.log(100, 10))   # 2.0

import random
print(random.randint(1, 10))
print(random.choice(['a', 'b', 'c']))
print(random.sample(range(100), 5))    # 5 unique random numbers
random.shuffle([1, 2, 3, 4, 5])       # Shuffle in-place
```

> **⚠️ Key Insights & Common Mistakes**
> - Always use **virtual environments** for projects to avoid package conflicts.
> - `math.ceil()` rounds UP, `math.floor()` rounds DOWN, `round()` rounds to nearest (banker's).
> - `random.sample()` returns unique elements. `random.choices()` allows repeats.

---

### 📝 Assignment Questions — Chapters 41–44

1. What is the purpose of a virtual environment?
2. How do you freeze your current package versions?
3. Write code to display today's date in "DD-MM-YYYY" format.
4. What is the difference between `math.ceil()` and `math.floor()`?
5. Generate a list of 10 random numbers between 1 and 100.

---

# Part VIII: File Handling and Data Persistence

---

## Chapter 45: File Handling — Read, Write, Append

### 45.1 Theory

**File handling** allows Python to read from and write to files on disk. This is essential for data processing, log management, and persistence.

### 45.2 Syntax

```python
# Open a file
file = open(filename, mode)

# Modes:
# 'r'  — Read (default). Error if file doesn't exist.
# 'w'  — Write. Creates file or OVERWRITES existing.
# 'a'  — Append. Creates file or adds to end.
# 'r+' — Read and Write.
# 'rb' — Read binary.
# 'wb' — Write binary.
```

### 45.3 Practice Examples

```python
# Writing to a file
with open('test.txt', 'w') as f:
    f.write('Hello, World!\n')
    f.write('Python is great.\n')

# Reading a file
with open('test.txt', 'r') as f:
    content = f.read()
    print(content)
# Output:
# Hello, World!
# Python is great.

# Reading line by line
with open('test.txt', 'r') as f:
    for line in f:
        print(line.strip())

# Reading all lines into a list
with open('test.txt', 'r') as f:
    lines = f.readlines()
    print(lines)    # ['Hello, World!\n', 'Python is great.\n']

# Appending to a file
with open('test.txt', 'a') as f:
    f.write('Data Science rocks!\n')
```

### 45.4 JSON Files

```python
import json

# Writing JSON
data = {'name': 'Alice', 'age': 25, 'skills': ['Python', 'SQL']}
with open('data.json', 'w') as f:
    json.dump(data, f, indent=4)

# Reading JSON
with open('data.json', 'r') as f:
    loaded = json.load(f)
    print(loaded['name'])    # Alice
```

### 45.5 CSV Files

```python
import csv

# Writing CSV
with open('data.csv', 'w', newline='') as f:
    writer = csv.writer(f)
    writer.writerow(['Name', 'Age', 'City'])
    writer.writerow(['Alice', 25, 'Pune'])
    writer.writerow(['Bob', 30, 'Mumbai'])

# Reading CSV
with open('data.csv', 'r') as f:
    reader = csv.reader(f)
    for row in reader:
        print(row)
# ['Name', 'Age', 'City']
# ['Alice', '25', 'Pune']
# ['Bob', '30', 'Mumbai']
```

> **⚠️ Key Insights & Common Mistakes**
> - **Always use `with` statement** (context manager) — it automatically closes the file, even if an error occurs.
> - `'w'` mode **overwrites** the file! Use `'a'` to append.
> - Forgetting `newline=''` in CSV writer on Windows causes extra blank lines.
> - Always specify encoding: `open('file.txt', 'r', encoding='utf-8')` to avoid encoding errors.

---

### 📝 Assignment Questions — Chapter 45

1. What is the difference between `'w'`, `'r'`, and `'a'` modes?
2. Why should you always use `with` when opening files?
3. Write code to read a JSON file and print all keys.
4. How do you handle file encoding issues?
5. Write a program that counts the number of lines and words in a text file.

---

## Chapters 46–47: Context Managers and Pickle

### 46: Context Managers

```python
# The 'with' statement IS a context manager
with open('file.txt', 'w') as f:
    f.write('Hello')
# f is automatically closed here — even if an error occurs!

# Custom context manager
class FileManager:
    def __init__(self, filename, mode):
        self.file = open(filename, mode)
    
    def __enter__(self):
        return self.file
    
    def __exit__(self, exc_type, exc_val, exc_tb):
        self.file.close()
```

### 47: Pickle (Binary Serialisation)

```python
import pickle

# Save Python objects to binary file
data = {'model': 'RandomForest', 'accuracy': 0.95, 'features': ['age', 'income']}
with open('model.pkl', 'wb') as f:
    pickle.dump(data, f)

# Load
with open('model.pkl', 'rb') as f:
    loaded = pickle.load(f)
    print(loaded)
```

> **⚠️ Key Insights & Common Mistakes**
> - **Never unpickle data from untrusted sources** — it can execute arbitrary code!
> - Pickle is Python-specific. Use JSON for cross-language compatibility.

---

# Part IX: Error and Exception Handling

---

## Chapter 48: Exception Handling — try, except, finally

### 48.1 Theory

**Exceptions** are errors that occur during program execution. Without handling, they crash the program. Python's exception handling mechanism (`try-except-finally`) lets you catch errors and respond gracefully.

### 48.2 Syntax

```python
try:
    # Code that might raise an exception
    risky_code()
except ExceptionType as e:
    # Handle the specific exception
    print(f'Error: {e}')
except AnotherException:
    # Handle another type
    pass
else:
    # Executes if NO exception occurred
    print('Success!')
finally:
    # ALWAYS executes (cleanup code)
    print('Done.')
```

### 48.3 Common Exception Types

| Exception | When It Occurs |
|-----------|---------------|
| `SyntaxError` | Invalid Python syntax |
| `NameError` | Variable not defined |
| `TypeError` | Wrong type for operation |
| `ValueError` | Right type, wrong value |
| `IndexError` | Index out of range |
| `KeyError` | Dict key not found |
| `AttributeError` | Object has no such attribute |
| `ZeroDivisionError` | Division by zero |
| `FileNotFoundError` | File doesn't exist |
| `ImportError` | Module not found |
| `StopIteration` | Iterator exhausted |
| `RecursionError` | Maximum recursion depth exceeded |

### 48.4 Extensive Practice Examples

```python
# Basic try-except
try:
    result = 10 / 0
except ZeroDivisionError:
    print('Cannot divide by zero!')
# Output: Cannot divide by zero!
```

```python
# Multiple except blocks
try:
    num = int(input('Enter a number: '))
    result = 100 / num
    print(f'Result: {result}')
except ValueError:
    print('Please enter a valid number!')
except ZeroDivisionError:
    print('Cannot divide by zero!')
```

```python
# try-except-else-finally
try:
    f = open('test.txt', 'r')
    content = f.read()
except FileNotFoundError:
    print('File not found!')
else:
    print(f'File content: {content}')
finally:
    print('This always executes — cleanup code.')
```

```python
# Catching the exception message
try:
    x = [1, 2, 3]
    print(x[10])
except IndexError as e:
    print(f'Error: {e}')
# Output: Error: list index out of range
```

> **⚠️ Key Insights & Common Mistakes**
> - **Never use bare `except:`** — it catches ALL exceptions including `KeyboardInterrupt` and `SystemExit`. Always specify the exception type: `except ValueError:`.
> - `else` runs only if **no exception** occurred. `finally` runs **always** (even if there's a `return` in try/except).
> - Don't use exceptions for control flow — they are for **unexpected** errors, not normal logic.
> - Catch the **most specific** exception first, then more general ones.

---

### 📝 Assignment Questions — Chapter 48

1. What is the difference between `except ValueError:` and `except:`?
2. When does the `else` block execute in try-except-else?
3. When does the `finally` block execute?
4. Write a program that handles `FileNotFoundError` gracefully.
5. Why should you never use bare `except:`?

---

## Chapters 49–50: Custom Exceptions and Raising Exceptions

### 49: Custom Exceptions

```python
class InsufficientFundsError(Exception):
    def __init__(self, balance, amount):
        self.balance = balance
        self.amount = amount
        super().__init__(f'Cannot withdraw {amount}. Balance: {balance}')

def withdraw(balance, amount):
    if amount > balance:
        raise InsufficientFundsError(balance, amount)
    return balance - amount

try:
    withdraw(100, 200)
except InsufficientFundsError as e:
    print(e)    # Cannot withdraw 200. Balance: 100
```

### 50: Raising Exceptions

```python
def set_age(age):
    if not isinstance(age, int):
        raise TypeError('Age must be an integer')
    if age < 0 or age > 150:
        raise ValueError('Age must be between 0 and 150')
    return age

try:
    set_age(-5)
except ValueError as e:
    print(e)    # Age must be between 0 and 150
```

> **⚠️ Key Insights & Common Mistakes**
> - Custom exceptions should inherit from `Exception`, not `BaseException`.
> - Use `raise` to throw exceptions explicitly when input is invalid.
> - Always provide meaningful error messages in custom exceptions.

---

### 📝 Assignment Questions — Chapters 49–50

1. How do you create a custom exception class?
2. What is the difference between `raise` and `assert`?
3. Write a custom exception for invalid email format.
4. When should you raise exceptions vs. return error codes?
5. What is the exception hierarchy in Python?

---

# Part X: Regular Expressions

---

## Chapters 51–52: Regular Expressions

### 51.1 Theory

**Regular expressions** (regex) are patterns used to match, search, and manipulate text. Python's `re` module provides regex support. Regex is essential for data cleaning, validation, and text processing in Data Science.

### 51.2 Common Patterns

| Pattern | Meaning |
|---------|---------|
| `.` | Any character except newline |
| `\d` | Any digit (0-9) |
| `\D` | Any non-digit |
| `\w` | Any word character (letter, digit, _) |
| `\W` | Any non-word character |
| `\s` | Any whitespace |
| `\S` | Any non-whitespace |
| `^` | Start of string |
| `$` | End of string |
| `*` | 0 or more |
| `+` | 1 or more |
| `?` | 0 or 1 |
| `{n}` | Exactly n times |
| `{n,m}` | Between n and m times |
| `[abc]` | Any of a, b, or c |
| `[^abc]` | NOT a, b, or c |
| `(...)` | Capture group |
| `\|` | OR |

### 51.3 Practice Examples

```python
import re

# search — find first match
result = re.search(r'\d+', 'Phone: 123-456-7890')
print(result.group())    # 123

# findall — find all matches
numbers = re.findall(r'\d+', 'Phone: 123-456-7890')
print(numbers)    # ['123', '456', '7890']

# sub — replace
cleaned = re.sub(r'\d', '#', 'Phone: 123-456')
print(cleaned)    # Phone: ###-###

# split
parts = re.split(r'[,;]', 'apple,banana;cherry')
print(parts)    # ['apple', 'banana', 'cherry']

# match — match at the START of string
result = re.match(r'\d+', '123abc')
print(result.group())    # 123

result = re.match(r'\d+', 'abc123')
print(result)    # None (no match at start!)
```

```python
# Email validation
pattern = r'^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$'
emails = ['test@email.com', 'invalid@', 'user@site.co.uk', 'bad']
for email in emails:
    if re.match(pattern, email):
        print(f'{email} — Valid')
    else:
        print(f'{email} — Invalid')
# Output:
# test@email.com — Valid
# invalid@ — Invalid
# user@site.co.uk — Valid
# bad — Invalid
```

> **⚠️ Key Insights & Common Mistakes**
> - Always use **raw strings** `r'...'` for regex patterns to avoid escape character conflicts.
> - `match()` checks only the **beginning** of the string. `search()` checks the **entire** string.
> - `findall()` returns a list of all matches. `search()` returns only the first match.
> - Regex can be slow on large texts — compile patterns with `re.compile()` for repeated use.

---

### 📝 Assignment Questions — Chapters 51–52

1. What is the difference between `re.match()` and `re.search()`?
2. Write a regex to validate an Indian phone number (10 digits starting with 6-9).
3. Extract all email addresses from a text using regex.
4. What does `\d+` match?
5. Why should you use raw strings for regex patterns?

---

# Part XI: Object-Oriented Programming

---

## Chapter 53: Classes and Objects

### 53.1 Theory

**Object-Oriented Programming (OOP)** is a programming paradigm that organises code into **objects** — bundles of data (attributes) and behaviour (methods). OOP provides:

1. **Modularity** — easy to maintain and debug
2. **Reusability** — use variables and methods in other classes (Inheritance)
3. **Readability** and code clarity
4. **Encapsulation** — hide internal details

**Key OOP Concepts :**
1. Inheritance
2. Encapsulation
3. Polymorphism
4. Abstraction

**Terminology:**
- **Class** — Blueprint of an object that defines methods and variables
- **Object** — Real-world entity created from a class
- **Method** — Function defined inside a class
- **Attribute** — Variable that belongs to an object or class
- **`self`** — Reference to the current instance; used to access attributes and methods within the class
- **`__init__`** — Constructor method; executes automatically when an object is created

### 53.2 Syntax 

```python
class ClassName():    # PascalCase (parenthesis is optional)
    class_variable = value    # Shared by all objects

    def __init__(self, param1, param2):    # Constructor
        self.instance_var1 = param1         # Unique to each object
        self.instance_var2 = param2

    def method_name(self):    # Method (snake_case)
        # statements
        pass

# Creating objects
obj = ClassName(arg1, arg2)    # Calls __init__ automatically
obj.method_name()              # Call method
```

### 53.3 Extensive Practice Examples 

```python
# Simplest class
class MyFunc:
    print('Hello x Family !!')
# Output: Hello x Family !! (executes when class is defined!)
```

```python
# Class structure with all elements
sub1 = 'Python'                         # Global Variable
sub2 = 'ML'                             # Global Variable

class Testclass():                       # Class Name
    class_var1 = 100                     # Class Variable
    class_var2 = 200                     # Class Variable

    def __init__(self, arg1):            # INIT Method (Constructor)
        print('We are in INIT Method')
        self.stud1 = arg1                # Instance Variable
        self.city = 'Pune'               # Instance Variable

    def my_method1(self):                # Method 1
        print('We are in Method 1')
        print('Global variable:', sub1)
        print('Class Var1:', self.class_var1)
        print('Student name is:', self.stud1)

student1 = 'Rajat'

obj1 = Testclass(student1)              # Creating object → __init__ runs
obj1.my_method1()

# Output:
# We are in INIT Method
# We are in Method 1
# Global variable: Python
# Class Var1: 100
# Student name is: Rajat

obj2 = Testclass(student1)
print(obj2.city)    # Pune
# Output:
# We are in INIT Method
# Pune
```

```python
# Calculator class — progressive building
class Calculator:
    def addition(self):
        print('Addition Method')

    def multiplication(self):
        print('Multiplication Method')

    def factorial(self):
        print('Factorial Method')

    def exponent(self):
        print('Exponent Method')

CalObj = Calculator()
CalObj.addition()       # Addition Method
CalObj.exponent()       # Exponent Method
```

```python
# Calculator with __init__ and parameters
class Calculator:
    def __init__(self, a, b):
        self.num1 = a
        self.num2 = b

    def addition(self):
        result = self.num1 + self.num2
        print(f'Addition: {result}')

    def multiplication(self):
        result = self.num1 * self.num2
        print(f'Multiplication: {result}')

    def exponent(self):
        result = self.num1 ** self.num2
        print(f'Exponent: {result}')

CalObj = Calculator(5, 3)
CalObj.addition()          # Addition: 8
CalObj.multiplication()    # Multiplication: 15
CalObj.exponent()          # Exponent: 125
```

### 53.4 Class Variables vs Instance Variables

```python
class Student:
    school = 'x Academy'    # Class variable (shared)
    count = 0

    def __init__(self, name, age):
        self.name = name    # Instance variable (unique)
        self.age = age      # Instance variable (unique)
        Student.count += 1

s1 = Student('Alice', 20)
s2 = Student('Bob', 22)

print(s1.name, s1.school)    # Alice x Academy
print(s2.name, s2.school)    # Bob x Academy
print(Student.count)          # 2
```

> **⚠️ Key Insights & Common Mistakes**
> - `__init__` is the **constructor** — it runs automatically when you create an object. You don't call it directly.
> - `self` is **required** as the first parameter of every method in a class. It refers to the current instance.
> - Forgetting `self` when accessing instance variables inside methods is a very common error.
> - **Class variables** are shared by all instances. **Instance variables** are unique to each instance.
> - If you assign to a class variable through an instance (`obj.class_var = value`), it creates an **instance variable** that shadows the class variable — it does NOT change the class variable.
> - Class names use **PascalCase** (e.g., `LinearRegression`, `RandomForestClassifier`).

---

### 📝 Assignment Questions — Chapter 53

1. What is the difference between a class and an object?
2. What is `__init__` and when does it execute?
3. What is `self` and why is it required?
4. What is the difference between class variables and instance variables?
5. Create a `BankAccount` class with methods for deposit, withdraw, and balance.

---

## Chapter 54: Inheritance

### 54.1 Theory

**Inheritance** allows a class (child) to inherit properties (variables and methods) from another class (parent). This promotes code **reuse** and makes code **easier to maintain**.

**Types of Inheritance :**
1. **Single Inheritance** — One parent, one child
2. **Multilevel Inheritance** — Chain: Grandparent → Parent → Child
3. **Multiple Inheritance** — One child, multiple parents
4. **Hierarchical Inheritance** — One parent, multiple children
5. **Hybrid Inheritance** — Combination of above types

**Terminology :**

| Term 1 | Term 2 |
|--------|--------|
| Parent Class | Child Class |
| Base Class | Derived Class |
| Super Class | Sub Class |

### 54.2 Syntax

```python
class ParentClass:
    # parent methods and variables
    pass

class ChildClass(ParentClass):    # Inherits from ParentClass
    # child methods and variables
    pass
```

### 54.3 Extensive Practice Examples 

#### Single Inheritance

```python
# Without inheritance — error!
class Calculator:
    num = 7

    def addition(self):
        print('Addition Method')

    def multiplication(self):
        print('Multiplication Method')

class DisplayResult():
    def result(self):
        print('Result Method')

CalObj1 = Calculator()
# CalObj1.result()    # AttributeError: 'Calculator' object has no attribute 'result'
```

```python
# With inheritance — works!
class Calculator:
    num = 7

    def addition(self):
        print('Addition Method')

    def multiplication(self):
        print('Multiplication Method')

class DisplayResult(Calculator):    # Inherits from Calculator
    def result(self):
        print('Result Method')

obj = DisplayResult()
obj.addition()          # Addition Method (inherited!)
obj.multiplication()    # Multiplication Method (inherited!)
obj.result()            # Result Method (own method)
print(obj.num)          # 7 (inherited class variable!)
```

#### Calling Methods Within a Class

```python
class TestClass():
    def __init__(self, x, y):
        print('INIT Function')
        self.var1 = x
        self.var2 = y

    def method1(self):
        print('Method 1')
        print(self.var1)
        print(self.var2)

    def method2(self):
        self.method1()        # Calling method1 from method2
        print('Method 2')

obj = TestClass(10, 20)
obj.method2()
# Output:
# INIT Function
# Method 1
# 10
# 20
# Method 2
```

#### super() — Calling Parent Methods

```python
class Animal:
    def __init__(self, name):
        self.name = name

    def speak(self):
        print(f'{self.name} makes a sound')

class Dog(Animal):
    def __init__(self, name, breed):
        super().__init__(name)    # Call parent's __init__
        self.breed = breed

    def speak(self):
        print(f'{self.name} barks!')

d = Dog('Buddy', 'Labrador')
d.speak()    # Buddy barks!
print(d.name, d.breed)    # Buddy Labrador
```

#### Multilevel Inheritance

```python
class Grandparent:
    def method1(self):
        print('Grandparent method')

class Parent(Grandparent):
    def method2(self):
        print('Parent method')

class Child(Parent):
    def method3(self):
        print('Child method')

c = Child()
c.method1()    # Grandparent method (inherited from Grandparent!)
c.method2()    # Parent method (inherited from Parent!)
c.method3()    # Child method
```

#### Multiple Inheritance

```python
class Father:
    def skill(self):
        print('Gardening')

class Mother:
    def skill(self):
        print('Cooking')

class Child(Father, Mother):    # Inherits from BOTH
    pass

c = Child()
c.skill()    # Gardening (Father comes first — MRO!)
print(Child.__mro__)    # Method Resolution Order
```

> **⚠️ Key Insights & Common Mistakes**
> - In multiple inheritance, Python uses **MRO (Method Resolution Order)** — the order of parent classes matters! First parent listed takes priority.
> - Use `super()` to call parent class methods — don't call them directly with `ParentClass.method(self)`.
> - Check MRO with `ClassName.__mro__` or `ClassName.mro()`.
> - The **Diamond Problem** occurs when a class inherits from two classes that share a common ancestor. Python resolves this using C3 Linearisation (MRO).

---

### 📝 Assignment Questions — Chapter 54

1. What is the difference between single and multiple inheritance?
2. What is `super()` and why is it used?
3. What is MRO (Method Resolution Order)?
4. Write a `Vehicle` → `Car` → `ElectricCar` multilevel inheritance example.
5. What is the Diamond Problem? How does Python solve it?

---

## Chapter 55: Encapsulation

### 55.1 Theory

**Encapsulation** is the principle of **restricting direct access** to an object's internal data and methods from outside the class. It protects data from accidental modification.

**Access Levels :**

| Convention | Access | Example |
|------------|--------|---------|
| `name` | Public | Accessible everywhere |
| `_name` | Protected (convention) | Accessible but "don't touch" signal |
| `__name` | Private (name mangling) | Not directly accessible outside class |

### 55.2 Syntax 

```python
# Private variable: __variablename
# Private method:   __methodname

# Name Mangling (access private from outside):
# obj._ClassName__variable
# obj._ClassName__method()
```

### 55.3 Extensive Practice Examples 

```python
# Public access
class TestClass:
    location = 'Pune'

    def method1(self):
        print('Method 1')

t1 = TestClass()
print(t1.location)    # Pune (accessible)
t1.method1()           # Method 1 (accessible)
```

```python
# Protected (single underscore — convention only, NOT enforced)
class TestClass:
    _location = 'Pune'

    def method1(self):
        print('Location is:', self._location)

t1 = TestClass()
t1._location = 'Mumbai'    # Can still access! Just a convention.
t1.method1()    # Location is: Mumbai
```

```python
# Private (double underscore — name mangling enforced!)
class TestClass:
    __location = 'Pune'    # Private variable

    def method1(self):
        print('Location is:', self.__location)

t1 = TestClass()
# print(t1.__location)    # AttributeError: 'TestClass' object has no attribute '__location'

t1.__location = 'Mumbai'    # Creates a NEW attribute! Does NOT change private var.
t1.method1()                 # Location is: Pune (original private value!)
```

```python
# Name mangling — access private from outside
class TestClass:
    __location = 'Pune'

    def method1(self):
        print('Location is:', self.__location)

t1 = TestClass()
print(t1._TestClass__location)    # Pune (name mangling access!)
```

```python
# Private method
class TestClass:
    location = 'Pune'

    def __method1(self):    # Private method
        print('Method 1')

t1 = TestClass()
# t1.__method1()    # AttributeError: 'TestClass' object has no attribute '__method1'
t1._TestClass__method1()    # Method 1 (name mangling access)
```

```python
# Instance variable must be accessed after method call
class TestClass:
    location = 'Pune'

    def method1(self):
        print('Method 1')
        self.x = 115

t1 = TestClass()
# print(t1.x)    # AttributeError! x doesn't exist until method1() is called!
t1.method1()      # Method 1
print(t1.x)       # 115 (now it exists)
```

### 55.4 Property Decorator (Getters/Setters)

```python
class Temperature:
    def __init__(self, celsius):
        self._celsius = celsius

    @property
    def celsius(self):
        return self._celsius

    @celsius.setter
    def celsius(self, value):
        if value < -273.15:
            raise ValueError('Temperature below absolute zero!')
        self._celsius = value

    @property
    def fahrenheit(self):
        return self._celsius * 9/5 + 32

t = Temperature(100)
print(t.celsius)       # 100
print(t.fahrenheit)    # 212.0
t.celsius = 0
print(t.fahrenheit)    # 32.0
# t.celsius = -300     # ValueError: Temperature below absolute zero!
```

> **⚠️ Key Insights & Common Mistakes**
> - Single underscore `_var` is **convention only** — Python does NOT enforce it. It's a hint: "don't use this from outside."
> - Double underscore `__var` triggers **name mangling**: Python renames it to `_ClassName__var`. It's not truly private — just harder to access.
> - Assigning `obj.__var = value` creates a **new public attribute** — it does NOT change the private variable!
> - Instance variables created in methods only exist **after that method is called**.
> - Use `@property` for clean getter/setter syntax instead of manual `get_x()` / `set_x()` methods.

---

### 📝 Assignment Questions — Chapter 55

1. What is encapsulation? Why is it important?
2. What is the difference between `_var`, `__var`, and `var`?
3. What is name mangling? How do you access a private variable from outside?
4. What happens if you do `obj.__private = 5` from outside the class?
5. What is the `@property` decorator and when should you use it?

---

## Chapter 56: Polymorphism

### 56.1 Theory

**Polymorphism** means "many forms". It allows objects of **different classes** to be treated through the same interface. The same method name can behave differently depending on the object that calls it.

**Two types :**
1. **Method Overriding** — Child class provides its own implementation of a parent method
2. **Duck Typing** — "If it walks like a duck and quacks like a duck, it's a duck"

### 56.2 Syntax

```python
# Same method name in different classes
class Shape:
    def area(self):
        pass

class Rectangle(Shape):
    def area(self):    # Overrides parent
        return self.l * self.b

class Circle(Shape):
    def area(self):    # Different implementation
        return math.pi * self.r ** 2
```

### 56.3 Extensive Practice Examples 

```python
# Polymorphism — same function, different types
str1 = 'Python'
list1 = [2, 3, 4, 5, 6]
print(len(str1))    # 6
print(len(list1))   # 5
# len() works on different types — that's polymorphism!

print(5 + 9)        # 14 (integer addition)
print('Hey' + 'Siri')  # HeySiri (string concatenation)
# + operator behaves differently for different types!
```

```python
# Polymorphism with classes 
class Rectangle():
    def area(self):
        print('Area function of Rectangle')

class Circle():
    def area(self):
        print('Area function of Circle')

class Square():
    def area(self):
        print('Area function of Square')

r1 = Rectangle()
c1 = Circle()
s1 = Square()

# Same method name, different behaviour
for obj in [r1, c1, s1]:
    obj.area()
# Output:
# Area function of Rectangle
# Area function of Circle
# Area function of Square
```

```python
# With calculations 
import math

class Rectangle():
    def __init__(self, l, b):
        self.l = l
        self.b = b

    def area(self):
        ar = self.l * self.b
        print('Area of Rectangle is:', ar)

class Circle():
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        ar = math.pi * self.radius**2
        print('Area of Circle is:', ar)

class Square():
    def __init__(self, side):
        self.side = side

    def area(self):
        ar = self.side ** 2
        print('Area of Square is:', ar)

r1 = Rectangle(8, 15)
c1 = Circle(5)
s1 = Square(7)

for obj in [r1, c1, s1]:
    obj.area()
# Output:
# Area of Rectangle is: 120
# Area of Circle is: 78.53981633974483
# Area of Square is: 49
```

```python
# Method Overriding — child overrides parent
class Animal:
    def speak(self):
        print('Animal speaks')

class Dog(Animal):
    def speak(self):    # Overrides parent's speak()
        print('Dog barks!')

class Cat(Animal):
    def speak(self):    # Overrides parent's speak()
        print('Cat meows!')

animals = [Dog(), Cat(), Animal()]
for animal in animals:
    animal.speak()
# Output:
# Dog barks!
# Cat meows!
# Animal speaks
```

> **⚠️ Key Insights & Common Mistakes**
> - Python doesn't have **method overloading** (same name, different parameters). Use default arguments or `*args` instead.
> - Python does have **method overriding** (child replaces parent's method).
> - In the loop `for obj in [r1, c1, s1]: obj.area()`, Python calls the **correct `area()` method** for each object automatically — this is polymorphism!
> - Python uses **duck typing**: it doesn't check the type, just whether the object has the required method.

---

### 📝 Assignment Questions — Chapter 56

1. What is polymorphism? Give a real-world example.
2. What is method overriding?
3. Does Python support method overloading? How do you achieve similar behaviour?
4. Write code demonstrating polymorphism with a `Shape` hierarchy.
5. What is duck typing?

---

## Chapters 57–61: Abstraction, Class/Static Methods, Magic Methods

### 57: Abstraction

```python
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def area(self):
        pass

    @abstractmethod
    def perimeter(self):
        pass

# shape = Shape()    # TypeError: Can't instantiate abstract class!

class Rectangle(Shape):
    def __init__(self, l, b):
        self.l = l
        self.b = b

    def area(self):
        return self.l * self.b

    def perimeter(self):
        return 2 * (self.l + self.b)

r = Rectangle(5, 3)
print(r.area())         # 15
print(r.perimeter())    # 16
```

### 58–60: Class Methods, Static Methods, Property

```python
class Employee:
    company = 'TechCorp'
    count = 0

    def __init__(self, name, salary):
        self.name = name
        self.salary = salary
        Employee.count += 1

    def display(self):              # Instance method
        print(f'{self.name}: {self.salary}')

    @classmethod                    # Class method
    def get_company(cls):
        return cls.company

    @classmethod
    def from_string(cls, emp_str):    # Alternative constructor
        name, salary = emp_str.split('-')
        return cls(name, int(salary))

    @staticmethod                   # Static method
    def is_valid_salary(salary):
        return salary > 0

print(Employee.get_company())             # TechCorp
emp = Employee.from_string('Alice-50000')
emp.display()                              # Alice: 50000
print(Employee.is_valid_salary(50000))    # True
```

| Method Type | First Parameter | Access |
|-------------|----------------|--------|
| Instance method | `self` | Instance + class variables |
| Class method `@classmethod` | `cls` | Class variables only |
| Static method `@staticmethod` | None | No access to class/instance |

### 61: Magic (Dunder) Methods

```python
class Vector:
    def __init__(self, x, y):
        self.x = x
        self.y = y

    def __repr__(self):
        return f'Vector({self.x}, {self.y})'

    def __add__(self, other):
        return Vector(self.x + other.x, self.y + other.y)

    def __len__(self):
        return int((self.x**2 + self.y**2)**0.5)

    def __eq__(self, other):
        return self.x == other.x and self.y == other.y

v1 = Vector(3, 4)
v2 = Vector(1, 2)
v3 = v1 + v2
print(v3)          # Vector(4, 6)
print(len(v1))     # 5
print(v1 == v2)    # False
```

**Common Magic Methods:**

| Method | Triggered By |
|--------|-------------|
| `__init__` | `obj = Class()` |
| `__str__` | `print(obj)`, `str(obj)` |
| `__repr__` | `repr(obj)`, interpreter display |
| `__add__` | `obj1 + obj2` |
| `__len__` | `len(obj)` |
| `__eq__` | `obj1 == obj2` |
| `__lt__` | `obj1 < obj2` |
| `__getitem__` | `obj[key]` |
| `__iter__` | `for x in obj` |
| `__contains__` | `x in obj` |

> **⚠️ Key Insights & Common Mistakes**
> - **Abstract classes** cannot be instantiated. They force subclasses to implement required methods.
> - `@classmethod` receives the **class** as first arg (`cls`). `@staticmethod` receives **nothing**.
> - Use `@classmethod` for **alternative constructors** (e.g., `from_string`, `from_dict`).
> - `__str__` is for human-readable output. `__repr__` is for debugging (should be unambiguous).
> - `__repr__` should ideally return a string that could recreate the object.

---

### 📝 Assignment Questions — Chapters 57–61

1. What is an abstract class? Why can't you instantiate it?
2. What is the difference between `@classmethod` and `@staticmethod`?
3. What is the difference between `__str__` and `__repr__`?
4. Implement `__add__` and `__eq__` for a `Money` class.
5. Write an abstract class `Database` with abstract methods `connect()` and `query()`.

---

# Part XII: Advanced Python

---

## Chapter 62: Iterators

### 62.1 Theory

An **iterator** is an object that implements `__iter__()` and `__next__()` methods. It produces values one at a time, on demand.

### 62.2 Practice Examples 

```python
# All iterables can produce iterators
my_list = [1, 2, 3]
my_iter = iter(my_list)    # Create iterator

print(next(my_iter))    # 1
print(next(my_iter))    # 2
print(next(my_iter))    # 3
# print(next(my_iter))  # StopIteration!
```

```python
# Custom iterator
class CountDown:
    def __init__(self, start):
        self.start = start

    def __iter__(self):
        return self

    def __next__(self):
        if self.start <= 0:
            raise StopIteration
        self.start -= 1
        return self.start + 1

for num in CountDown(5):
    print(num, end=' ')    # 5 4 3 2 1
```

> **⚠️ Key Insights & Common Mistakes**
> - An iterator can only be consumed **once**. After `StopIteration`, you need a new iterator.
> - All iterables (list, tuple, string, dict) are NOT iterators themselves — `iter()` creates an iterator from them.

---

## Chapter 63: Generators

### 63.1 Theory

A **generator** is a special function that uses `yield` instead of `return`. It produces values **lazily** (one at a time), making it memory-efficient for large datasets.

### 63.2 Practice Examples 

```python
def count_up(n):
    i = 1
    while i <= n:
        yield i
        i += 1

for num in count_up(5):
    print(num, end=' ')    # 1 2 3 4 5
```

```python
# Generator expression
squares = (x**2 for x in range(1000000))
print(sum(squares))    # Memory efficient!
```

```python
# Fibonacci generator
def fibonacci():
    a, b = 0, 1
    while True:
        yield a
        a, b = b, a + b

fib = fibonacci()
for _ in range(10):
    print(next(fib), end=' ')    # 0 1 1 2 3 5 8 13 21 34
```

> **⚠️ Key Insights & Common Mistakes**
> - `yield` **pauses** the function and remembers its state. `return` **exits** the function permanently.
> - Generators can only be iterated **once**. After exhaustion, they produce nothing.
> - Use generators for large datasets that don't fit in memory (e.g., reading large CSV files line by line).

---

## Chapter 64: Decorators

### 64.1 Theory

A **decorator** is a function that takes another function as input and extends its behaviour **without modifying** the original function. Decorators are widely used in web frameworks (Flask, Django) and for logging, timing, authentication, etc.

### 64.2 Syntax

```python
def decorator_name(func):
    def wrapper(*args, **kwargs):
        # Before
        result = func(*args, **kwargs)
        # After
        return result
    return wrapper

@decorator_name
def my_function():
    pass
```

### 64.3 Practice Examples 

```python
# Timer decorator
import time

def timer(func):
    def wrapper(*args, **kwargs):
        start = time.time()
        result = func(*args, **kwargs)
        end = time.time()
        print(f'{func.__name__} took {end - start:.4f} seconds')
        return result
    return wrapper

@timer
def slow_function():
    time.sleep(1)
    print('Done!')

slow_function()
# Output:
# Done!
# slow_function took 1.00xx seconds
```

```python
# Logging decorator
def logger(func):
    def wrapper(*args, **kwargs):
        print(f'Calling {func.__name__} with args={args}, kwargs={kwargs}')
        result = func(*args, **kwargs)
        print(f'{func.__name__} returned {result}')
        return result
    return wrapper

@logger
def add(a, b):
    return a + b

add(3, 5)
# Calling add with args=(3, 5), kwargs={}
# add returned 8
```

> **⚠️ Key Insights & Common Mistakes**
> - `@decorator` is syntactic sugar for `func = decorator(func)`.
> - Always use `*args, **kwargs` in the wrapper to handle any arguments.
> - Use `functools.wraps(func)` to preserve the original function's name and docstring.

---

### 📝 Assignment Questions — Chapters 62–64

1. What is the difference between an iterable and an iterator?
2. What is `yield` and how is it different from `return`?
3. Why are generators memory-efficient?
4. Write a decorator that prints "Before" and "After" around any function call.
5. What does `@functools.wraps` do?

---

## Chapters 65–69: Type Hints, Context Managers, Threading, Web Scraping

### 65: Type Hints

```python
def greet(name: str) -> str:
    return f'Hello, {name}!'

def average(numbers: list[float]) -> float:
    return sum(numbers) / len(numbers)

from typing import Optional, Union

def find_user(user_id: int) -> Optional[dict]:
    # Returns dict or None
    pass

def process(data: Union[str, list]) -> None:
    pass
```

### 66: Context Managers (Advanced)

```python
from contextlib import contextmanager

@contextmanager
def timer():
    import time
    start = time.time()
    yield
    end = time.time()
    print(f'Elapsed: {end - start:.4f}s')

with timer():
    sum(range(1000000))
```

### 67: Threading and Multiprocessing

```python
import threading

def task(name):
    print(f'Task {name} running')

threads = []
for i in range(5):
    t = threading.Thread(target=task, args=(i,))
    threads.append(t)
    t.start()

for t in threads:
    t.join()
```

### 68–69: Web Scraping and APIs

```python
import requests

# API call
response = requests.get('https://api.github.com')
print(response.status_code)    # 200
data = response.json()

# Beautiful Soup for HTML parsing
from bs4 import BeautifulSoup
html = '<html><body><h1>Title</h1></body></html>'
soup = BeautifulSoup(html, 'html.parser')
print(soup.h1.text)    # Title
```

> **⚠️ Key Insights & Common Mistakes**
> - Type hints are **optional** and not enforced at runtime — use `mypy` for static checking.
> - Use **threading** for I/O-bound tasks. Use **multiprocessing** for CPU-bound tasks (due to the GIL).
> - Always check `response.status_code` before using API response data.

---

### 📝 Assignment Questions — Chapters 65–69

1. What are type hints? Are they enforced at runtime?
2. What is the GIL? Why does it matter for threading?
3. Write a context manager that logs entry and exit.
4. What is the difference between `requests.get()` and `requests.post()`?
5. How do you parse HTML content using BeautifulSoup?

---

# Part XIII: Python for Data Science — A Bridge

---

## Chapters 70–72: NumPy, Pandas, Matplotlib

### 70: NumPy

```python
import numpy as np

# Creating arrays
arr = np.array([1, 2, 3, 4, 5])
print(arr, type(arr))    # [1 2 3 4 5] <class 'numpy.ndarray'>

# Array operations (vectorised — no loops!)
print(arr * 2)        # [ 2  4  6  8 10]
print(arr ** 2)       # [ 1  4  9 16 25]
print(np.mean(arr))   # 3.0
print(np.std(arr))    # 1.4142...

# 2D array
matrix = np.array([[1, 2, 3], [4, 5, 6]])
print(matrix.shape)    # (2, 3)
print(matrix[0, 1])    # 2

# Useful functions
print(np.zeros((3, 3)))       # 3x3 matrix of zeros
print(np.ones((2, 4)))        # 2x4 matrix of ones
print(np.arange(0, 10, 2))    # [0 2 4 6 8]
print(np.linspace(0, 1, 5))   # [0.   0.25 0.5  0.75 1.  ]
```

### 71: Pandas

```python
import pandas as pd

# Series
s = pd.Series([10, 20, 30], index=['a', 'b', 'c'])
print(s['b'])    # 20

# DataFrame
data = {
    'Name': ['Alice', 'Bob', 'Charlie'],
    'Age': [25, 30, 35],
    'Salary': [50000, 60000, 70000]
}
df = pd.DataFrame(data)
print(df)
#       Name  Age  Salary
# 0    Alice   25   50000
# 1      Bob   30   60000
# 2  Charlie   35   70000

# Basic operations
print(df.describe())          # Statistical summary
print(df['Age'].mean())       # 30.0
print(df[df['Age'] > 25])     # Filter rows
df['Tax'] = df['Salary'] * 0.2    # Add column
```

### 72: Matplotlib

```python
import matplotlib.pyplot as plt

# Line plot
x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]
plt.plot(x, y, marker='o')
plt.xlabel('X Axis')
plt.ylabel('Y Axis')
plt.title('Line Plot')
plt.show()

# Bar chart
categories = ['A', 'B', 'C']
values = [25, 40, 30]
plt.bar(categories, values, color=['red', 'green', 'blue'])
plt.title('Bar Chart')
plt.show()
```

> **⚠️ Key Insights & Common Mistakes**
> - NumPy operations are **vectorised** — no need for loops. `arr * 2` multiplies every element.
> - In Pandas, use `&` and `|` for boolean operations, NOT `and`/`or`.
> - `df[df['col'] > value]` is the standard filtering syntax. Don't forget the outer `df[...]`.
> - Always call `plt.show()` to display plots (in scripts; not needed in Jupyter).

---

### 📝 Assignment Questions — Chapters 70–72

1. What is the advantage of NumPy arrays over Python lists?
2. What is the difference between a Pandas Series and DataFrame?
3. How do you filter rows in a DataFrame where age > 25?
4. Create a bar chart comparing sales of 4 products.
5. What does `df.describe()` show?

---

# Part XIV: Professional Python

---

## Chapter 73: Testing — unittest and pytest

### 73.1 Theory

**Testing** ensures your code works correctly and continues to work after changes. Python provides `unittest` (built-in) and `pytest` (third-party, more popular).

### 73.2 Practice Examples

```python
# Using unittest
import unittest

def add(a, b):
    return a + b

class TestAdd(unittest.TestCase):
    def test_positive(self):
        self.assertEqual(add(2, 3), 5)

    def test_negative(self):
        self.assertEqual(add(-1, -1), -2)

    def test_zero(self):
        self.assertEqual(add(0, 0), 0)

# Run: python -m unittest test_file.py
```

```python
# Using pytest (simpler syntax)
def add(a, b):
    return a + b

def test_add_positive():
    assert add(2, 3) == 5

def test_add_negative():
    assert add(-1, -1) == -2

# Run: pytest test_file.py
```

> **⚠️ Key Insights & Common Mistakes**
> - `pytest` is more Pythonic and simpler than `unittest`. Use `pytest` for new projects.
> - Test files should start with `test_` and test functions should start with `test_`.
> - Write tests for **edge cases**: empty inputs, None values, negative numbers, very large inputs.

---

## Chapter 74: Coding Best Practices and The Zen of Python

### 74.1 The Zen of Python

```python
import this
# Beautiful is better than ugly.
# Explicit is better than implicit.
# Simple is better than complex.
# Readability counts.
# Errors should never pass silently.
# In the face of ambiguity, refuse the temptation to guess.
```

### 74.2 Best Practices Checklist

| Practice | Do ✓ | Don't ✗ |
|----------|------|---------|
| Naming | `snake_case` for functions/variables | `camelCase` for functions |
| Naming | `PascalCase` for classes | `lowercase` for classes |
| Constants | `UPPER_CASE` | `lowercase` |
| Imports | One per line, at top of file | `from x import *` |
| Exceptions | Catch specific exceptions | Bare `except:` |
| Strings | Use f-strings | String concatenation with `+` in loops |
| Lists | Use list comprehensions | Verbose for-loop for simple transforms |
| Files | Use `with` statement | Manual `open()`/`close()` |
| Testing | Write tests for all functions | No tests at all |
| Documentation | Write docstrings | No documentation |

---

## Chapter 75: Python Certification Preparation

### 75.1 Certification Roadmap

| Level | Certification | Topics |
|-------|--------------|--------|
| Entry | **PCEP** (Certified Entry-Level) | Syntax, data types, operators, control flow, functions |
| Associate | **PCAP** (Certified Associate) | OOP, modules, exceptions, file handling |
| Professional | **PCPP1** (Certified Professional) | Advanced OOP, design patterns, networking |

### 75.2 Sample Exam Questions

**1.** What is the output?
```python
x = [1, 2, 3]
y = x
y.append(4)
print(x)
```
**Answer:** `[1, 2, 3, 4]` — `y = x` creates a reference, not a copy!

**2.** What is the output?
```python
print(type(1/1))
```
**Answer:** `<class 'float'>` — division always returns float.

**3.** What is the output?
```python
print(bool(''), bool(' '), bool(0), bool([]))
```
**Answer:** `False True False False` — empty string is falsy, space string is truthy!

**4.** What is the output?
```python
def f(x=[]):
    x.append(1)
    return x

print(f())
print(f())
print(f())
```
**Answer:** `[1]`, `[1, 1]`, `[1, 1, 1]` — mutable default argument trap!

**5.** What is the output?
```python
for i in range(5):
    pass
print(i)
```
**Answer:** `4` — the loop variable persists after the loop ends!

---

### 📝 Final Assignment Questions — Chapter 75

1. What is the output of `round(2.5)` and why?
2. What is the output of `'abc' < 'abd'`?
3. Explain the mutable default argument trap.
4. What is the difference between `is` and `==`?
5. What does `LEGB` stand for in Python scope resolution?

---

# Appendices

---

## Appendix A: Python Keywords (35 keywords)

```
False    True     None     and      or       not
if       elif     else     for      while    break
continue pass     return   def      class    import
from     as       try      except   finally  raise
with     yield    lambda   global   nonlocal del
in       is       assert   async    await
```

## Appendix B: Built-in Functions Quick Reference

```python
# Type functions
int(), float(), str(), bool(), list(), tuple(), set(), dict(), type()

# Math functions
abs(), round(), pow(), divmod(), min(), max(), sum()

# Sequence functions
len(), sorted(), reversed(), enumerate(), zip(), range()

# Boolean functions
any(), all(), isinstance(), issubclass()

# I/O
print(), input(), open()

# Conversion
bin(), oct(), hex(), ord(), chr()
```

## Appendix C: Operator Precedence (Highest to Lowest)

```
1.  ()          Parentheses
2.  **          Exponentiation
3.  +x, -x, ~x Unary operators
4.  *, /, //, % Multiplication, division
5.  +, -        Addition, subtraction
6.  <<, >>      Bitwise shifts
7.  &           Bitwise AND
8.  ^           Bitwise XOR
9.  |           Bitwise OR
10. ==, !=, <, >, >=, <=, is, in   Comparisons
11. not         Logical NOT
12. and         Logical AND
13. or          Logical OR
```

## Appendix D: Common Exceptions

| Exception | Cause |
|-----------|-------|
| `SyntaxError` | Invalid syntax |
| `IndentationError` | Wrong indentation |
| `NameError` | Undefined variable |
| `TypeError` | Wrong type |
| `ValueError` | Wrong value |
| `IndexError` | Index out of range |
| `KeyError` | Dict key not found |
| `AttributeError` | No such attribute |
| `ZeroDivisionError` | Division by zero |
| `FileNotFoundError` | File not found |
| `ImportError` | Module not found |
| `StopIteration` | Iterator exhausted |
| `RecursionError` | Max recursion depth |
| `UnboundLocalError` | Local variable referenced before assignment |

## Appendix E: Glossary

| Term | Definition |
|------|-----------|
| **API** | Application Programming Interface — a way for programs to communicate |
| **Class** | Blueprint for creating objects |
| **Constructor** | `__init__` method that initialises objects |
| **Decorator** | Function that modifies another function's behaviour |
| **DRY** | Don't Repeat Yourself — avoid code duplication |
| **Duck Typing** | If it looks and acts like a duck, treat it as a duck |
| **GIL** | Global Interpreter Lock — prevents true multi-threading for CPU-bound tasks |
| **IDE** | Integrated Development Environment (PyCharm, VS Code, Jupyter) |
| **Immutable** | Cannot be changed after creation (str, tuple, frozenset) |
| **Iterator** | Object that produces values one at a time |
| **Generator** | Function using `yield` to produce values lazily |
| **Lambda** | Anonymous one-line function |
| **Mutable** | Can be changed after creation (list, dict, set) |
| **OOP** | Object-Oriented Programming |
| **PEP 8** | Python Enhancement Proposal 8 — style guide |
| **REPL** | Read-Eval-Print Loop — interactive Python shell |
| **Scope** | Region where a variable is accessible |
| **Self** | Reference to current instance in a class |
| **Virtualenv** | Isolated Python environment for project dependencies |

---

**End of Book**

*Python: The Definitive Guide — From Zero to Data Science and AI*
*Edition V.0 | 75 Chapters | 14 Parts | 5 Appendices*

---
