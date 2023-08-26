# Ex-01_DS_Data_Cleansing


# AIM
To read the given data and perform data cleaning and save the cleaned data to a file. 

# EXPLANATION
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect, incompleted, irrelevant, duplicated or improperly formatted. 
Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information. 

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Get the information about the data
### STEP 3
Remove the null values from the data
### STEP 4
Save the Clean data to the file

# CODE 
```
import pandas as pd
df=pd.read_csv("/content/SAMPLEDS - Sheet1.csv")

df

df.head()

df.tail()

df.info()

df.describe()

df.shape

df.isnull().sum()

df.dropna(how='any').shape

x=df.dropna(how='any')

x

df.dropna(how='all').shape

df

tot=df.dropna(subset=['TOTAL'],how='any')

tot

m=df.dropna(subset=['M1','M2','M3','M4'],how='any')

m

df.fillna(0)

df

df.fillna(method='ffill')

df.fillna(method='bfill')

df.interpolate()

mn=df.TOTAL.mean()
mn

df.TOTAL.fillna(mn,inplace=True)
df

n=df.TOTAL.median()
n

m=df.TOTAL.mode()
m

df.isnull()

df.notnull()

df.dropna()

df.head()

df.tail()

df.info()

df.describe()

df

df.duplicated()

df

df.drop_duplicates(inplace=True)
df

df['cd']=pd.to_datetime(df['DOB'])
df

for x in df.index:
  if df.loc[x,"AVG"]>100:
    df.drop(x,inplace=True)

df
```
