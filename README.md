# Ex03-Univariate-Analysis

## Aim

To read the given data and perform the univariate analysis with different types of plots.

## Explanation

Univariate analysis is basically the simplest form to analyze data. Uni means one and this means that the data has only one kind of variable. The major reason for univariate analysis is to use the data to describe. The analysis will take data, summarise it, and then find some pattern in the data.

## Algorithm

### Step1
Read the given data.

### Step2
Get the information about the data.

### Step3
Remove the null values from the data.

### Step4
Mention the datatypes from the data.

### Step5
Count the values from the data.

### Step6
Do plots like boxplots,countplot,distribution plot,histogram plot.

## Program
```
Developed by : DHARSHINI DS
Registration Number : 212221230022

import pandas as pd
import numpy as np
import seaborn as sns
df=pd.read_csv("SuperStore.csv")
df
df.head()
df.info()
df.describe()
df.isnull().sum()
df.dtypes
df['Postal Code'].value_counts()
sns.boxplot(x="Postal Code", data=df)
sns.countplot(x="Postal Code", data=df)
sns.distplot(df["Postal Code"])
sns.histplot(x="Postal Code", data=df)
```
## OUTPUT

### DATA
![DS1](https://user-images.githubusercontent.com/93427345/191898791-4de0a8c9-8581-41ea-8d84-b5ec9c6743c7.PNG)

### DATA HEAD
![DS2](https://user-images.githubusercontent.com/93427345/191898834-8d3130d9-0b40-4365-a3ea-74e3d28431d2.PNG)

### DATA INFORMATION
![DS3](https://user-images.githubusercontent.com/93427345/191898931-2e68fa8f-cf9d-43bc-a312-daf160e07afc.PNG)

### DATA DESCRIBE
![DS4](https://user-images.githubusercontent.com/93427345/191899037-e94c8007-a87b-4ead-b12d-71bd330a2a8c.PNG)

### DATA NULL VALUES
![DS5](https://user-images.githubusercontent.com/93427345/191899055-86795845-012e-4143-b9c9-8713c4a43ff4.PNG)

### DATA DATA TYPES
![DS6](https://user-images.githubusercontent.com/93427345/191899082-b33f146f-342f-4f3a-91eb-a75f3df20ffc.PNG)

### DATA VALUE COUNT
![DS7](https://user-images.githubusercontent.com/93427345/191899148-cd36cef2-1862-47bc-b22d-5b103fceb4cb.PNG)

### BOXPLOT
![DS8](https://user-images.githubusercontent.com/93427345/191899185-be661814-d402-4245-ba45-cbe649579323.PNG)

### COUNTPLOT
![DS9](https://user-images.githubusercontent.com/93427345/191899219-e401211a-2cfc-4307-94c8-80141da63e6c.PNG)

### DISTRIBUTION PLOT
![DS10](https://user-images.githubusercontent.com/93427345/191899278-36e61237-4504-4203-b341-bb5da1c7a3e8.PNG)

### HISTOGRAM PLOT
![DS11](https://user-images.githubusercontent.com/93427345/191899301-c3316b5a-2418-44e3-8422-c2e772aca695.PNG)

## RESULT
Thus we have read the given data and performed the univariate analysis with different types of plots.
