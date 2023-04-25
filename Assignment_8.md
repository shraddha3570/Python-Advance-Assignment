

```python
Q1. What are the two latest user-defined exception constraints in Python 3.X?
Answer:
raise statement - This is used to raise an inbuilt exception explicitly.
assert statement - when condition in assert statement is true, program is executed normally.
When condition is false, program gives an AssertionError.
```


```python
Q2. How are class-based exceptions that have been raised matched to handlers?
Answer:
When exceptions are raised, then the exception is handled by the same class mentioned in except statement or its base
classes. "Exception" is the base class(Superclass) for all other exception classes.
```


```python
Q3. Describe two methods for attaching context information to exception artefacts.
Answer:
By using logging.exception() method, we can log log messages with level ERROR on the logger. It will store the information like type of error, line number, file name and path.
By using raise keyword. It will also display Traceback of the recent exception raised.

import logging
try: 
    4/0
except Exception as e: 
    logging.exception(e)
    raise
    
```


```python
Q4. Describe two methods for specifying the text of an exception object's error message.
Answer:
We can print the text of an exception, by using the object of an Exception class.
We can access different attributes like messgae, args, traceback from that object.
By using logging.error() method
```


```python
Q5. Why do you no longer use string-based exceptions?
Answer:
In Python versions 1.5 and earlier, Exceptions were strings and not classes. Now all exceptions are classes, 
derived from the superclass BaseException. With classes it is more efficiently handled as classes have many useful features.
```
