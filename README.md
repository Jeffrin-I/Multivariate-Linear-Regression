# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step 1:  Import the required libraries such as Pandas and Scikit-learn to handle data and perform linear regression.
<br>

### Step 2: Read the cars.csv file using Pandas and store it in a dataframe.
<br>

### Step 3: Select Weight and Volume as independent variables (X) and CO2 as the dependent variable (y).
<br>

### Step 4: Create a linear regression model and train it using the dataset with the fit() function.
<br>

### Step 5: Then use the trained model to predict the CO2 emission and display the result.
<br>

## Program:
```
# Developed by: JEFFRIN I
# Register No: 212225240060

import pandas as pd
from sklearn import linear_model
df=pd.read_csv("car (1).csv")
x=df[["Volume","Weight"]]
y=df["CO2"]
regression=linear_model.LinearRegression()
regression.fit(x,y)
print(regression.coef_)
print(regression.intercept_)
print(regression.predict([[3300,1300]]))
```

## Output:
<img width="1911" height="912" alt="Screenshot 2026-03-20 202928" src="https://github.com/user-attachments/assets/27209412-7fd8-4613-9bc0-1240808e2d2b" />

## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
