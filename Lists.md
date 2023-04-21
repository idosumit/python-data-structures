# Lists

## Quick look at the main funtionalities

Lists in Python are used to store multiple items in a single variable. They are ordered, mutable (modifiable), and allow duplicate items. To create a list, we can use square brackets `[]` and separate the elements with commas.

| Functionality              | Description                                  | Example (Easy)                  | Example (Medium)                 | Example (Sophisticated)          |
|-----------------------------|----------------------------------------------|---------------------------------|----------------------------------|----------------------------------|
| Initializing                | Creating a new list                          | `my_list = [1, 2, 3]`           | `my_list = ['apple', 'banana']`  | `my_list = [1, 'apple', [1, 2]]` |
| Indexing                    | Accessing elements by position               | `print(my_list[0])`             | `print(my_list[-1])`             | `print(my_list[2][1])`           |
| Length                      | Determining the number of elements           | `print(len(my_list))`           | `print(len(my_list))`            | `print(len(my_list))`            |
| Modifying                   | Changing the value of an element             | `my_list[1] = 4`                | `my_list[1] = 'orange'`          | `my_list[2][1] = 3`              |
| Adding                      | Inserting new elements                       | `my_list.append(4)`             | `my_list.extend(['cherry'])`     | `my_list.insert(1, 'kiwi')`      |
| Removing                    | Deleting elements                            | `my_list.remove(1)`             | `my_list.pop()`                  | `del my_list[1]`                 |
| Counting                    | Counting occurrences of an element           | `print(my_list.count(2))`       | `print(my_list.count('apple'))`  | `print(my_list.count([1, 2]))`   |
| Slicing                     | Extracting a portion of a list               | `print(my_list[1:3])`           | `print(my_list[2:])`             | `print(my_list[:-1])`            |
| Concatenation               | Combining two lists                          | `print(my_list + [4, 5, 6])`    | `print(my_list + ['cherry'])`    | `print(my_list + [1, 'apple'])`  |
| Repetition                  | Creating a new list by repeating elements    | `print(my_list * 2)`            | `print(my_list * 3)`             | `print(my_list * 4)`             |
| Membership                  | Checking if an element is in the list        | `print(1 in my_list)`           | `print('apple' in my_list)`      | `print([1, 2] in my_list)`       |
| Iterating                   | Looping through elements                     | `for x in my_list: print(x)`    | `for i, x in enumerate(my_list): print(i, x)` | `for x in my_list[::-1]: print(x)` |
| Sorting                     | Arranging elements in a specific order       | `my_list.sort()`                | `my_list.sort(reverse=True)`     | `print(sorted(my_list))`         |
| Reversing                   | Reversing the order of elements             | `my_list.reverse()`             | `print(my_list[::-1])`           | `print(list(reversed(my_list)))` |
| Copying                     | Creating a new list with the same elements   | `my_list_copy = my_list.copy()` | `my_list_copy = my_list[:]`      | `my_list_copy = list(my_list)`   |
