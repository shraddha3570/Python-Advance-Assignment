

```python
Q1. What is the difference between __getattr__ and __getattribute__?
Answer:
Normally, if we want to access the attribute of a class, we access it with instance of the class like 
instance.attribute_name. These attributes are already present in the class. Where as, to access the attribute of class 
which are not defined in the class, we use getattr() method.
But if the attribute does exist, getattr won’t be invoked
class Sample:
    def __init__(self,address):
        self.address = address
    
    def __getattr__(self,name):
        return name.lower()
    
s =Sample('Banglore')
print(s.address) # existing attribute
print(s.ABCD) # ABCD is non defined in class

Banglore
abcd

getattribute will look for every attribute, doesn’t matter if the attribute exists or not.
class Dummy():

    def __getattribute__(self, attr):
        return 'New Value'

d = Dummy()
d.value = "Old value"
print(d.value)
New Value
```


```python
Q2. What is the difference between properties and descriptors?
Answer:
In Properties, We can bind getter, setter functions with an attribute name, using the built-in property function.
In descriptor, We can bind getter, setter (and deleter) functions into a separate class. We then assign an object of 
this class to the attribute name.
```


```python
Q3. What are the key differences in functionality between __getattr__ and __getattribute__, 
as well as properties and descriptors?
Answer:
To access the attribute of class which are not defined in the class, we use getattr() method. But if the attribute does
exist, getattr won’t be invoked. getattribute will look for every attribute, doesn’t matter if the attribute exists or not.

In Properties, We can bind getter, setter functions with an attribute name, using the built-in property function. 
In descriptor, We can bind getter, setter (and deleter) functions into a separate class. We then assign an object of this 
class to the attribute name.
```
