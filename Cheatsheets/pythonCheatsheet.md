# Python Cheatsheet for Beginners

A beginner-friendly Python cheatsheet with examples that cover basic concepts, such as data types, operators, control structures, functions, and more.

## Variables

Variables are used to store values in Python. Variable names should be descriptive and follow the [PEP8 naming conventions](https://www.python.org/dev/peps/pep-0008/#naming-conventions).

```python
name = "John"
age = 25
```

## Data types

Python has several built-in data types:

### Numbers

* **Integers**: Whole numbers, positive or negative.

  ```python
  a = 42
  b = -7
  ```

* **Floats**: Real numbers, decimal points allowed.

  ```python
  c = 3.14
  d = -0.5
  ```

### Strings

A sequence of characters enclosed in quotes.

```python
greeting = "Hello, World!"
```

### Booleans

True or False values.

```python
is_true = True
is_false = False
```

## Operators

### Arithmetic operators

* `+` (Addition)
* `-` (Subtraction)
* `*` (Multiplication)
* `/` (Division)
* `**` (Exponentiation)
* `//` (Floor division)
* `%` (Modulus)

### Comparison operators

* `==` (Equal to)
* `!=` (Not equal to)
* `>` (Greater than)
* `<` (Less than)
* `>=` (Greater than or equal to)
* `<=` (Less than or equal to)

### Logical operators

* `and` (Logical AND)
* `or` (Logical OR)
* `not` (Logical NOT)

## Control Structures

### If-else statement

Conditional execution of code blocks based on boolean expressions.

```python
if age >= 18:
    print("You are an adult")
else:
    print("You are not an adult")
```

### While loop

Repeatedly execute a block of code as long as a condition is true.

```python
count = 1
while count <= 5:
    print(count)
    count += 1
```

### For loop

Iterate over a sequence (like a list or a range).

```python
for i in range(1, 6):
    print(i)
```

## Functions

A block of reusable code that performs a specific task.

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")
```

## Lists

An ordered, mutable collection of elements enclosed in square brackets.

```python
fruits = ["apple", "banana", "orange"]
```

## Tuples

An ordered, immutable collection of elements enclosed in round brackets.

```python
coordinates = (4, 5)
```

## Dictionaries

An unordered, mutable collection of key-value pairs enclosed in curly brackets.

```python
person = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}

