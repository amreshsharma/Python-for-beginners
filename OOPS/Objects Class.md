## Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes.
## Classes are essentially a template to create your objects.

## Class variable: A variable that is shared by all instances of a class. Class variables are defined within a class but outside any of the class's methods.
## Class variables are not used as frequently as instance variables are.

## Data member: A class variable or instance variable that holds data associated with a class and its objects.

### Function overloading: The assignment of more than one behavior to a particular function. The operation performed varies by the types of 
### objects or arguments involved.

### Instance variable: A variable that is defined inside a method and belongs only to the current instance of a class.

### Inheritance: The transfer of the characteristics of a class to other classes that are derived from it.

### Instantiation: The creation of an instance of a class.

# Creating Classes
The class statement creates a new class definition. The name of the class immediately follows the keyword class followed by a colon as
follows −
```
Syntex:

class ClassName:
   'Optional class documentation string'
   class_suite
  
 Example:
 
 class Employee:
   'Common base class for all employees'
   empCount = 0

   def __init__(self, name, salary):
      self.name = name
      self.salary = salary
      Employee.empCount += 1
   
   def displayCount(self):
     print "Total Employee %d" % Employee.empCount

   def displayEmployee(self):
      print "Name : ", self.name,  ", Salary: ", self.salary
```

## Creating Instance Objects -
   
 "This would create first object of Employee class"
emp1 = Employee("Zara", 2000)
"This would create second object of Employee class"
emp2 = Employee("Manni", 5000)


## You access the object's attributes using the dot operator with object. Class variable would be accessed using class name as follows −
```
emp1.displayEmployee()
emp2.displayEmployee()
print "Total Employee %d" % Employee.empCount
```

## Class Inheritance
Instead of starting from scratch, you can create a class by deriving it from a preexisting class by listing the parent class
in parentheses after the new class name.

The child class inherits the attributes of its parent class, and you can use those attributes as if they were defined in the child class.
A child class can also override data members and methods from the parent.


Syntax
Derived classes are declared much like their parent class; however, a list of base classes to inherit from is given after the class name −
```
class SubClassName (ParentClass1[, ParentClass2, ...]):
   'Optional class documentation string'
   class_suite
```
