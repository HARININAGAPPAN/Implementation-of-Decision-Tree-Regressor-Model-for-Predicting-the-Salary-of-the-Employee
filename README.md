# Implementation-of-Decision-Tree-Regressor-Model-for-Predicting-the-Salary-of-the-Employee

## AIM:
To write a program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Jupyter notebook

## Algorithm
1.Import pandas

2.Import Decision tree classifier

3.Fit the data in the model

4.Find the accuracy score
## Program:
```
/*
Program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee.
Developed by: Harini N
RegisterNumber: 212223040057
import pandas as pd
data=pd.read_csv("Salary.csv")
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
y.head()
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test=train_test_split(x,y,test_size=0.2,random_state=2)
from sklearn.tree import DecisionTreeRegressor
dt=DecisionTreeRegressor()
dt.fit(x_train,y_train)
y_pred=dt.predict(x_test)
y_pred
from sklearn.metrics import r2_score
r2=r2_score(y_test,y_pred)
R2 score:  0.48611111111111116
dt.predict([[5,6]])


*/
```

## Output:
<img width="406" height="163" alt="image" src="https://github.com/user-attachments/assets/dfe1d02e-b084-409e-a5a1-cfb9edcd20d7" />
<img width="380" height="179" alt="image" src="https://github.com/user-attachments/assets/ac47175c-3f8f-4fe5-9cc0-13b7a8bd97d5" />
<img width="308" height="97" alt="image" src="https://github.com/user-attachments/assets/9749e376-c0ff-488e-aa27-db61fcf3d463" />
<img width="281" height="24" alt="image" src="https://github.com/user-attachments/assets/a9773ee2-b0e4-45ec-b4c5-6dcadc617405" />

<img width="182" height="25" alt="image" src="https://github.com/user-attachments/assets/3df50d52-9f22-4390-970c-577b5b2f84af" />




## Result:
Thus the program to implement the Decision Tree Regressor Model for Predicting the Salary of the Employee is written and verified using python programming.
