

```python
Q1. What is the distinction between a numpy array and a pandas data frame? Is there a way to convert between the two
if there is?
Answer:
Numpy array: This is in the form of matrix structure which have rows and columns. It generally performs python 
mathematical operation which is not genrally easy manually to perfomr in coding case. It may be of any 
dimensions like 1-d, 2-d, 3-d, 4-d, etc depend upon the use to requirement. Unlike dataframe, numpy array are 
not in a tabular form which ahve records and have fields instead it is in the form of matrices. It can have
single row and single column as well but dataframe poses more than one column
DataFrame: This is a kind of tabular structure format which are having more than one column. Unlike numpy 
array which can have more single as well as many number of columns, but dataframe have more than one column.
Dataframe can have any number of dimensons but it should be more than one. We can use numpy array operation 
in dataframe and can also convert the numpy array into dataframe.
We can convert between the two in following manner:

```


```python
import pandas as pd
import numpy as np
array=np.arange(10).reshape(2,5)
array
```




    array([[0, 1, 2, 3, 4],
           [5, 6, 7, 8, 9]])




```python
df=pd.DataFrame(array)
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>0</th>
      <th>1</th>
      <th>2</th>
      <th>3</th>
      <th>4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>0</td>
      <td>1</td>
      <td>2</td>
      <td>3</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>5</td>
      <td>6</td>
      <td>7</td>
      <td>8</td>
      <td>9</td>
    </tr>
  </tbody>
</table>
</div>




```python
Q2. What can go wrong when an user enters in a stock-ticker symbol, and how do you handle it?
Answer: User may end up with wrong asset
```


```python
Q3. Identify some of the plotting techniques that are used to produce a stock-market chart.
Answer:
LINE CHART.POINT AND FIGURE CHART, CANDLESTICK CHART, BAR CHART.
```


```python
Q4. Why is it essential to print a legend on a stock market chart?
Answer:
Legends adds a beauty to visualize the trend of data w.r.t. different features. It creates the different 
trend in different colors indicating that which is belong to which trend is belong to which feature.
```


```python
Q5. What is the best way to limit the length of a pandas data frame to less than a year?
Answer:
We can use start and end parameters for that. In start we write the date from where we are starting and at 
the end we write the end date. SO within this span we can restric the duration. Also we can use the parameters 
like periods for how much times we need the duration and we can also use the frequency parameter.
```


```python
Q6. What is the definition of a 180-day moving average?
Answer:
Moving Averages help to filter out market noise and smooth out fluctuations in price. In statistics, a moving
average is a calculation used to analyze data points by creating a series of averages of different subsets of 
the full data set. 180-day moving average means A simple moving average (SMA) is a arithmetic mean of a given 
set of prices over the 180 days in the past
```
