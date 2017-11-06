# Python tuple

### In Python, tuple is immutable. You cannot change elements of a tuple once it is assigned.

A tuple is a sequence of immutable Python objects. Tuples are sequences, just like lists. The differences between tuples and lists are,
the tuples cannot be changed unlike lists and tuples use parentheses, whereas lists use square brackets.
```
tup1 = ('physics', 'chemistry', 1997, 2000);
tup2 = (1, 2, 3, 4, 5 );
tup3 = "a", "b", "c", "d";
```

### Accessing Values in Tuples:
To access values in tuple, use the square brackets for slicing along with the index or indices to obtain value available at that index. For example −
```
#!/usr/bin/python

tup1 = ('physics', 'chemistry', 1997, 2000);
tup2 = (1, 2, 3, 4, 5, 6, 7 );

print "tup1[0]: ", tup1[0]
print "tup2[1:5]: ", tup2[1:5]
```
### Updating Tuples
Tuples are immutable which means you cannot update or change the values of tuple elements.
