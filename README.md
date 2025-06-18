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
```python
d1 = {'a': 1}
d2 = {'b': 2}
merged = d1 | d2
```

### 6. Explain dictionary comprehension with example?
```python
squares = {x: x*x for x in range(5)}
```


### 7. What are nested dictionaries and how do they you access inner values?
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


