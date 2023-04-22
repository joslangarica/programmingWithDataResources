# Intermediate Python Cheatsheet for Beginners

An easy-to-understand Python cheatsheet covering intermediate concepts for beginners, including comprehensions, file handling, error handling, modules and packages, and object-oriented programming.

## Comprehensions

### List comprehension

A quick way to create a new list by applying a formula to each item in another list (or iterable).

```python
# Original list
numbers = [1, 2, 3, 4, 5]

# Formula: square each number
# Result: A new list of squared numbers
squares = [x ** 2 for x in numbers]
```

### Dictionary comprehension

A fast method for creating a new dictionary by applying a formula to each item in a list (or iterable).

```python
# Original list
names = ["Alice", "Bob", "Charlie"]

# Formula: Get the length of each name
# Result: A new dictionary with names as keys and lengths as values
name_lengths = {name: len(name) for name in names}
```

## Handling files

### Reading from a file

```python
# Open the file in read mode ('r') and give it the name 'file'
with open("file.txt", "r") as file:
    # Read the content of the file
    contents = file.read()
```

### Writing to a file

```python
# Open the file in write mode ('w') and give it the name 'file'
with open("file.txt", "w") as file:
    # Write a string to the file
    file.write("Hello, World!")
```

## Error handling

### Try-except block

Catch and handle mistakes (errors) while running certain code.

```python
try:
    # Try to convert user input to an integer
    number = int(input("Enter a number: "))
except ValueError:
    # If it doesn't work, print a message
    print("That's not a valid number.")
```

### Raising exceptions

Create a custom error message with the `raise` keyword.

```python
def divide(a, b):
    # If b is 0, create an error message
    if b == 0:
        raise ValueError("Division by zero is not allowed")
    # Otherwise, return a divided by b
    return a / b
```

## Modules and packages

### Importing a module

Use the `import` keyword to use functions from a module.

```python
# Import the 'math' module
import math

# Use the 'sqrt' function from 'math' to find the square root of 9
sqrt = math.sqrt(9)
```

### Importing specific functions

Use the `from ... import ...` syntax to import only certain functions from a module.

```python
# Import the 'sqrt' function from the 'math' module
from math import sqrt

# Use the 'sqrt' function directly (no need for 'math.sqrt')
result = sqrt(9)
```

### Creating a package

Organize related modules in one folder (the package) and add an `__init__.py` file.

```
my_package/
  __init__.py
  module1.py
  module2.py
```

## Object-oriented programming (OOP)

### Defining a class

```python
# Create a 'Dog' class
class Dog:
    # The class constructor (called when a new Dog is created)
    def __init__(self, name, age):
        self.name = name
        self.age = age

    # A method for the Dog class (all Dogs can use this)
    def bark(self):
        print("Woof!")
```

### Creating an object (instance)

```python
# Create a new Dog with the name "Buddy" and age 3
my_dog = Dog("Buddy", 3)
```

### Accessing attributes and methods

```python
# Print the 'name' attribute of 'my_dog'
print(my_dog.name)

# Call the 'bark' method of 'my_dog'
my_dog.bark()
```

### Inheritance

```python
# Create a class 'Labrador' that inherits from the 'Dog' class
class Labrador(Dog):
    # The class constructor (called when a new Labrador is created)
    def __init__(self, name, age, color):
        # Call the parent class constructor
        super().__init__(name, age)
        self.color = color

    # A new method, specific to the Labrador class
    def fetch(self):
        print("I fetched the ball!")

# Create a new Labrador with the name "Rex", age 2, and color "yellow"
my_labrador = Labrador("Rex", 2, "yellow")
```

!