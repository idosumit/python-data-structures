# Tuples

## Quick look at the main funtionalities

In this table, we will compare and contrast the functionalities of Tuple: an ordered, immutable collection of values that can be of any data type.
A description of each functionality is provided, along with easy, medium, and sophisticated examples to illustrate how it can be used.

| Functionality | Description                                       | Example (Easy)                 | Example (Medium)                | Example (Sophisticated)             |
|---------------|---------------------------------------------------|--------------------------------|---------------------------------|------------------------------------|
| Declaration   | Creating a tuple                                  | `my_tuple = (1, 2, 3)`         | `my_tuple = ('apple', 'banana', 'cherry')` | `my_tuple = (10, 'hello', [1, 2, 3])` |
| Accessing Elements | Accessing elements in a tuple                | `print(my_tuple[0])`           | `print(my_tuple[-1])`            | `print(my_tuple[1])`                |
| Length        | Finding the length of a tuple                     | `print(len(my_tuple))`         | `print(len(my_tuple))`           | `print(len(my_tuple))`              |
| Concatenation | Concatenating two tuples                          | `tuple3 = tuple1 + tuple2`     | `tuple3 = tuple1 + tuple2`      | `tuple3 = tuple1 + tuple2`          |
| Repetition    | Creating a new tuple by repeating an existing tuple| `tuple2 = my_tuple * 2`        | `tuple2 = my_tuple * 3`         | `tuple2 = my_tuple * 4`             |
| Membership    | Checking if an element is present in a tuple       | `print(3 in my_tuple)`         | `print('orange' not in my_tuple)`| `print('hello' in my_tuple)`        |
| Index         | Finding the first index of a specified value       | `print(my_tuple.index('apple'))`| `print(my_tuple.index('banana'))`| `print(my_tuple.index(10))`       |
| Count         | Counting the number of occurrences of a specified value in a tuple | `print(my_tuple.count(1))` | `print(my_tuple.count('cherry'))`| `print(my_tuple.count([1, 2, 3]))` |
| Slicing       | Extracting a subset of a tuple                     | `print(my_tuple[1:3])`         | `print(my_tuple[::2])`           | `print(my_tuple[1:-1])`             |
| Unpacking     | Unpacking values from a tuple into variables       | `a, b, c = my_tuple`           | `x, y, z = my_tuple`             | `p, q, r = my_tuple`                |
| Immutability  | Values in a tuple cannot be changed once created   | `my_tuple[1] = 4`              | `del my_tuple[1]`               | `my_tuple[2][0] = 4`                |
| Comparison    | Comparing tuples lexicographically                 | `tuple1 < tuple2`              | `tuple1 > tuple2`               | `tuple1 < tuple2`                   |

#

## Details on each functionality

### Declaration
Creating a tuple with a specific set of elements.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)

# Example 2 (Medium)
my_tuple = ('apple', 'banana', 'cherry')

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
```
In Python, a tuple is created by enclosing a set of elements in parentheses. Each element in a tuple can be of a different data type.

In Example 1, we create a tuple of three integers.

In Example 2, we create a tuple of three strings.

In Example 3, we create a tuple of an integer, a string, and a list. Tuples are immutable, which means that their values cannot be changed once they are created.

#

### Accessing Elements
Retrieving individual elements of a tuple by their index.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
print(my_tuple[0])  # Output: 1

# Example 2 (Medium)
my_tuple = ('apple', 'banana', 'cherry')
print(my_tuple[2])  # Output: cherry

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
print(my_tuple[-1][1])  # Output: 2
```
In Python, elements in a tuple can be accessed using their index, which starts at 0 for the first element.

In the easy example, we create a tuple `my_tuple` with three integers and print the first element of the tuple using its index, which is 0. The output of this code is `1`, since the first element of the tuple is `1`.

In the medium example, we create a tuple `my_tuple` with three strings and print the last element of the tuple using its index, which is 2. The output of this code is `cherry`, since the last element of the tuple is `'cherry'`.

In the sophisticated example, we create a tuple my_tuple with three elements - an integer, a string, and a list. We then use two indices to retrieve the last element of the tuple, which is a list, and the second element of that list, which is 2. The output of this code is 2.

#

### Length
Determining the number of elements in a tuple.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
print(len(my_tuple))  # Output: 3

# Example 2 (Medium)
my_tuple = ('red', 'green', 'blue', 'yellow')
print(len(my_tuple))  # Output: 4

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
print(len(my_tuple))  # Output: 3
```
In Python, the len() function is used to determine the number of elements in a tuple.

In the easy example, we create a tuple `my_tuple` with three integers and use the `len()` function to determine the number of elements in the tuple, which is 3. The output of this code is `3`.

In the medium example, we create a tuple `my_tuple` with four strings and use the `len()` function to determine the number of elements in the tuple, which is 4. The output of this code is `4`.

In the sophisticated example, we create a tuple `my_tuple` with three elements - an integer, a string, and a list. We use the `len()` function to determine the number of elements in the tuple, which is 3. The output of this code is `3`.

#

### Concatenation
Combining two or more tuples into a single tuple.

```python
# Example 1 (Easy)
tuple3 = (1, 2, 3) + (4, 5, 6)
print(tuple3)  # Output: (1, 2, 3, 4, 5, 6)

# Example 2 (Medium)
tuple1 = ('a', 'b', 'c')
tuple2 = ('d', 'e', 'f')
tuple3 = tuple1 + tuple2
print(tuple3)  # Output: ('a', 'b', 'c', 'd', 'e', 'f')

# Example 3 (Sophisticated)
fruits = ('apple', 'banana', 'cherry')
vegetables = ('carrot', 'tomato', 'spinach')
groceries = fruits + vegetables
print(groceries)  # Output: ('apple', 'banana', 'cherry', 'carrot', 'tomato', 'spinach')
```
In Python, the `+` operator can be used to concatenate two tuples into a new tuple. The resulting tuple contains all the elements of the first tuple followed by all the elements of the second tuple.

In the easy example, we simply concatenate two tuples of integers, `(1, 2, 3)` and `(4, 5, 6)`, using the `+` operator and assign the resulting tuple to a variable `tuple3`. We then print `tuple3` to verify that the new tuple contains all the elements of the two original tuples.

In the medium example, we concatenate two tuples of strings, `('a', 'b', 'c')` and `('d', 'e', 'f')`, into a new tuple `tuple3`, and then print `tuple3` to verify that it contains all the elements of the two original tuples in the correct order.

In the sophisticated example, we concatenate two tuples of different data types, `('apple', 'banana', 'cherry')` and `('carrot', 'tomato', 'spinach')`, into a new tuple `groceries`. We then print `groceries` to verify that it contains all the elements of the two original tuples, with the elements of the second tuple following those of the first tuple.

#

### Repetition
Creating a new tuple by repeating an existing tuple a specified number of times.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
print(my_tuple * 3)  # Output: (1, 2, 3, 1, 2, 3, 1, 2, 3)

# Example 2 (Medium)
my_tuple = ('a', 'b', 'c')
print(my_tuple * 2)  # Output: ('a', 'b', 'c', 'a', 'b', 'c')

# Example 3 (Sophisticated)
my_tuple = (1, 2, 3)
print(my_tuple * 0)  # Output: ()
```
In Python, the `*` operator is used to repeat a tuple a specified number of times.

In the easy example, we create a tuple `my_tuple` with three integers and use the `*` operator to repeat the tuple three times. The resulting tuple contains all the elements of the original tuple repeated three times, and the output of this code is `(1, 2, 3, 1, 2, 3, 1, 2, 3)`.

In the medium example, we create a tuple `my_tuple` with three strings and use the `*` operator to repeat the tuple two times. The resulting tuple contains all the elements of the original tuple repeated two times, and the output of this code is `('a', 'b', 'c', 'a', 'b', 'c')`.

In the sophisticated example, we create a tuple `my_tuple` with three integers and use the `*` operator to repeat the tuple zero times. Since multiplying any tuple by zero results in an empty tuple, the output of this code is `()`.

#

### Membership
Checking if an element is present in a tuple.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
print(2 in my_tuple)  # Output: True

# Example 2 (Medium)
my_tuple = ('red', 'green', 'blue', 'yellow')
print('yellow' not in my_tuple)  # Output: False

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
print([1, 2, 3] in my_tuple)  # Output: True
```
In Python, the `in` and `not in` operators are used to check if an element is present in a tuple.

In the easy example, we create a tuple `my_tuple` with three integers and use the in operator to check if the element `2` is present in the tuple. Since `2` is one of the elements in `my_tuple`, the output of this code is `True`.

In the medium example, we create a tuple `my_tuple` with four strings and use the not in operator to check if the element `'yellow'` is not present in the tuple. Since `'yellow'` is one of the elements in `my_tuple`, the output of this code is `False`.

In the sophisticated example, we create a tuple `my_tuple` with three elements of different data types and use the in operator to check if the list `[1, 2, 3]` is present in the tuple. Since the list `[1, 2, 3]` is one of the elements in `my_tuple`, the output of this code is `True`.
#

### Index
Finding the index of the first occurrence of a given element in a tuple.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
print(my_tuple.index(2))  # Output: 1

# Example 2 (Medium)
my_tuple = ('red', 'green', 'blue')
print(my_tuple.index('green'))  # Output: 1

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
print(my_tuple.index([1, 2, 3]))  # Output: 2
```
In Python, the `index()` method is used to find the index of the first occurrence of a given element in a tuple.

In Example 1, we create a tuple of three integers and find the index of the integer `2` using the `index()` method. Since `2` is the second element in the tuple (i.e., at index 1), the output of this code is `1`.

In Example 2, we create a tuple of three strings and find the index of the string `'green'` using the `index()` method. Since `'green'` is the second element in the tuple (i.e., at index 1), the output of this code is `1`.

In Example 3, we create a tuple of an integer, a string, and a list, and find the index of the list `[1, 2, 3]` using the `index()` method. Since `[1, 2, 3]` is the third element in the tuple (i.e., at index 2), the output of this code is `2`.

#

### Count
Counting the number of occurrences of a given element in a tuple.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 2, 3, 2)
print(my_tuple.count(2))  # Output: 3

# Example 2 (Medium)
my_tuple = ('red', 'green', 'green', 'blue')
print(my_tuple.count('green'))  # Output: 2

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3], [1, 2, 3])
print(my_tuple.count([1, 2, 3]))  # Output: 2
```
In Python, the `count()` method is used to count the number of occurrences of a given element in a tuple.

In Example 1, we create a tuple of five integers and count the number of occurrences of the integer 2 using the `count()` method. Since `2` appears 3 times in the tuple, the output of this code is `3`.

In Example 2, we create a tuple of four strings and count the number of occurrences of the string `'green'` using the `count()` method. Since `'green'` appears 2 times in the tuple, the output of this code is `2`.

In Example 3, we create a tuple of an integer, a string, and two lists, and count the number of occurrences of the list `[1, 2, 3]` using the `count()` method. Since `[1, 2, 3` appears 2 times in the tuple, the output of this code is `2`.

#

### Slicing
Extracting a portion of a tuple by specifying the start and end indices.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3, 4, 5)
print(my_tuple[1:4])  # Output: (2, 3, 4)

# Example 2 (Medium)
my_tuple = ('apple', 'banana', 'cherry', 'orange', 'kiwi')
print(my_tuple[2:5])  # Output: ('cherry', 'orange', 'kiwi')

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3], 'world', 5.5)
print(my_tuple[1:3])  # Output: ('hello', [1, 2, 3])
```
In Python, tuples can be sliced using the colon `:` operator to specify the start and end indices of the slice.

In the easy example, we create a tuple `my_tuple` with five integers and use slicing to extract the elements between indices 1 and 4 (inclusive). Since indexing starts at 0 in Python, these indices correspond to the second through fifth elements of `my_tuple`. Therefore, the output of this code is `(2, 3, 4)`.

In the medium example, we create a tuple `my_tuple` with five strings and use slicing to extract the elements between indices 2 and 4 (inclusive). Therefore, the output of this code is `('cherry', 'orange', 'kiwi')`.

In the sophisticated example, we create a tuple `my_tuple` with five elements of different types and use slicing to extract the elements between indices 1 and 2 (inclusive). Therefore, the output of this code is `('hello', [1, 2, 3])`.

#

### Unpacking
Assigning the values of a tuple to multiple variables at once.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
a, b, c = my_tuple
print(a)  # Output: 1
print(b)  # Output: 2
print(c)  # Output: 3

# Example 2 (Medium)
my_tuple = ('apple', 'banana', 'cherry')
x, y, z = my_tuple
print(x)  # Output: apple
print(y)  # Output: banana
print(z)  # Output: cherry

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
p, q, r = my_tuple
print(p)  # Output: 10
print(q)  # Output: hello
print(r)  # Output: [1, 2, 3]
```
In Python, tuples can be used to assign multiple values to multiple variables at once. This is called tuple unpacking.

In the easy example, we create a tuple `my_tuple` with three integers and use unpacking to assign the values of the tuple to three variables `a`, `b`, and `c` respectively. We then print the values of these variables to confirm that the values were assigned correctly. Therefore, the output of this code is:
```python
1
2
3
```

In the medium example, we create a tuple `my_tuple` with three strings and use unpacking to assign the values of the tuple to three variables `x`, `y`, and `z` respectively. We then print the values of these variables to confirm that the values were assigned correctly. Therefore, the output of this code is:
```python
apple
banana
cherry
```

In the sophisticated example, we create a tuple `my_tuple` with three elements of different types and use unpacking to assign the values of the tuple to three variables `p`, `q`, and `r` respectively. We then print the values of these variables to confirm that the values were assigned correctly. Therefore, the output of this code is:
```python
10
hello
[1, 2, 3]
```

#

### Immutability
Tuples are immutable, meaning their values cannot be changed once they are created.

```python
# Example 1 (Easy)
my_tuple = (1, 2, 3)
my_tuple[1] = 4
print(my_tuple)  # Output: TypeError: 'tuple' object does not support item assignment

# Example 2 (Medium)
my_tuple = ('apple', 'banana', 'cherry')
del my_tuple[1]
print(my_tuple)  # Output: TypeError: 'tuple' object doesn't support item deletion

# Example 3 (Sophisticated)
my_tuple = (10, 'hello', [1, 2, 3])
my_tuple[2][0] = 4
print(my_tuple)  # Output: (10, 'hello', [4, 2, 3])
```
In Python, tuples are immutable, which means that their values cannot be changed once they are created.

In Example 1, we attempt to change the value of the second element `2` in a tuple of three integers, but we get a `TypeError` because tuples are immutable.

In Example 2, we attempt to delete the second element `'banana` in a tuple of three strings, but we get a `TypeError` because tuples are immutable.

In Example 3, we create a tuple of an integer, a string, and a list, and change the value of the first element of the list using the indexing operator. This is possible because the list is mutable, but the tuple itself is still immutable.

#

### Comparison
Comparing tuples lexicographically.

```python
# Example 1 (Easy)
tuple1 = (1, 2, 3)
tuple2 = (1, 2, 4)
print(tuple1 < tuple2)  # Output: True

# Example 2 (Medium)
tuple1 = ('apple', 'banana', 'cherry')
tuple2 = ('apple', 'banana', 'kiwi')
print(tuple1 > tuple2)  # Output: False

# Example 3 (Sophisticated)
tuple1 = (10, 'hello', [1, 2, 3])
tuple2 = (10, 'world', [1, 2, 3])
print(tuple1 < tuple2)  # Output: True
```
In Python, tuples can be compared lexicographically using the comparison operators `<`, `<=`, `>`, and `>=`. The comparison starts with the first element of each tuple and proceeds until a difference is found or all elements are compared.

In Example 1, we create two tuples of three integers each, and compare them lexicographically using the `<` operator. The result is `True` because the first tuple has a smaller third element than the second tuple.

In Example 2, we create two tuples of three strings each, and compare them lexicographically using the `>` operator. The result is `False` because the first tuple has a smaller third element than the second tuple.

In Example 3, we create two tuples of an integer, a string, and a list, and compare them lexicographically using the `<` operator. The result is `True` because the first tuple has a smaller second element than the second tuple.


