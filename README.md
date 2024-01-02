# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Start the program.

### Step2
Import pandas and from sklearn import linear_model.

### Step3
Read the csv file , declare and assign the variables.

### Step4
Use in built functions .LinearRegression() and .fit(),then print the required outputs.

### Step5
End the program.

## Program:
### Developed by : JOTHIKRISHNAA V
### Register Number : 212223100017
~~~python
import pandas as pd
from sklearn import linear_model

df=pd.read_csv('cars.csv')
a=df[['Weight','Volume']]
b=df[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(a,b)
print("co-efficient",regr.coef_)
print("Intercept",regr.intercept_)
print("Amount:",regr.predict([[3300,1300]]))
~~~
## Output:
![10](<Screenshot 2024-01-02 225601.png>)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.