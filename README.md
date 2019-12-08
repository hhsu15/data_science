## Data Science
Review of data science


### Some triks
#### pandas
You can group by numeric values by ranges:
- refer to Multiregression.ipynb
```python
bins = np.arange(0,50000,10000)  # make the ranges you want
my_groups = pd.cut(df['Mileage'],bins) # fit the rows into each range
groups = df.groupby(my_groups).mean()  # calculate average for each group
```
