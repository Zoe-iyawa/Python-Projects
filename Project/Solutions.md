# Required Tasks
These are the required tasks for this project. 
1. Read the data from the spreadsheet
2. Collect all of the sales from each month into a single list
3. Output the total sales across all months

## Answers 
- Read the data from the spreadsheet
N.B The sales file has been saved amongst my other python file

```python
import pandas as pd
df = pd.read_csv('sales.csv')
df

 	year 	month 	sales 	expenditure
0 	2018 	jan 	6226 	3808
1 	2018 	feb 	1521 	3373
2 	2018 	mar 	1842 	3965
3 	2018 	apr 	2051 	1098
4 	2018 	may 	1728 	3046
5 	2018 	jun 	2138 	2258
6 	2018 	jul 	7479 	2084
7 	2018 	aug 	4434 	2799
8 	2018 	sep 	3615 	1649
9 	2018 	oct 	5472 	1116
10 	2018 	nov 	7224 	1431
11 	2018 	dec 	1812 	3532
```
- Collect all of the sales from each month into a single list
```python
df['sales']

0     6226
1     1521
2     1842
3     2051
4     1728
5     2138
6     7479
7     4434
8     3615
9     5472
10    7224
11    1812
Name: sales, dtype: int64
```
- Output the total sales across all months
```python
total_sales = df['sales'].sum()
x = 'The total sales across all months is: {}'.format(total_sales)
x
```
The total sales across all months is: 45542

### Additional learning 
1.
```python
df = pd.read_csv('sales.csv') # The column index was changed from default figures to 'month' column
df = df.set_index('month')
df

year 	sales 	expenditure
month 			
jan 	2018 	6226 	3808
feb 	2018 	1521 	3373
mar 	2018 	1842 	3965
apr 	2018 	2051 	1098
may 	2018 	1728 	3046
jun 	2018 	2138 	2258
jul 	2018 	7479 	2084
aug 	2018 	4434 	2799
sep 	2018 	3615 	1649
oct 	2018 	5472 	1116
nov 	2018 	7224 	1431
dec 	2018 	1812 	3532

```
2.
```python
average_sales = df['sales'].mean()

'The average sales is {}'.format(average_sales) # The average sales in year 2018
```
The average sales is 3795.1666666666665

3. 
```python
df['sales'].min()  # the lowest sales within 2018
```
The lowest sales is 1521

# Visualization

```python
import matplotlib.pyplot as plt    # import matplot 
import numpy as np
import pandas as pd

df['sales'].plot(kind = 'bar', title = 'Monthly Sales', ylabel = 'Sales', color = ['purple', 'blue', 'green'])  # create a bar chart visualization with multiple colours.
```
Link to Graph here: ![Graph](/Users/zoephilipiyawa/PycharmProjects/pythonProject2/monthly_sales.png)


