# Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn

## AIM:
To write a program to implement the Decision Tree Classifier Model for Predicting Employee Churn.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import the required libraries.
2. Upload and read the dataset.
3. Check for any null values using the isnull() function.
4. From sklearn.tree import DecisionTreeClassifier and use criterion as entropy.
5. Find the accuracy of the model and predict the required values by importing the required module from sklearn.

## Program:
```
/*
Program to implement the Decision Tree Classifier Model for Predicting Employee Churn.
Developed by:Sharon Harshini L M 
RegisterNumber: 212223040193

import pandas as pd
data=pd.read_csv("Employee.csv")
data.head()

data.info()

data.isnull().sum()

data['left'].value_counts()

from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data['salary']=le.fit_transform(data['salary'])
data.head()

x=data[['satisfaction_level','last_evaluation','number_project','average_montly_hours','time_spend_company','Work_accident','promotion_last_5years','salary']]
x.head()

y=data['left']

from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=100)
from sklearn.tree import DecisionTreeClassifier
dt=DecisionTreeClassifier(criterion='entropy')
dt.fit(x_train,y_train)
y_predict=dt.predict(x_test)

from sklearn import metrics
accuracy=metrics.accuracy_score(y_test,y_predict)
accuracy

dt.predict([[0.5,0.8,9,206,6,0,1,2]])

*/
```

## Output:
1.read_csv

![1](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/5198cb2b-f172-4b34-a6e5-d34aae75aaa5)

2.Null Values

![2](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/a1233c8a-656d-408d-9374-32a1aedc7f4d)

3.Left value count

![3](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/0264c8ac-675b-44e2-bb19-07fe3c2fbad0)

4.Converting string to numerical

![4](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/d1d5a16e-5957-42eb-9116-1cffb4c1fb57)

5.Displaying the rows

![5](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/737c7202-bdfd-4b23-9e50-249a77acdf7d)

6.Decision tree classifier

![6](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/3fcea7b2-8db2-46d5-a883-2d258449a20d)

7.Accuracy

![7](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/8b20fcc0-87f9-4deb-9577-7f6dbefda18e)

8.Data prediction

![320173814-441719a0-d664-4283-ae45-c03d741ccd75](https://github.com/sharon120/Implementation-of-Decision-Tree-Classifier-Model-for-Predicting-Employee-Churn/assets/149555539/6894f4e1-14ee-4a1f-a844-c4f8f8343853)


## Result:
Thus the program to implement the  Decision Tree Classifier Model for Predicting Employee Churn is written and verified using python programming.
