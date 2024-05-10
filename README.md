# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1. Import pandas
2. Import Decision Tree Classifier
3. Fit the data in the model
4. Find the accuracy score

## Program:

/*
### Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
### Developed by: V.Divyashree
### RegisterNumber: 212223230051
```
import pandas as pd
data=pd.read_csv("/content/Salary.csv")
data.head()
data.info()
data.isnull().sum()
from sklearn.preprocessing import LabelEncoder
le=LabelEncoder()
data["Position"]=le.fit_transform(data["Position"])
data.head()
x=data[["Position","Level"]]
x.head()
y=data["Salary"]
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn import metrics
mse=metrics.mean_squared_error(y_test,y_pred) 
mse
r2=metrics.r2_score(y_test,y_pred)
r2
dt.predict([[5,6]])
```
*/


## Output:
### data.head()

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/7ae6f988-792d-4411-bf52-a40ee02e22af)

### data.info()

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/b99b42ec-b0d7-42b3-a546-cdc3d178e16b)

### isnull() and sum()

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/9aaf0370-823d-4f70-b4f7-7a1ec38f33bf)

### data.head() for salary

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/3c449696-2586-416b-8ac7-6c0539fa84f2)

### MSE Value

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/803fc198-4ffe-416e-8a2d-6feb13ca2af0)

### r2 value
data prediction

![image](https://github.com/divya280/Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee/assets/82276099/35489784-631f-46e4-8d14-1d933893b5e4)

## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
