# Implementation of Multivariate Linear Regression:
## Aim:
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1:
Import pandas.

### Step2:
Impor linear model from sklearn.

### Step3:
Read the files cars.csv.

### Step4:
Assign he values for x and y as requried.

### Step5:
Create the LinearRegression model and predic he output

## Program:

Developed by: MAMTHA I

RegisterNumber: 2122222300076

```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv('/content/cars.csv')
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO2 for the corresponding weight and volume",predictedCO2)
```
## Output:

![Screenshot 2023-06-08 155051](https://github.com/Mamthaiyappaprabu/Multivariate-Linear-Regression/assets/119393563/5436b9e4-7119-41f5-93c1-394be5faa792)

## Result:
Thus the multivariate linear regression is implemented and predicted the output using python program.
