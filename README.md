# Ex-01_DS_Data_Cleansing
# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# ALGORITHM
## STEP 1
Read the given Data

## STEP 2
Get the information about the data

## STEP 3
Remove the null values from the data

## STEP 4
Save the Clean data to the file

# CODE
import pandas as pd

df=pd.read_csv('/content/Data_set.csv')

df.head()

df.info()

df.head(10)

df.isnull()

df ["show_name"]=df['show_name'].fillna(df[ 'aired_on'].mode()[0])

df.head()

df ["aired_on"]=df['aired_on'].fillna(df[ 'aired_on'].mode()[0])

df.head()

df ["original_network"]=df['original_network'].fillna(df[ 'aired_on'].mode()[0])

df.head()

df.isnull().sum()


# OUPUT

![Screenshot (4)](https://user-images.githubusercontent.com/84709944/226189032-5561794d-226b-4aea-a9e0-bd61d11ca521.png)

![Screenshot (5)](https://user-images.githubusercontent.com/84709944/226189044-fba52e20-8156-490e-ac4a-bf920ee64917.png)

![Screenshot (6)](https://user-images.githubusercontent.com/84709944/226189058-c20425d1-9119-491b-bf26-dbb1fb93bdbf.png)

![Screenshot (7)](https://user-images.githubusercontent.com/84709944/226189071-71b30474-e981-40ae-ae6b-7ac2cb344f5c.png)

![Screenshot (8)](https://user-images.githubusercontent.com/84709944/226189083-3a93b366-ece8-4918-b040-735d7bf0b125.png)

![Screenshot (9)](https://user-images.githubusercontent.com/84709944/226189095-56e36c58-c5b7-4518-a8dc-899ec0f1f19e.png)

![Screenshot (10)](https://user-images.githubusercontent.com/84709944/226189105-592e4cbb-445e-4efa-8d66-8b28e6179e0b.png)

![Screenshot (11)](https://user-images.githubusercontent.com/84709944/226189120-638b40e1-2ba0-4973-a120-6f4bd3784f15.png)

![Screenshot (12)](https://user-images.githubusercontent.com/84709944/226189126-5e8d02bd-0f73-4666-afa5-8dcaa9fc4b85.png)

![Screenshot (13)](https://user-images.githubusercontent.com/84709944/226189144-7e5ebe56-08f8-40e6-9f81-62b762ddaf2c.png)

![Screenshot (14)](https://user-images.githubusercontent.com/84709944/226189156-7d69ea2e-c0e4-4d3f-9a07-110f56196b95.png)

![Screenshot (14)](https://user-images.githubusercontent.com/84709944/226189173-ad294424-1698-4e0d-820c-44f84b4768e0.png)

![Screenshot (15)](https://user-images.githubusercontent.com/84709944/226189187-aea46f3d-8a14-44b7-a1ac-45fdb9d0979a.png)

![Screenshot (16)](https://user-images.githubusercontent.com/84709944/226189194-c0a18e05-9b74-42cd-b89d-9661985aeec3.png)

![Screenshot (17)](https://user-images.githubusercontent.com/84709944/226189205-5304d833-93b3-4a3e-9e15-02fa0d19328d.png)

![Screenshot (18)](https://user-images.githubusercontent.com/84709944/226189210-def0d8bb-342c-4ac4-9770-ca28c1529460.png)

![Screenshot (19)](https://user-images.githubusercontent.com/84709944/226189217-cb47f13a-1dd0-42f0-b28e-5a3840775844.png)

![Screenshot (20)](https://user-images.githubusercontent.com/84709944/226189226-aaad1b62-5fd8-48de-800e-1c94a8f9e6e0.png)

Result:
Hence the given data is read,cleaned and saved into a file successfully.
