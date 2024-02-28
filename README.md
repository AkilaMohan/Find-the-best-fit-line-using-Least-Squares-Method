/*
Program to implement univariate Linear Regression to fit a straight line using least squares.
Developed by: Ajay K
RegisterNumber: 212222080005
import numpy as np
import matplotlib.pyplot as plt
x=np.array(eval(input()))
y=np.array(eval(input()))
#mean
xmean=np.mean(x)
ymean=np.mean(y)
num,den=0,0 # for slope
# to find slope
for i in range(len(x)):
  num+=(x[i]-xmean)*(y[i]-ymean)
  den+=(x[i]-xmean)**2
m=num/den
c=ymean-m*xmean
print("slope",m,"\n")
print("y-intercept",c,"\n")
y_pred=m*x+c
print(y_pred,"\n")
plt.scatter(x,y)
plt.plot(x,y_pred,color="green")
plt.show() 
*/
