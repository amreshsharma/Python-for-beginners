In this section we learn about Python generators. They were introduced in Python 2.3. It is an easier way to create iterators 
using a keyword yield from a function.

### A Python generator is a function which returns a generator iterator (just an object we can iterate over) by calling yield .
### yield may be called with a value,in which case that value is treated as the "generated" 

In general, a generator is a special routine that can be used to control the iteration behaviour of a loop. A generator is similar to a 
function returning an array. A generator has parameters, it can be called and it generates a sequence of numbers. But unlike functions,
which return a whole array, a generator yields one value at a time. This requires less memory.

```
def gen():
   x, y = 1, 2
   yield x, y
   x += 1
   yield x, y


it = gen()

print it.next()
print it.next()

try:
   print it.next()
except StopIteration:
   print "Iteration finished"
   
>>> def my_generator():
...     print("Inside my generator")
...     yield 'a'
...     yield 'b'
...     yield 'c'
...
>>> my_generator()
```

In the above example we create a simple generator using the yield statements. We can use it in a for loop just like we use any other
iterators.

```
>>> for char in my_generator():
...     print(char)
...
```
Inside my generator
a
b
c