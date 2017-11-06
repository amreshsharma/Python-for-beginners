## The list is a most versatile datatype available in Python which can be written as a list of comma-separated values (items) between 
square brackets.
Important thing about a list is that items in a list need not be of the same type.
```
list1 = ['physics', 'chemistry', 1997, 2000];
list2 = [1, 2, 3, 4, 5 ];
list3 = ["a", "b", "c", "d"]
```
### Accessing Values in Lists -
To access values in lists, use the square brackets for slicing along with the index or indices to obtain value available at that index.
Example:
```
list1 = ['physics', 'chemistry', 1997, 2000];
list2 = [1, 2, 3, 4, 5, 6, 7 ];

print "list1[0]: ", list1[0]
print "list2[1:5]: ", list2[1:5]

#Output
list1[0]:  physics
list2[1:5]:  [2, 3, 4, 5]
```
You can update single or multiple elements of lists by giving the slice on the left-hand side of the assignment operator, and you can
add to elements in a list with the append() method.

Here are all of the methods of list objects:
```
list.append(x)
Add an item to the end of the list; equivalent to a[len(a):] = [x].

list.extend(L)
Extend the list by appending all the items in the given list; equivalent to a[len(a):] = L.

list.insert(i, x)
Insert an item at a given position. The first argument is the index of the element before which to insert, so a.insert(0, x) inserts at the front of the list, and a.insert(len(a), x) is equivalent to a.append(x).

list.remove(x)
Remove the first item from the list whose value is x. It is an error if there is no such item.
```
