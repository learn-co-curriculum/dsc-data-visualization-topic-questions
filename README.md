## Data Visualization

In this checkpoint you will be using a FIFA dataset of soccer player statistics to create a visualization, then also interpreting a visualization we have created.


```python
# Run this cell without changes
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
%matplotlib inline
```


```python
# Run this cell without changes
df = pd.read_csv('./data/fifa.csv')
df.head()
```

**1) Find the top 10 countries with the most players (using the 'Nationality' column). Create a bar chart showing the number of players in those 10 countries**

Don't forget to add a **title** and **x axis label** to your charts.

If you are unable to find the top 10 countries but want the chance to demonstrate your plotting skills use the following dummy data to create a bar chart
```
Country Name  | Num Players
============  | ===========
Country A     | 100
Country B     | 60
Country C     | 125
Country D     | 89
```


```python
# Code here to get the top 10 countries with the most players

```


```python
# Code here to plot a bar chart.  A recommended figsize is (10, 6)

```

**2) Below is code for a scatter plot for the player stats `StandingTackle` and `SlidingTackle`**


```python
# Run this cell without changes
fig, ax = plt.subplots()

ax.set_title('Standing Tackle vs. Sliding Tackle')
ax.set_xlabel('Standing Tackle')
ax.set_ylabel('Sliding Tackle')

x = df['StandingTackle']
y = df['SlidingTackle']

ax.scatter(x, y)
```

**How would you describe the relationship between these two features?**


```python
# Your written answer here
```
