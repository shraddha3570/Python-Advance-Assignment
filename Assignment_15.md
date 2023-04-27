

```python
1.What are the new features added in Python 3.8 version?
Answer:
Positional-only parameters(/)
There is a new function parameter syntax “/” which indicates that some function parameters must be specified positionally 
and can’t be used as keyword arguments.
Assignment Expressions(:=)
This operator is used to assign and return a value in the same expression. This removes the need for initializing the 
variable upfront.
f-strings now support “=”
No parentheses for return and yield statements ‘yield’ and ‘return’ statements do not require parentheses to return
multiple values.
```


```python
2.What is monkey patching in Python?
Answer:
In python, monkey patching refers to run-time modifications of a class or module. In Python, we can actually change the
behavior of code at run-time.
```


```python
3.What is the difference between a shallow copy and deep copy?
Answer:
In python, when we use = operator, it does not create a copy of the object. It just creates the variable, which shares a 
reference to the same memory location. This is called as shallow copy. In deep copy, new object is a copy of old object
and it is created at different memory address and any changes made to new object won't be reflected in old object.
```


```python
4.What is the maximum possible length of an identifier?
Answer:
The maximum possible length of an identifier is not defined in Python. It can be any number.
```


```python
5.What is generator comprehension?
Answer:
It is like a list comprehension but it returns an iterator. We use () instead of [] to achieve this.
numbers = (i for i in range(5))
print(numbers)
print(next(numbers))
print(next(numbers))
print(next(numbers))
print(next(numbers))
print(next(numbers))
<generator object <genexpr> at 0x000002138D30EC50>
0
1
2
3
4
```
