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
\*
# Program to find univariate linear regression
# Developed by: V. Yogesh
# Register number: 212223230250
\*
import numpy as np
import matplotlib.pyplot as plt
x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
x_mean=np.mean(x)
y_mean=np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-x_mean)*(y[i]-y_mean)
    den+=(x[i]-x_mean)**2
m=num/den
b=y_mean-m*x_mean
print(m,b)
y_pred=m*x+b
print(y_pred)
plt.scatter(x,y,color="Red")
plt.plot(x,y_pred,color="Blue")
plt.show
```
## Output
![Screenshot 2024-01-02 192602](https://github.com/Yogesh-Yogi-1/Univariate-Linear-Regression/assets/148514598/fb05fafe-b5e8-4223-9d6d-521585a36b2d)
![Screenshot 2024-01-02 191919](https://github.com/Yogesh-Yogi-1/Univariate-Linear-Regression/assets/148514598/675dbd2d-6b55-4f24-b061-c94b5f2fad29)
![Screenshot 2024-01-02 191948](https://github.com/Yogesh-Yogi-1/Univariate-Linear-Regression/assets/148514598/5116d26e-97fa-4d92-a859-49030502009c)

</br>
</br>
</br>
</br>

## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
