# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
# Step1:
Importing pandas and scikit-learn libraries.

# Step2:
Reading the data from a CSV file.

# Step3:
Splitting the data into features (X) and target (y).

# Step4:
Creating and fitting the linear regression model.

# Step5:
Printing the coefficients and intercept of the linear regression model.

# Step6:
Making a prediction.

# Step7:
Printing the predicted CO2 emissions.

## Program:
```
#Program to implement multivariate linear regression and predict the output
#Devloped by : Vinnush Kumar L S
#Register no : 23012349
import pandas as pd 
from sklearn import linear_model
data=pd.read_csv("cars (1).csv")
x=data[['Weight','Volume']]
y=data[['CO2']]
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('Coeffients:',regr.coef_)
print('Intercept:',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('predicted CO2 for the corresponding weight and volume',predictCO2)

```
## Output:
![image](https://github.com/vinnush147/Multivariate-Linear-Regression/assets/147139234/037a159f-cdd4-40b0-922d-43a23d799143)

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
