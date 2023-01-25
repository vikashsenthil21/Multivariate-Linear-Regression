# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Get the independent variable X and dependent variable Y.

### Step 2
Calculate the mean of the X -values and the mean of the Y -values.
### Step3
Find the slope m of the line of best fit using the formula

### Step4
Compute the y -intercept of the line by using the formula:

### Step5
Use the slope m and the y -intercept to form the equation of the line.

## Program:
```
#Developed by :vikash s
#Register number:22008879
import pandas as pd
from sklearn import linear_model

df = pd.read_csv('carsemision.csv')
X = df[['Weight','Volume']]
y = df['CO2']
regr = linear_model.LinearRegression()
regr.fit(X,y)
print("Cofficients: ",regr.coef_)
print("Intercept: ",regr.intercept_)
predictedCO2 = regr.predict([[3300,1300]])
print('Predicted co2 for the corresponding weight and volume',predictedCO2)






```
## Output:

### Insert your output
![WhatsApp Image 2023-01-24 at 21 49 23](https://user-images.githubusercontent.com/119433834/214365262-3e8bc0fe-e843-4c88-b63d-52f2bc6e6be0.jpg)


## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
