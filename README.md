# Implementation of Multivariate Linear Regression
## Aim
To write a python program to implement multivariate linear regression and predict the output.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
### Step1
<br>Import panda

### Step2
<br>Import linear model for sklearn

### Step3
<br>Read the file cars.csv

### Step4
<br>Assign the values for x and y as required

### Step5
<br>Create the linear regression model and predict the output 

## Program:
```python
#Developed by: DHARSHINI S
#RegisterNumber: 23010890
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
![output](./MULTIVARIATE%20LINEAR%20REGRESSION.png)



## Result
Thus the multivariate linear regression is implemented and predicted the output using python program.