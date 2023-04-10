# Ex03-Univariate-Analysis
import pandas as pd
df=pd.read_csv("/content/SuperStore.csv")
df.head()
![image](https://user-images.githubusercontent.com/112244898/230829043-55d2cde5-4e37-4c20-b3ff-dfbad75a58bc.png)
df.info()
![image](https://user-images.githubusercontent.com/112244898/230829161-c091279f-ebd4-4ec6-917a-602ad9625fa5.png)
df.dtypes
![image](https://user-images.githubusercontent.com/112244898/230829616-c61eed59-a3ba-4f8f-9f2a-74a7c52af88c.png)
df['Postal Code'].value_counts()
![image](https://user-images.githubusercontent.com/112244898/230829635-9b843ba6-57d2-48b3-9b47-6e1d151507d9.png)
df['Sales'].value_counts()
![image](https://user-images.githubusercontent.com/112244898/230829647-4a345271-42d9-42f9-a2c4-b4b59951b313.png)
df.describe()
![image](https://user-images.githubusercontent.com/112244898/230829702-e059fed1-5539-475a-b199-61bb63292b5e.png)
import seaborn as sns
sns.boxplot(x="Sales",data=df)
![image](https://user-images.githubusercontent.com/112244898/230829756-c7483c5d-c8e7-4a16-9106-d93656269b6a.png)
import seaborn as sns
sns.boxplot(x="Postal Code",data=df)
![image](https://user-images.githubusercontent.com/112244898/230829817-ee355c87-7a14-4786-8109-6c5f66dc7c0d.png)
sns.countplot(x="Postal Code",data=df)
![image](https://user-images.githubusercontent.com/112244898/230829979-eafadf97-1448-4bd6-b307-5bbd69c285b5.png)
sns.distplot(df["Postal Code"])
![image](https://user-images.githubusercontent.com/112244898/230830138-33f1c71c-9ff6-4ea5-a51c-d2545fbbdee5.png)
sns.distplot(df["Sales"])
![image](https://user-images.githubusercontent.com/112244898/230830231-2af30846-8a93-4767-bbc8-3cc8836a465b.png)
sns.histplot(x="Postal Code",data=df)
![image](https://user-images.githubusercontent.com/112244898/230830322-9fc1a111-f7e9-464a-81b7-27da108d7f2f.png)
sns.histplot(x="Sales",data=df)
![image](https://user-images.githubusercontent.com/112244898/230830364-d2caec3f-b753-4056-831f-9990cebaa30f.png)


