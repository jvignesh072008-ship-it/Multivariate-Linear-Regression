# Implementation of Multivariate Linear Regression

## Aim
To write a python program to implement multivariate linear regression and predict the output.

## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner.
   
## Algorithm:

### Step1:Import Libraries: The necessary libraries, pandas for data manipulation and LinearRegression from sklearn.linear_model for the regression model, are imported into the program environment.

### Step2:Load Data: The dataset is loaded from a CSV file named car (1).csv into a pandas DataFrame.

### Step3:Define Variables: The data is split into independent variables (features) x, which consist of the Volume and Weight columns, and the dependent variable (target) y, which is the CO2 column.

### Step4:Initialize and Train Model: An instance of the LinearRegression model is created and then trained (fitted) using the independent variables (x) and the dependent variable (y) from the loaded data. During this step, the model calculates the optimal coefficients and intercept that best fit the data.

### Step5:Output Model Parameters: The program prints the calculated coefficients (regression.coef_) and the intercept (regression.intercept_) of the fitted regression line.

### Step6:Make and Print Prediction: The trained model is used to predict the CO2 value for a new data point (volume of 3300 and weight of 1300), and the resulting prediction is printed to the console. 


## Program:
```
import pandas as pd
from sklearn.linear_model import LinearRegression
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```
```
program developed by vignesh j and reg.no 212225230297
```

## Output:
```
[0.00780526 0.00755095]
79.6947192911594
[115.26830058]
```

### Insert your output

<img width="1372" height="383" alt="Screenshot 2026-03-17 111030" src="https://github.com/user-attachments/assets/e78bd347-dc9d-406b-bc67-5c0bd63527e7" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
