Counter is a **container data type**, part of the built-in collections module. Counters are useful when you need to count the number of occurrences of elements in a list or other iterable and/or access the count for individual elements.

_Here are some examples of situations where the Counter class might be useful:_

- Counting the number of occurrences of words in a text file or a string.
- Counting the number of occurrences of elements in a list.
- Finding the most common elements in a list or other iterable.
- Keeping track of the counts of elements in a list or other iterable as it is updated over time.

Being a _dict()_ subccalss, when given a iterable, it will return a dictionary that maps the elements of the iterable to their counts.
Example:

'''python
from collections import Counter

lst = [1, 2, 2, 3, 3, 3, 4, 4, 4, 4]
counter = Counter(lst)
print(counter) # Output: Counter({4: 4, 3: 3, 2: 2, 1: 1})
'''
