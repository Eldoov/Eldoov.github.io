---
title: "Pandas Note 1"
date: 2023-04-10
draft: false
---

# Pandas note


Find all nan values in df

```
# Below are the quick examples

# Example 1: Count the NaN values in single column
nan_count = df['Fee'].isna().sum()

# Example 2: Count NaN values in multiple columns of DataFrame
nan_count = df.isna().sum() 

# Example 3: Count NaN values of whole DataFrame
nan_count = df.isna().sum().sum()

# Example 4: Count the NaN values in single row
nan_count = df.loc[['r1']].isna().sum().sum()

# Example 5: Count the NaN values in multiple rows
nan_count = df.isna().sum(axis = 1)
```

Find unique value

```
# Find unique values in all columns
for col in df:
  print(df[col].unique())

output:
['A' 'B' 'C']
['East' 'West']
[11  8 10  6  5]

# Find unique value in one column
df.team.unique()

output:
array(['A', 'B', 'C'], dtype=object)

# Find and sort

#find unique points values
points = df.points.unique()

#sort values smallest to largest
points.sort()

#display sorted values
points

output:
array([ 5,  6,  8, 10, 11])

# Find and Count Unique Values in a Column
df.team.value_counts()

output:
A    3
B    2
C    1
Name: team, dtype: int64

#count unique values in each column
df.nunique()

#count unique values in each row
df.nunique(axis=1)

```

Fillna method (fill nan with mean of one column)

```
df['price'].fillna(df['price'].mean(), inplace = True)

#fill given number
df_obj.fillna('66.0')  # 使用66.0替换缺失值
df_obj.fillna({'A': 4.0, 'B': 5.0}) # 指定列填充数据
df.fillna(method='ffill')  # 使用前向填充的方式替换空值或缺失值
df_obj.dropna()   # 删除数据集中的空值和缺失值

```

Row count 

```
rows_count = len(df.index)
rows_count = len(df.axes[0])
rows_count = df.shape[0]
rows_count = df.count()[0]
```

#School/Homework #School/Note
