

```python
Q1. What is the purpose of Python's OOP?
Answer:
Provides a clear program structure and a clean code
Facilitates easy maintenance and modification of existing code.
Since the class is sharable, the code can be reused.
Since the class is sharable, the code can be reused and many other such Advantages.
```


```python
Q2. Where does an inheritance search look for an attribute?
Answer:
Attribute fetches are simply tree searches. The term inheritance is applied because objects lower in a tree inherit
attributes attached to objects higher in that tree. As the search proceeds from the bottom up, in a sense, 
the objects linked into a tree are the union of all the attributes defined in all their tree parents, all the way
up the tree.
```


```python
Q3. How do you distinguish between a class object and an instance object?
Answer:
Objects and Instances are almost similar and are often used interchangeably but with a small difference. 
bject is a generic term , it is physically present but remains undiferrentiated. Instance is something that 
gives them a separate identity.
Object is the physical entity for which memory is allocated. Object contains many instances.
Instance : An instance is also the physical manifestation of a class that occupies memory and has data members.
e.g. There is Class car, when I create c = car(), c is object. When we create different object with different
specifications(car name, type, company) such as i10, i20, Creta, audi7 are called as instances which actually exists.
```


```python
Q4. What makes the first argument in a class’s method function special?
Answer:
Self represents the instance of the class. By using the “self” keyword we can access the attributes and methods of the
class in python. It binds the attributes with the given arguments.The reason you need to use self. is because Python does
not use the @ syntax to refer to instance attributes. Python decided to do methods in a way that makes the instance to 
which the method belongs be passed automatically, but not received automatically: the first parameter of methods is 
the instance the method is called on.
```


```python
Q5. What is the purpose of the __init__ method?
Answer:
The task of init method is to initialize(assign values) to the data members of the class when an object of class is 
created. It contains collection of statements that are executed at time of Object creation. It is run as soon as an 
object of a class is instantiated. The method is useful to do any initialization you want to do with your object.
```


```python
Q6. What is the process for creating a class instance?
Answer:
To create instances of a class, you call the class using class name and pass in whatever arguments its init method accepts.
```


```python
Q7. What is the process for creating a class?
Answer:
The class statement creates a new class definition. The name of the class immediately follows the keyword class
followed by a colon.
```


```python
Q8. How would you define the superclasses of a class?
Answer:
A superclass is the class from which many subclasses can be created. 
The subclasses inherit the characteristics of a superclass.
The superclass is also known as the parent class or base class.
```
