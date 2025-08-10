# Titanic Project Note

## Statistics and filling None
1. Statistice the datafrom all None
> ```python
    df = read_csv("your data")
    df.isna().sum()
```
This code lists the number of missing values (NaN) for each column.

2. Filling miss value
To fill missing values with the median of numerical columns, use the following code.

> ```python
    med = df.median(number_only) # # Calculate the median for numerical columns
    df = df.fillan(med)   # Fill missing values with the median
```

## Transfrom string to integers


## One-Hot Encoder


Transform string values to integers for model input, except for the "Sex" column, 
which contains "male" or "female".

The model raises an error when running with string values.

I can transform "male" to 1 and "female" to 2 to resolve this issue.

