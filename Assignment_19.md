

```python
Q1. Define the relationship between a class and its instances. Is it a one-to-one or a one-to-many partnership, for example?
Answer:
Class is abstraction of an real world entity. It consists of attributes and methods. Instance is an object of a class. 
Its one to many relationship between class and its instatnces.
```


```python
Q2. What kind of data is held only in an instance?
Answer:
Instance objects contains the Instance variables which are specific to that specific Instance object.
```


```python
Q3. What kind of knowledge is stored in a class?
Answer:
Class creates a user-defined data structure, which holds its own data members and member functions,which can be 
accessed and used by creating an instance of that class. A class is like a blueprint for an object. 
```


```python
Q4. What exactly is a method, and how is it different from a regular function?
Answer:
The methods with a class can be used to access the instance variables of its instance. So, the object's state 
can be modified by its method. Function cant access the attributes of an instance of a class or cant modify the state of 
the object.
```


```python
Q5. Is inheritance supported in Python, and if so, what is the syntax?
Answer:
Inheritance is supported by python
Example:
```


```python
class A:
    var=1
    def __init__(self):
        pass
class B(A): # class B is detived from class A
    def __init__(self):
        super().__init__()
c=B()
print("Class of Instance:",c.__class__)
print("Base class:",c.__class__.__bases__)

```

    Class of Instance: <class '__main__.B'>
    Base class: (<class '__main__.A'>,)
    


```python
Q6. How much encapsulation (making instance or class variables private) does Python support?
Answer:
Encapsulation prevents from accessing accidentally, but not intentionally. The private attributes and methods are not 
really hidden. The private attributes can be accessed within the object method.
```


```python
Q7. How do you distinguish between a class variable and an instance variable?
Answer:
The class attribute is available to all the instance objects of that class. Instance variable is accessible only to the
object or Instance of that class
```


```python
Q8. When, if ever, can self be included in a class's method definitions?
Answer:
self can included to access the class variables and instance variiables.
```


```python
Q9. What is the difference between the _ _add_ _ and the _ _radd_ _ methods?
Answer:
When you add two numbers using the + operator, internally, the __add__() method will be called. We can overload this method 
to perform
```


```python
Q10. When is it necessary to use a reflection method? When do you not need it, even though you support the operation in question?
Answer:
Suppose we are implementing a class that you want to act like a number via operator overloading.So we implement
 __add__ in your class, and now expressions like obj + 10 is acceptable.This is because obj + 10 is interpreted as
    obj.__add__(10), and the custom method __add__ can do whatever it means to add 10 to custom class.
However, what about an expression like 10 + obj which is really (10).__add__(myobj)? 
The 10 is an instance of a Python built-in type and its __add__ method doesn't know anything about the new type,obj,
so it will return a error NotImplemented. 
To handle such scenarios, __radd__ is used. Python will first try (10).__add__(myobj), 
and if that returns NotImplemented, Python will check if the right-hand operand implements 
__radd__, and if it does, it will call obj.__radd__(10) rather than raising a TypeError.
```


```python
Q11. What is the _ _iadd_ _ method called?
Answer:
__iadd__ method is called when we use implementation like a+=b which is a.__iadd__(b)
```


```python
Q12. Is the _ _init_ _ method inherited by subclasses? What do you do if you need to customize its behavior within
a subclass?
Answer:
__init__ method is inherited by its subclass. But it can be overloaded, to customize it
```


```python
class A:
    def __init__(self,x):
        self.x=x
class B(A):
    pass
obj=B(2)
obj.x 
#        here the value x is accessible to instance of class B which is subclass of class A.This means
#        __init__ of class A is inherited in sub class B
class C(A):
    def __init__(self,x,y): # Here we are overloading the __init__ inherited from class A 
        self.x=x
        self.y=y
    def func(self):
        return(self.x + self.y)
obj1=C(3,4)
obj1.func()
```




    7


