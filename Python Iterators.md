# Iterators
### Python iterator objects are required to support two methods while following the iterator protocol.

__iter__ returns the iterator object itself. This is used in for and in statements.

__next__ method returns the next value from the iterator. If there is no more items to return then it should raise StopIteration exception.

```
class Counter(object):
    def __init__(self, low, high):
        self.current = low
        self.high = high

    def __iter__(self):
        'Returns itself as an iterator object'
        return self

    def __next__(self):
        'Returns the next value till current is lower than high'
        if self.current > self.high:
            raise StopIteration
        else:
            self.current += 1
            return self.current - 1
            
 >>> c = Counter(5,10)
>>> for i in c:
...   print(i, end=' ')
...
5 6 7 8 9 10
```
