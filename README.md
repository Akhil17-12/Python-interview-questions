# Python-interview-questions
### 1. Difference between List and Tuple in Python?
- **List**: Mutable, uses `[]`, slower, more functionality.
- **Tuple**: Immutable, uses `()`, faster, safer.

### 2. How do sets help in removing duplicates?
Using `set(list)` converts the list into a set, which automatically removes duplicates.

```python
my_list = [1, 2, 2, 3]
unique = list(set(my_list))
