# Python-interview-questions
### 1. Difference between List and Tuple in Python?
- **List**: Mutable, uses `[]`, slower, more functionality.
- **Tuple**: Immutable, uses `()`, faster, safer.

### 2. How do sets help in removing duplicates?
Using `set(list)` converts the list into a set, which automatically removes duplicates.

```python
my_list = [1, 2, 2, 3]
unique = list(set(my_list))
```
### 3. Why are dictionaries faster than lists for lookups?
Dictionaries use hashing, enabling O(1) lookup time. Lists require O(n) time to search.

### 4. How are Python strings immutable if they allow replace()?
replace() creates a new string; it doesn’t modify the original.
```python
s = "hello"
print(s.replace("h", "y"))  # Output: yello
print(s)  # Still "hello"
```

### 5.How do you merge two dictionaries in python latest version?
the | operator merges the two dictionaries
```python
d1 = {'a': 1}
d2 = {'b': 2}
merged = d1 | d2
```

### 6. Explain dictionary comprehension with example?
dictionary comprehension is a concise and elegant way to create dictionaries in python by using a single line of code
```python
squares = {x: x*x for x in range(5)}
```


### 7. What are nested dictionaries and how do they you access inner values?
A nested dictionary is a dictionary within another dictionary. It's used to store complex or hierarchical data in a structured way.
```python
data = {"person": {"name": "Alice", "age": 25}}
print(data["person"]["name"])
```

### 8. How can you convert the list of tuples in to a dictionary?
```python
pairs = [('a', 1), ('b', 2)]
d = dict(pairs)
```

### 9. How would you handle missing Key in a dictionary ?
```python
my_dict = {"a": 1}
print(my_dict.get("b", "Not Found"))
```

### 10. Can we use a list as a key in a dictionary? why and why not?
No – lists are mutable and unhashable. Only immutable types can be keys.


### 11. What happens if you try add a mutable object to set?
You'll get a TypeError
since sets require elements to be hashable.
```python
s = set()
s.add([1, 2])  # TypeError
```

### 12. Write a code to find common elements in two lists using set operations?
```python
a = [1, 2, 3]
b = [2, 3, 4]
print(list(set(a) & set(b)))  # [2, 3]
```

### 13. What is the difference between is and ==for string ? what is the syntax?
is: Identity check
==: Value check
```python
a = "hello"
b = "hello"
print(a is b)   # True in CPython due to interning
print(a == b)   # Always True if values are same
```

### 14. How does sciling works in tuple and string? what are the syntax?
```python
s = "hello"
print(s[1:4])  # ell
t = (0, 1, 2, 3)
print(t[::2])  # (0, 2)
```

### 15. How can you reserve a string or list in python using sciling?
```python
s = "hello"
print(s[::-1])  # olleh
lst = [1, 2, 3]
print(lst[::-1])  # [3, 2, 1]
```











