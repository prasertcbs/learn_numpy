

```python
import pandas as pd
import matplotlib.pyplot as plt
%matplotlib inline
%config InlineBackend.figure_format = 'retina'
```

## read data from github


```python
df=pd.read_csv('https://github.com/prasertcbs/tutorial/raw/master/mpg.csv')
df.head()
df.tail()
```

## explore data
$$E=mc^2$$


```python
df.cty.plot(kind='box');
```


```python
df.hist();
```


```python
df.cty.hist();
```


```python
df.cty.hist();
```


```python
df.cty.hist(bins=20);
```


```python
df[['cty', 'hwy']].hist(grid=False, color='orange', sharex=True, sharey=True);
```


```python
df[['cty', 'hwy']].plot.hist(alpha=.2)
```


```python
df[['cty', 'hwy']].plot.hist();
```


```python
df.cty.plot.density();
```


```python
df.cty.plot.kde();
```


```python
df
```


```python
df['class'].value_counts()
```


```python
df['class'].value_counts().plot.bar()
```


```python
df['class'].value_counts().plot.barh(color='orange')
```


```python
df['class'].value_counts().plot.barh(color='.7')
```


```python
df['class'].value_counts().sort_values().plot.barh(color='.7')
```
