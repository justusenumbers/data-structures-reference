#Counter

The Counter is a **container data type**, part of the built-in collections module. Counters are useful when you need to count the number of occurrences of elements in a list or other iterable and/or access the count for individual elements.

_The Counter class is useful for:_

- Counting the number of occurrences of words in a text file or a string.
- Counting the number of occurrences of elements in a list.
- Finding the most common elements in a list or other iterable.
- Keeping track of the counts of elements in a list or other iterable as it is updated over time.

Being a _dict()_ subccalss, when given a iterable, it will return a dictionary that maps the elements of the iterable to their counts.
Example:

```python
from collections import Counter

# Count the occurrences of each character in a string
string = 'abcabcabc'
counter = Counter(string)
print(counter)  # Output: Counter({'a': 3, 'b': 3, 'c': 3})

# Count the occurrences of each word in a list
words = ['apple', 'banana', 'apple', 'grape', 'banana', 'banana']
counter = Counter(words)
print(counter)  # Output: Counter({'banana': 3, 'apple': 2, 'grape': 1})

# Find the two most common elements in a list
most_common = counter.most_common(2)
print(most_common)  # Output: [('banana', 3), ('apple', 2)]

# Update the counter with the counts from another iterable
counter.update([1, 1, 2, 3, 3, 3, 4, 5])
print(counter)  # Output: Counter({'banana': 3, 'apple': 2, '3': 3, '1': 2, '2': 1, '4': 1, '5': 1, 'grape': 1})
```
