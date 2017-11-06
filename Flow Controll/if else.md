
### The if…elif…else statement is used in Python for decision making.
```
if test expression:
    statement(s)
    
Example:
num = 6
if num > 0:
    print(num, "is a positive number.")

Syntax of if...else - 

if test expression:
    Body of if
else:
    Body of else
    
Syntax of if...elif...else -

if test expression:
    Body of if
elif test expression:
    Body of elif
else: 
    Body of else
```  
    
### Python Nested if statements
We can have a if...elif...else statement inside another if...elif...else statement. This is called nesting in computer programming.
```
num = float(input("Enter a number: "))
if num >= 0:
    if num == 0:
        print("Zero")
    else:
        print("Positive number")
else:
    print("Negative number")
```
