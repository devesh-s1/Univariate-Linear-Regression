# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1.	Get the independent variable X and dependent variable Y.
2.	Calculate the mean of the X -values and the mean of the Y -values.
3.	Find the slope m of the line of best fit using the formula.
 ![eqn1](./eq1.jpg)
4.	Compute the y -intercept of the line by using the formula:
![eqn2](./eq2.jpg)  
5.	Use the slope m and the y -intercept to form the equation of the line.
6.	Obtain the straight line equation Y=mX+b and plot the scatterplot.
## Program
```

# Program for Multivariate linear regression using the least squares method.
# Developed by: S.dvesh sharma
# RegisterNumber:22005350
import pandas as pd
from sklearn import linear_model
data=pd.read_csv("cars1.csv")
x=data[['Weight','Volume']]
y=data['CO2']
regr=linear_model.LinearRegression()
regr.fit(x,y)
print('coefficient: ',regr.coef_)
print('Intercept: ',regr.intercept_)
predictCO2=regr.predict([[3300,1300]])
print('Predicted CO2 fot the corresponding weight and volume',predictCO2)





```
## Output
![univariate](https://user-images.githubusercontent.com/121490523/215452905-55fe7443-ac84-4aa6-8800-31ed32a3ef63.png)


## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
