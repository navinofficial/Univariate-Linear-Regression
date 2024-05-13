### Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
![image](https://github.com/navinofficial/Univariate-Linear-Regression/assets/151710204/3108d9c2-8e72-496f-a3a5-dd518f78386e)
## Program
#Developed by:Navinkumar v
#register number: 212223230141
```
import numpy as np 
import matplotlib.pyplot as plt
x = np.array([0,1,2,3,4,5,6,7,8,9])
y = np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean = np.mean(x)
ymean = np.mean(y)
num=0
den=0
for i in range(len(x)):
    num+=(x[i]-xmean)*(y[i]-ymean)
    den+=(x[i]-xmean)**2
m = num/den
b = ymean - m*xmean
print(m,b)
ypred = m*x+b
print(ypred)
plt.scatter(x,y,color='Red')
plt.plot(x,ypred,color='Blue')
plt.show()
```
## Output
![image](https://github.com/navinofficial/Univariate-Linear-Regression/assets/151710204/b61bc420-d424-46f5-9417-94507746d6ae)
## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
