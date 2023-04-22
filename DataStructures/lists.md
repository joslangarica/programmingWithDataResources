# Python Lists for Beginners

A comprehensive guide on Python lists for beginners

## What are Lists?

Lists in Python are ordered collections of items that can store different types of data, such as strings, integers, or objects. Lists are mutable, meaning you can add, delete, or modify elements in them.

### Creating a List

A list is created by placing items inside square brackets `[ ]` and separating them with commas.

```python
# Empty list
empty_list = []

# List with various data types (string, integer, float)
mixed_list = ["apple", 3, 8.5]
```

## Accessing Items in a List

Items in a list can be accessed using the item's index, which is an integer value representing the position of the item in the list.

```python
# A list of fruits
fruits = ["apple", "orange", "banana", "grape"]

# Access the first item (index 0)
first_item = fruits[0]   # "apple"

# Access the last item using negative index
last_item = fruits[-1]   # "grape"
```

## Modifying Items in a List

You can change an item in a list by assigning a new value to its index.

```python
# A list of numbers
numbers = [1, 2, 3, 4]

# Change the second item (index 1) to 8
numbers[1] = 8   # [1, 8, 3, 4]
```

## Adding Items to a List

You can add items to the end of a list or at a specified index using the `append()` and `insert()` methods, respectively.

```python
# Start with an empty list
planets = []

# Add "Earth" to the end of the list
planets.append("Earth")   # ["Earth"]

# Add "Mars" at index 1
planets.insert(1, "Mars")   # ["Earth", "Mars"]
```

## Removing Items from a List

To remove an item from a list, you can use the `remove()` method, which removes the first occurrence of the specified item. Alternatively, use the `pop()` method to remove the item at a specified index (or the last item by default).

```python
animals = ["cat", "dog", "elephant", "lion"]

# Remove the "dog" from the list
animals.remove("dog")   # ["cat", "elephant", "lion"]

# Remove the item at index 0
first_animal = animals.pop(0)   # "cat" (animals: ["elephant", "lion"])

# Remove the last item
last_animal = animals.pop()   # "lion" (animals: ["elephant"])
```

## Sorting Items in a List

The `sort()` method allows you to sort a list in ascending order. To sort a list in descending order, use the `reverse=True` argument.

```python
grades = [85, 67, 99, 74]

# Sort the grades in ascending order
grades.sort()   # [67, 74, 85, 99]

# Sort the grades in descending order
grades.sort(reverse=True)   # [99, 85, 74, 67]
```

## Built-in List Functions

Python provides several built-in functions to work with lists, such as `len()`, `min()`, `max()`, and `sum()`.

```python
temperatures = [72, 65, 78, 61]

# Find the number of items in the list
length = len(temperatures)   # 4

# Find the minimum value in the list
min_temp = min(temperatures)   # 61

# Find the maximum value in the list
max_temp = max(temperatures)   # 78

# Calculate the sum of the list items
total_temp = sum(temperatures)   # 276
```

## List Methods

Some commonly used list methods are:

* `append(item)`: Add `item` to the end of the list.
* `insert(index, item)`: Insert `item` at `index`.
* `remove(item)`: Remove the first occurrence of `item`.
* `pop(index)`: Remove and return the item at `index` (or the last item if no index is specified).
* `sort()`: Sort the list items in ascending order.
* `reverse()`: Reverse the list items.
* `extend(iterable)`: Add all items of `iterable` to the end of the list.

```python
shopping_list = ["eggs", "milk", "bread"]

# Add "butter" to the list
shopping_list.append("butter")

# Reverse the items in the list
shopping_list.reverse()

# Combine two lists
vegetables = ["carrot", "broccoli", "pepper"]
shopping_list.extend(vegetables)
```

