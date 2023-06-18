Q1. How do you load a CSV file into a Pandas DataFrame?
Ans: To load a CSV file into a Pandas DataFrame, you can use the read_csv() function. The read_csv() function takes a path to the CSV file as its argument.

import pandas as pd
df = pd.read_csv("path/to/csv/file.csv")

Q2. How do you check the data type of a column in a Pandas DataFrame?
Ans: To check the data type of a column in a Pandas DataFrame, you can use the dtype attribute. The dtype attribute returns the data type of the column.

df["column_name"].dtype

Q3. How do you select rows from a Pandas DataFrame based on a condition?
Ans: To select rows from a Pandas DataFrame based on a condition, you can use the loc attribute. The loc attribute takes a Boolean expression as its argument. The Boolean expression is evaluated, and the rows that satisfy the condition are returned.

df = df[df["column_name"] == "value"]

Q4. How do you rename columns in a Pandas DataFrame?
Ans: To rename columns in a Pandas DataFrame, you can use the rename() method. The rename() method takes a dictionary as its argument. The dictionary maps the old column names to the new column names.

df = df.rename(columns={"old_column_name": "new_column_name"})

Q5. How do you drop columns in a Pandas DataFrame?
Ans: To drop columns in a Pandas DataFrame, you can use the drop() method. The drop() method takes a list of column names as its argument. The columns that are listed in the list are dropped from the DataFrame.

df = df.drop(["column_name1", "column_name2"], axis=1)

Q6. How do you find the unique values in a column of a Pandas DataFrame?
Ans: Use the unique() method. The unique() method returns a list of the unique values in the column.

df["column_name"].unique()

Q7. How do you find the number of missing values in each column of a Pandas DataFrame?
Ans: To find the number of missing values in each column of a Pandas DataFrame, you can use the isnull() method. The isnull() method returns a Boolean Series, where True indicates a missing value and False indicates a non-missing value. The sum() method can then be used to count the number of True values in each column.

df.isnull().sum()

Q8. How do you fill missing values in a Pandas DataFrame with a specific value?
Ans: To fill missing values in a Pandas DataFrame with a specific value, you can use the fillna() method. The fillna() method takes a value as its argument and replaces all missing values in the DataFrame with the specified value.

df = df.fillna(value)

Q9. How do you concatenate two Pandas DataFrames?
Ans: To concatenate two Pandas DataFrames, you can use the concat() method. The concat() method takes a list of DataFrames as its argument and concatenates them along the specified axis.

df = pd.concat([df1, df2], axis=1)

Q10. How do you merge two Pandas DataFrames on a specific column?
Ans: To merge two Pandas DataFrames on a specific column, you can use the merge() method. The merge() method takes two DataFrames and a column name as its arguments and merges the DataFrames on the specified column.

df = pd.merge(df1, df2, on="column_name")

Q11. How do you group data in a Pandas DataFrame by a specific column and apply an aggregation function?
Ans: To group data in a Pandas DataFrame by a specific column and apply an aggregation function, you can use the groupby() method. The groupby() method takes a column name as its argument and returns a GroupBy object. The GroupBy object can then be used to apply aggregation functions to the grouped data.

df = df.groupby("column_name").agg({"column_name": "mean"})

Here, the mean() aggregation function is applied to the "column_name" column.

Q12. How do you pivot a Pandas DataFrame?
Ans: To pivot a Pandas DataFrame, you can use the pivot() method. The pivot() method takes a column name as its argument and returns a pivot table. The pivot table can then be used to summarize the data in a different way.

df = df.pivot("column_name", "another_column_name")

Here,the pivot table is created by pivoting on the "column_name" column and the "another_column_name" column.

Q13. How do you change the data type of a column in a Pandas DataFrame?
Ans: To change the data type of a column in a Pandas DataFrame, you can use the astype() method. The astype() method takes a data type as its argument and returns a Series with the converted data type.

df["column_name"] = df["column_name"].astype("int")

Q14. How do you sort a Pandas DataFrame by a specific column?
Ans: To sort a Pandas DataFrame by a specific column, you can use the sort_values() method. The sort_values() method takes a column name as its argument and sorts the DataFrame by the specified column.

df = df.sort_values("column_name")

Q15. How do you create a copy of a Pandas DataFrame?
Ans: To create a copy of a Pandas DataFrame, you can use the copy() method. The copy() method returns a copy of the DataFrame.

df_copy = df.copy()

Q16. How do you filter rows of a Pandas DataFrame by multiple conditions?
Ans: To filter rows of a Pandas DataFrame by multiple conditions, you can use the & (and) or | (or) operators. The & operator is used to filter rows that satisfy both conditions, and the | operator is used to filter rows that satisfy either condition.

df = df[(df["column_name1"] == "value1") & (df["column_name2"] == "value2")]

Q17. How do you calculate the mean of a column in a Pandas DataFrame?
Ans: To calculate the mean of a column in a Pandas DataFrame, you can use the mean() method. The mean() method takes a column name as its argument and returns the mean of the values in the column.

mean_value = df["column_name"].mean()

Q18. How do you calculate the standard deviation of a column in a Pandas DataFrame?
Ans: To calculate the standard deviation of a column in a Pandas DataFrame, you can use the std() method. The std() method takes a column name as its argument and returns the standard deviation of the values in the column.

std_value = df["column_name"].std()

Q19. How do you calculate the correlation between two columns in a Pandas DataFrame?
Ans: To calculate the correlation between two columns in a Pandas DataFrame, you can use the corr() method. The corr() method takes two column names as its arguments and returns the correlation coefficient between the two columns.

correlation_coefficient = df["column_name1"].corr(df["column_name2"])

Q20. How do you select specific columns in a DataFrame using their labels?
Ans: To select specific columns in a DataFrame using their labels, you can use the loc attribute. The loc attribute takes a list of column names as its argument and returns a DataFrame with the selected columns.

df = df.loc[:, ["column_name1", "column_name2"]]

Q21. How do you select specific rows in a DataFrame using their indexes?
Ans: You can use the `loc` or `iloc` accessors to select specific rows in a DataFrame using their indexes. The `loc` accessor allows you to select rows by label, while the `iloc` accessor allows you to select rows by position.
For example, to select the row with the index label "A": df.loc["A"]
To select the first row in the DataFrame, : df.iloc[0]

Q22. How do you sort a DataFrame by a specific column?
Ans: You can use the `sort_values` method to sort a DataFrame by a specific column. The `sort_values` method takes two arguments: the column name and the sort order. The sort order can be either `"ascending"` or `"descending"`.

df.sort_values("Name", ascending=True)

Q23. How do you create a new column in a DataFrame based on the values of another column?
Ans: You can use the `assign` method to create a new column in a DataFrame based on the values of another column. The `assign` method takes a dictionary as its argument. The keys of the dictionary are the names of the new columns, and the values of the dictionary are the expressions that will be used to calculate the values of the new columns.

df = df.assign(Age_Group=lambda x: x["Age"].astype("category").cat.codes)

Q24. How do you remove duplicates from a DataFrame?
Ans: You can use the `drop_duplicates` method to remove duplicates from a DataFrame. The `drop_duplicates` method takes two arguments: the column(s) to check for duplicates and the keep option. 

df = df.drop_duplicates("Column_Name")

Q25. What is the difference between .loc and .iloc in Pandas?
Ans: The 'loc' and 'iloc' accessors are used to select rows and columns in a DataFrame. The 'loc' accessor allows you to select rows and columns by label, while the 'iloc' accessor allows you to select rows and columns by position.
