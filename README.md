# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
'''
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("titanic_dataset.csv")
 df.head()
 '''
<img width="1417" height="378" alt="image" src="https://github.com/user-attachments/assets/5cbb86b6-ea1e-40af-9f46-98787342dcdb" />
'''
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
 '''
<img width="832" height="646" alt="image" src="https://github.com/user-attachments/assets/7f761539-ed8c-4bdc-88ec-e60f621fb8c6" />
'''
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
 '''
<img width="767" height="730" alt="image" src="https://github.com/user-attachments/assets/6f92b02e-3c24-43fa-80e2-6bb811b4309c" />
'''
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
 '''
<img width="1447" height="785" alt="image" src="https://github.com/user-attachments/assets/e8fec287-14a7-489f-bc69-3b8a42914e3b" />
'''
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()
 '''

<img width="828" height="627" alt="image" src="https://github.com/user-attachments/assets/f37866bc-cb38-4027-b5b3-ed09606938c5" />
'''
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
 '''
<img width="942" height="635" alt="image" src="https://github.com/user-attachments/assets/8e9a272c-afa8-438e-af14-58c108d9d264" />
'''
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
 '''
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
 '''
<img width="819" height="583" alt="image" src="https://github.com/user-attachments/assets/09183fd1-b5dc-4a13-ae1d-c3e92b9d49e3" />
'''
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
 '''
  sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
 '''
<img width="1441" height="753" alt="image" src="https://github.com/user-attachments/assets/2e55d768-d10c-4744-bd7b-84aa6fc417c6" />
'''
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
 '''
<img width="908" height="630" alt="image" src="https://github.com/user-attachments/assets/4c2b364a-29ce-403a-94d2-2262c66bee7a" />
<img width="975" height="757" alt="image" src="https://github.com/user-attachments/assets/cf029b76-901c-400a-89f9-465b1312f383" />
<img width="831" height="733" alt="image" src="https://github.com/user-attachments/assets/65de35b8-e07d-4d42-b856-283d96ff4100" />


# Result:
 Thus, the Data Visualization using seaborn python library for the given data is implemented successfully.
