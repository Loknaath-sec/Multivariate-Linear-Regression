# Implementation of Multivariate Linear Regression
## Aim:
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import necessary libraries: Bring in pandas for data manipulation and sklearn's linear_model for regression.
### Step2
Load and prepare data: Read car data from 'cars.csv', extract 'Weight' and 'Volume' as features (a), and 'CO2' as the target variable (b).

### Step3
Create and train model: Build a linear regression model and train it using the prepared data (a and b).

### Step4
Predict CO2: Use the trained model to predict CO2 emission for a car with weight 3300 and volume 1300.

## Program:
```
# Developed by : P.LOKNAATH
# Register Number : 212223240080
 
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("coefficient",regr.coef_)
print("Intercept:",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))


```
## Output:
![1](https://github.com/Loknaath-sec/Multivariate-Linear-Regression/assets/145742558/41b0ce3f-c002-445c-9e67-78a43a36a4cb)
![2](https://github.com/Loknaath-sec/Multivariate-Linear-Regression/assets/145742558/899c767a-3125-4284-8cd1-ea17e753e8f1)

![3](https://github.com/Loknaath-sec/Multivariate-Linear-Regression/assets/145742558/17fcea4b-d2c6-4357-b25b-e23d50958fe7)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
