# Exno:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# CODE
## DATA CLEANING PROCESS
```
import pandas as pd
df=pd.read_csv("/content/Data_set.csv")

df.head(5)

df.tail(3)

df.info()

df.describe()

df.isnull()

df.notnull()

df.dropna(axis=1)

dfs=df[df['rating']>8]
dfs

df.iloc[[1,3,6],[1,4]]

df=df.fillna(0)
df
```
# OUTPUT
![Screenshot 2024-03-09 212023](https://github.com/Roselinjovita/exno1/assets/119104296/bb42e70a-7dc1-4d7b-a3ce-55e4fc91adb3)

![Screenshot 2024-03-09 212059](https://github.com/Roselinjovita/exno1/assets/119104296/978deb48-9e84-47ad-b404-38e5741015d5)


![Screenshot 2024-03-09 212121](https://github.com/Roselinjovita/exno1/assets/119104296/e0607c3e-f1b0-4deb-b8f9-d9762d143683)


![Screenshot 2024-03-09 212131](https://github.com/Roselinjovita/exno1/assets/119104296/e8ee2c4f-446b-45cf-b212-1393fffad5be)

![Screenshot 2024-03-09 212159](https://github.com/Roselinjovita/exno1/assets/119104296/35704f6a-7e6c-418c-9fa0-09702f376648)

![Screenshot 2024-03-09 212220](https://github.com/Roselinjovita/exno1/assets/119104296/d64ec11f-3a7b-46cf-8e84-1bc502a609c8)


![Screenshot 2024-03-09 212323](https://github.com/Roselinjovita/exno1/assets/119104296/4b0a95eb-d8bf-47d0-9c31-f2d8b8c2ef4a)


# Result
 Thus the given data is read,cleansed and the cleaned data is saved into the file.      
