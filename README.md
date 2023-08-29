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
df=pd.read_csv("SAMPLEDS.csv")

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
# OUTPUT
![s1](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/c2398868-01dd-41c5-be5e-e8890b57fa5b)
![s2](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/e6cf20e9-6bf2-4a54-ab67-d54564d7300f)
![s3](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/0b2eaaa4-e12a-4bc9-8538-094b3a11e67c)
![s4](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/42c26296-b814-4731-8757-48d36c08153d)
![s5](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/e6974564-a05e-4d27-ab69-bc74864895c5)

![s6](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/b6fec48e-ec4f-41bc-bb4a-100e1bc0694f)

![s7](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/19c79787-442f-4d37-a3b3-61b218234860)

![s8](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/1852f27c-7f8a-47d7-949d-adcceba0672d)

![s9](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/78e5fde7-8aff-4bc8-8ef9-c481b88829ee)

![s10](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/d4868e3b-4357-441b-89ed-cfc3845614b9)

![s11](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/102a246f-0256-42e5-82ba-e394ca7ea123)
![s12](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/7109344e-8905-4c2e-af99-28c35aeadfbb)
![s13](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/18fd29c4-9a25-46be-bec6-95552c0372c4)
![s14](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/0a475af2-e2e6-4113-8884-5cdff81aa082)
![s15](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/e14948e9-61c0-45ea-9264-f4d8166bbb86)
![s16](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/350527c2-7b20-45e9-a192-44a4593e9248)
![s17](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/a1d24814-3d2b-482d-a621-e2f15f30ac5a)
![s18](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/946fc7ce-ed02-4e11-ac07-79337286b0e6)

![s19](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/a658d648-8aae-4476-9477-a9dd24c21dad)

![s20](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/b8dffd5e-ed28-41c4-a9c3-8e2fd43ac1c1)

![s21](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/731fb274-ca89-44b3-a84d-b925f265a3b3)

![s22](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/1d7df624-5183-4436-ad88-7b10f1a191a0)

![s23](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/11e1db84-ad2a-491e-996c-c9692255f846)
![s24](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/d828d812-a82a-4ca4-aa7b-22cd6d1067ec)
![s25](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/3a38ec20-bd1d-4dae-852f-d306b6532435)
![s26](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/ee0a653d-deee-437d-a21d-35c117ea12f0)
![s27](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/4d7dede5-efe5-4bc2-881e-2708cd5364b7)
![s28](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/7640524a-67af-48f3-a6fa-19614d0817c2)
![s29](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/ef99cac9-6cac-4ce7-a592-b2d73e472299)
![s30](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/c420a488-2544-40b6-bcc0-17d9f8790ec1)

![s31](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/b14b4684-0933-480f-8a8a-2c1370605a3c)

![s32](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/62bf0d06-f9cc-4349-b090-1fa4a030f03c)
![s33](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/09a50b4a-6fa1-47dd-8678-7bf119bd59db)
![s34](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/830ff8dc-f784-4912-83a3-8b7baea29fad)
![s35](https://github.com/SmritiManikand/ODD2023-Datascience-Ex01/assets/113674204/beaacd3c-4bc2-4fe9-add5-d5961a11ca91)

# RESULT
Thus,the given data is read,cleansed and the cleaned data is saved into the file.
