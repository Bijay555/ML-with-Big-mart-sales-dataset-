# ML-with-Big-mart-sales-dataset-
This repository consists of some machine learning feature engineering with big mart sales prediction dataset and try to understand it through linear regression and polynomial regression of degree 2,3 and 4

Some thing About the working model:

# Model Building
In model building we use two models. One is
# Linear Regression:
Linear Regression is a machine learning algorithm based on supervised learning. Linear regression performs the task to predict a dependent variable value (y) based on a given independent variable (x). So, this regression technique finds out a linear relationship between x (input) and y(output).
Hypothesis function for Linear Regression :
			y=  θ1 + θ2*x
			
While training the model we are given :

x: input training data (univariate – one input variable(parameter))
y: labels to data (supervised learning)
When training the model – it fits the best line to predict the value of y for a given value of x. The model gets the best regression fit line by finding the best θ1 and θ2 values.
θ1: intercept
θ2: coefficient of x
Once we find the best θ1 and θ2 values, we get the best fit line. So when we are finally using our model for prediction, it will predict the value of y for the input value of x

Cost Function:
By achieving the best-fit regression line, the model aims to predict y value such that the error difference between the predicted value and the true value is minimum. So, it is very important to update the θ1 and θ2 values, to reach the best value that minimize the error between predicted y value (pred) and true y value (y).			
 
# Polynomial Regression:
Polynomial Regression is a form of linear regression in which the relationship between the independent variable x and dependent variable y is modeled as an nth degree polynomial. Polynomial regression fits a nonlinear relationship between the value of x and the corresponding conditional mean of y, denoted E(y |x)

So when the dataset is not linear, linear regression cannot learn the dataset and make good predictions.
So we need a polynomial model which considered the polynomial terms as well. So we need terms like x, x^2, x^3, x^4 ….. etc
y = a + b1x + b2x^2 +....+ bnx^n

Advantage over linear regression
●	Broad range of function can be fit under it.
●	Polynomial basically fits wide range of curvature.
●	Polynomial provides the best approximation of the relationship between dependent and independent variable.
One down side of this model is that, We will have to decide the value of n. But this is better than a linear regression model. We can get an idea of the value of n by visualizing a dataset, but for multi variable dataset, we will have to try different values of n and check which is better.

you can calculate the polynomial features for each feature by programming it or you can try sklearn.preprocessing.PolynomialFeatures which allows us to make polynomial terms of our data.
We will try degree 2, 3 and 4

