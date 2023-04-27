

```python
Q1. Is an assignment operator like += only for show? Is it possible that it would lead to faster results at the runtime?
Answer:
+= is faster and easy to write for us. runtime of a += 5 is slightly less than a = a + 5 but, the difference is 
really minor.
```


```python
Q2. What is the smallest number of statements you'd have to write in most programming languages to replace the Python
expression a, b = a + b, a?
Answer:
Two
```


```python
Q3. In Python, what is the most effective way to set a list of 100 integers to 0?
Answer:
l = [0] * 100
print(l)
```


```python
Q4. What is the most effective way to initialise a list of 99 integers that repeats the sequence 1, 2, 3? S If necessary, 
show step-by-step instructions on how to accomplish this.
Answer:
l1 = [1,2,3] # create a list containing 1,2,3
count = int(101/len(l1)) # repeat count
l =  l1 * count # * operator is used to repeat the list
print(l)
```


```python
Q5. If you're using IDLE to run a Python application, explain how to print a multidimensional list as efficiently?
Answer:
We can print multidimentional list by simply writing the name of the variable in a cell
l = [[1,2,3,4],['A','B'],[5,6,7,8]]
l
[[1, 2, 3, 4], ['A', 'B'], [5, 6, 7, 8]]
```


```python
Q6. Is it possible to use list comprehension with a string? If so, how can you go about doing it?
Answer:
Yes, it is possible as string is an iterable object. Explained below:
s = 'shraddha'
[i*2 for i in s]
['ss', 'hh', 'rr', 'aa', 'dd', 'dd', 'hh', 'aa']
```


```python
Q7. From the command line, how do you get support with a user-written Python programme? Is this possible from inside IDLE?
Answer:
Steps for command line:
1. Open command prompt.
2. Go to the directory containing python program file(.py)
3. Type "python file_name.py", press enter to run the file.
Steps for python IDLE:
1. Open python IDLE.
2. Click on file>open>file_name.py
3. Press F5 key to run the program.
```


```python
Q8. Functions are said to be “first-class objects” in Python but not in most other languages, such as C++ or Java. 
What can you do in Python with a function (callable object) that you can't do in C or C++?
Answer:
In Python, functions are like any other object, such as an int or a list. That means that you can use functions as 
arguments to other functions, store functions as dictionary values, or return a function from another function.
This leads to many powerful ways to use functions.
```


```python
Q9. How do you distinguish between a wrapper, a wrapped feature, and a decorator?
Answer:
A wrapper, a wrapped feature, and a decorator are all same. They can be thought of as functions which modify the
functionality of another function. They help to make your code shorter and more "Pythonic".
```


```python
Q10. If a function is a generator function, what does it return?
Answer:
If a function is a generator function, it does not return any values, instead, it return an iterator object, 
which we can iterate through to get values.
```


```python
Q11. What is the one improvement that must be made to a function in order for it to become a generator function in 
the Python language?
Answer:
We can use "yield" keyword instead of "return" to make function a generator.
```


```python
Q12. Identify at least one benefit of generators.
Answer:
The main advantage here is that instead of having to compute an entire series of values up front, the generator computes
one value and then suspends its activity awaiting the next instruction. This feature is known as state suspension.
Generators are memory efficient.
```
