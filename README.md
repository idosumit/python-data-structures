# Python Data Structures
Easy explanation for Tuple, List, Set, and Dictionary in Python as I expand on my markdown note-taking ability.

## Each Data Structure in Detail

### [Tuples](https://github.com/psumitcode/python-data-structures/blob/main/Tuples.md)

#### Coming soon: Lists, Dictionaries, Sets

#

Note: This README file provides a quick summary of some important elements that are synonymous to most or all of the data structures. For details regarding each, please refer to the hyperlinks inside `Each Data Structure in Detail` section.

## Ordering and Indexing

| Functionality | List | Tuple | Set | Dictionary |
| --- | --- | --- | --- | --- |
| Ordered | ✓ | ✓ | ✕ | ✓¹ |
| Indexed | ✓ | ✓ | ✕ | ✕² |
| Duplicate Elements | ✓ | ✓ | ✕ | Keys Only |
| Mutable | ✓ | ✕ | ✓ | ✓ |
| Hashable | ✕ | ✓ | ✕³ | Keys Only |

¹ Starting from Python 3.7, dictionaries are ordered by default due to their implementation. However, it is important to note that this is a language-specific detail, and relying on the order of dictionaries is not recommended in general. For guaranteed ordering, we should consider using `collections.OrderedDict`. For details, see [OrderedDict](https://github.com/psumitcode/python-data-structures/blob/main/OrderedDict.md).

² Dictionaries are not indexed, but we can access their values using keys.

³ Sets are not hashable, as they are mutable, but their elements must be hashable. However, Python provides a special immutable version called `frozenset` that is hashable.

For details on the complexities of hashing in `Sets` and `Dictionaries`, see [Hashing Complexities](https://github.com/psumitcode/python-data-structures/blob/main/Hashing%20Complexities.md).
