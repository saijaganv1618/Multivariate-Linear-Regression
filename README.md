# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
Import pandas as pd.

### Step2
Import Linear model from sklearn

### Step3
Read the file cars.csv.

### Step4
Assign the values for x and y as required and create the linear regression model.

### Step5
Predict the output.

## Program:
```
import pandas as pd
from sklearn import linear_model
df=pd.read_csv("cars.csv")
x=df[['Weight','Volume']]
y=df['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print("Coefficient:",regr.coef_)
print("Intercept:",regr.intercept_)
predictedCO2=regr.predict([[3300,1300]])
print("Predicted CO@ for the corresponding weight and volume",predictedCO2)

```
## Output:
![WhatsApp Image 2022-02-14 at 2 00 46 PM](https://user-images.githubusercontent.com/59290560/153830857-08ff0283-7b5b-4217-a55a-fd3baefdee23.jpeg)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.
