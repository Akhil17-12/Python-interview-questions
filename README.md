# Python-interview-questions
### 1. Difference between List and Tuple in Python?
- **List**: Mutable, uses `[]`, slower, more functionality.
- **Tuple**: Immutable, uses `()`, faster, safer.

### 2. How do sets help in removing duplicates?
Using `set(list)` converts the list into a set, which automatically removes duplicates.

```python
my_list = [1, 2, 2, 3]
unique = list(set(my_list))

### 3.3. Why are dictionaries faster than lists for lookups?
Dictionaries use hashing, enabling O(1) lookup time. Lists require O(n) time to search.
