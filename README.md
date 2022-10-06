# Ex03-Univariate-Analysis
AIM:
     
To determine the univariate and removal using IQR with given csv files.

ALGORITHM:

1)Start the program
2) Remove univariate using IQR
(3) After removing univariate in step 1, you get a new dataframe.
(4) use zscore of 3 to analysis univariate. This is quite similar to IQR and you will get exact same result
(5) for the data set superstore.csv find the following
6)stop the program

PROGRAM:


 import pandas as ps
import numpy as np
import seaborn as sns 
df=ps.read_csv("/content/SuperStore.csv")
df.info()
df.dtypes
df['Sales'].value_counts()
df.describe()
sns.boxplot(x="Sales",data=df)
sns.countplot(x="Postal Code",data=df)
sns.distplot(df["Sales"])
sns.histplot(x="Postal Code",data=df)

RESULT:


Thus the Univariate Analysis is completed successfully
