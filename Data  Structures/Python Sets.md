## Sets in Python -

A Set is an unordered collection data type that is iterable, mutable, and has no duplicate elements. Python’s set class
represents the mathematical notion of a set. The major advantage of using a set, as opposed to a list, is that it has a
highly optimized method for checking whether a speci?c element is contained in the set. This is based on a data structure known
as a hash table.

### Example:
```
Same as {"a", "b","c"}
normal_set = set(["a", "b","c"])
``` 
### Adding an element to normal set is fine
```
normal_set.add("d")
 
print("Normal Set")
print(normal_set)
 
# A frozen set
frozen_set = frozenset(["e", "f", "g"])
 
print("Frozen Set")
print(frozen_set)

Output:

Normal Set
set(['a', 'c', 'b', 'd'])
Frozen Set
frozenset(['e', 'g', 'f'])
```
