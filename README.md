# Ex-08-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.


# CODE
```
import numpy as np
import pandas as pd
df=pd.read_csv("sus.csv")
df.head()
df.info()
import matplotlib.pyplot as plt
plt.bar(df['Segment'],df['Sales'])
df.Segment.unique()
plt.bar(df["City"],df["Profit"])
plt.bar(df["Ship Mode"],df["Profit"])
plt.scatter(df["Sales"],df["Profit"])
plt.xlabel("Sales")
plt.ylabel("profit")

import seaborn as sns
plt.plot(df['Segment'], df['Sales'])
plt.show()
plt.plot(df['Segment'], df['Profit'])

sns.lineplot(x='Profit',y='Sales', hue ="Segment",data=df)

sns.lineplot(x='Profit',y='Sales', hue ="Ship Mode",data=df)

sns.lineplot(x='Profit',y='Sales', hue ="Region",data=df)

sns.lineplot(y='Profit',x='Region',data=df)


```
# OUPUT

![image](https://user-images.githubusercontent.com/94154683/200159624-6d30dd61-0f63-4f21-9aa7-9e6e914d9ef1.png)

![image](https://user-images.githubusercontent.com/94154683/200159635-c18b9bb1-9d35-43e8-b19b-fa71ec1538c0.png)

![image](https://user-images.githubusercontent.com/94154683/200159645-3be55068-2978-424c-b4ac-dfeae452fbfc.png)

![image](https://user-images.githubusercontent.com/94154683/200159658-b8665875-3b0a-40a4-b828-1c168d88b2b6.png)

![image](https://user-images.githubusercontent.com/94154683/200159723-2e017a6f-6e74-4054-acc2-216b084c4696.png)

![image](https://user-images.githubusercontent.com/94154683/200159731-00289bec-17f7-4a2a-b462-0257746c9aa6.png)

![image](https://user-images.githubusercontent.com/94154683/200159737-81fd4223-f862-49cb-82f5-454b1191e04a.png)

![image](https://user-images.githubusercontent.com/94154683/200159742-2d9c8bcd-8f23-41fd-af5f-48e1ccb4119f.png)

![image](https://user-images.githubusercontent.com/94154683/200159761-dc7acda9-f9ac-4399-8c1b-18b0fa77d28b.png)

![image](https://user-images.githubusercontent.com/94154683/200159767-8d2bfabd-957c-4e26-af2e-04dc38725eaa.png)


# Result:
Hence, Data Visualization is applied using libraries like Seaborn and Matplotlib successfully and got tha data insights.







