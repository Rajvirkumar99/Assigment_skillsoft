1. Topic Name: Data Frame
Target audience : A new commerce graduate who wants to pursue a career in the field of Data Analysis
Explanation 
A DataFrame is a two-dimensional, tabular data structure commonly used in data analysis and manipulation — especially in Python with the pandas library.

✅ Features of DataFrame:
•	Can hold different data types (integer, float, string, etc.)
•	Labeled axes (rows and columns)
•	Built on top of NumPy

Language Mostly Use 
1.	Python Pandas 
2.	R language 
Pandas is a powerful open-source Python library for data analysis and manipulation.
It offers two core data structures:
1.	Series → 1D labeled array (like a single column)
2.	DataFrame → 2D labeled table (like Excel or SQL table)




Series :
A Series is a one-dimensional labeled array capable of holding any data type (integers, strings, floats, etc.). Think of it like a single column in Excel.
🧩 Structure of Series
Index    Value
  0      'Raj'
  1      'Simran'
  2      'Rahul'


import pandas as pd

s = pd.Series(['Raj', 'Simran', 'Rahul'])
print(s)

DataFrame:
📘 Theory:
A DataFrame is a 2-dimensional labeled data structure with columns of potentially different types.
You can think of it as a table (like Excel or SQL):
•	Rows have indexes
•	Columns have labels

🧩 Structure of DataFrame:
Index | Name    | Age | City
-------------------------------
   0  | Raj     | 25  | Delhi
   1  | Simran  | 30  | Mumbai
   2  | Rahul   | 22  | Pune

Code Example:
data = {
    'Name': ['Raj', 'Simran', 'Rahul'],
    'Age': [25, 30, 22],
    'City': ['Delhi', 'Mumbai', 'Pune']
}
df = pd.DataFrame(data)
print(df)

DIAGRAM: Series vs DataFrame

Series (1D)                                                   
------------                     
Index   Value
  0     10
  1     20
  2     30                  
DataFrame (2D)
--------------------------
Index | Name   | Age | City
  0   | Raj    | 25  | Delhi
  1   | Simran | 30  | Mumbai
  2   | Rahul  | 22  | Pune


🔍 Difference Between Series and DataFrame
Feature	Series	DataFrame
Dimension	1D	2D
Structure	Single column	Multiple columns
Axis Labels	Index only	Rows (index) + Columns
Real-Life Use	One column of a table	Full table (rows & columns)
Example	List of names	Table of names, ages, cities

How to Load Datasets in DataFrame

1. Load from CSV
df = pd.read_csv('filename.csv')
2. Load from Excel
df = pd.read_excel('filename.xlsx')
3. Load from JSON
df = pd.read_json('filename.json')
🔍 Useful DataFrame Functions
Function	Purpose
df.head()	First 5 rows
df.tail()	Last 5 rows
df.shape	Rows and columns count
df.columns	List of column names
df.dtypes	Data types of columns
df.info()	Summary of DataFrame
df.describe()	Stats summary for numeric columns

🧠 Summary
•	Series = 1D (like a column)
•	DataFrame = 2D (like a table)
•	Pandas is used to handle structured data
•	You can create DataFrames from lists, dicts, NumPy arrays, or external files (CSV, Excel)
	

