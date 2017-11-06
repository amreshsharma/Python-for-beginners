## for Loop in Python

### Syntax of for Loop - 

```
for val in sequence:
	Body of for
  
Exampple:
# List of numbers
numbers = [6, 5, 3, 8, 4, 2]

# variable to store the sum
sum = 0

# iterate over the list
for val in numbers:
	sum = sum+val

# Output: The sum is 28
print("The sum is", sum)
```

### The range() function - 

We can generate a sequence of numbers using range() function. range(10) will generate numbers from 0 to 9 (10 numbers).
We can also define the start, stop and step size as range(start,stop,step size). step size defaults to 1 if not provided.
```
# Output: range(0, 5)
print(range(10))

# Output: [0, 1, 2, 3, 4]
```
### for loop with else -

A for loop can have an optional else block as well. The else part is executed if the items in the sequence used in for loop exhausts.
```
Example:
digits = [0, 1, 5]

for i in digits:
    print(i)
else:
    print("No items left.")
```