# Python Data Structures

Python offers various data structures to work with. Here, you will learn about some essential data structures, including Tuples, Lists, Dictionaries, built-in functions, and methods associated with them.

## Tuples

A tuple is a collection of ordered, immutable elements enclosed in round brackets. You cannot modify the values in a tuple.

### Example

```python
my_tuple = ("apple", "orange", "banana")
print(my_tuple[1])  # Output: orange
```

### Tuple methods:

* `len(tuple)`: Returns the number of elements in the tuple.
* `tuple.count(element)`: Counts the occurrences of an element in the tuple.
* `tuple.index(element)`: Finds the index of the first occurrence of an element in the tuple.

## Lists

A list is an ordered, mutable collection of elements enclosed in square brackets. Lists can have mixed data types.

### Example

```python
my_list = [42, "apple", 3.14, True]
print(my_list[2])  # Output: 3.14
```

### List methods:

* `len(list)`: Returns the number of elements in the list.
* `list.append(element)`: Adds an element to the end of the list.
* `list.insert(index, element)`: Inserts an element at the specified index of the list.
* `list.remove(element)`: Removes the first occurrence of an element in the list.
* `list.pop()`: Removes and returns the last element of the list.
* `list.clear()`: Removes all elements from the list.
* `list.count(element)`: Counts the occurrences of an element in the list.
* `list.index(element)`: Finds the index of the first occurrence of an element in the list.
* `list.reverse()`: Reverses the order of elements in the list.
* `list.sort()`: Sorts the elements of the list in ascending order.

## Dictionaries

A dictionary is an unordered, mutable data structure that contains key-value pairs. Keys must be unique, and values can be of any data type. Dictionaries are enclosed in curly brackets.

### Example

```python
my_dict = {
    "name": "Alice",
    "age": 30,
    "city": "New York"
}
print(my_dict["age"])  # Output: 30
```

### Dictionary methods:

* `len(dict)`: Returns the number of key-value pairs in the dictionary.
* `dict.get(key[, default])`: Returns the value associated with the key or the default value (if provided) if the key is not present.
* `dict.keys()`: Returns a view object that displays a list of all the dictionary's keys.
* `dict.values()`: Returns a view object that displays a list of all the dictionary's values.
* `dict.items()`: Returns a view object that displays a list of all the dictionary's key-value pairs.
* `dict.update(another_dict)`: Merges two dictionaries, and the second dictionary's values overwrite the first dictionary's values if there are matching keys.
* `dict.pop(key)`: Removes the key-value pair with the specified key and returns the corresponding value.
* `dict.clear()`: Removes all key-value pairs from the dictionary.

## Built-in functions (useful for all data structures)

* `len(data_structure)`: Returns the number of elements/items in the data structure (tuple, list, or dictionary).
* `sorted(data_structure)`: Returns a new list containing all elements of the given data structure, sorted in ascending order.
* `min(data_structure)`: Returns the smallest element in the data structure.
* `max(data_structure)`: Returns the largest element in the data structure.
* `del data_structure[index]`: Deletes an element from the data structure at the given index.
* `data_structure_1 + data_structure_2`: Concatenates two data structures (tuples or lists) into a single one.
