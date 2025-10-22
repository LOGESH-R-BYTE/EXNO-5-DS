# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

import numpy as np

import matplotlib.pyplot as plt

from scipy.interpolate import make_interp_spline

import pandas as pd

x_values=[1,2,3,4,5]

y_values=[1,4,9,16,25]

plt.plot(x_values,y_values,color="#e75480",linestyle="solid",marker="s",markersize=12,linewidth=5,markerfacecolor="blue")

plt.legend("line1")

plt.xlabel("X axis")

plt.ylabel("Y axis")

plt.title('Squares') 

plt.grid(True)

plt.show()


<img width="824" height="591" alt="image" src="https://github.com/user-attachments/assets/ad4638d7-5bf3-4fc8-9746-8dbfa8847827" />


x=np.arange(1,11)

y=np.array([2,3,5,7,8,8,9,10,11,12])

spl=make_interp_spline(x,y)

x_smooth=np.linspace(x.min(),x.max(),100)

y_smooth=spl(x_smooth)

plt.plot(x,y,'o',label='data')

plt.plot(x_smooth,y_smooth,'-',label='spline')

plt.legend()

plt.show()


<img width="814" height="603" alt="image" src="https://github.com/user-attachments/assets/7032a6da-bd24-4891-92d4-606d80df4f35" />



years=[i for i in range(2000,2007)]

apples=[0.895,0.91,0.919,0.926,0.931,0.934,0.936]

oranges=[0.962,0.950,0.934,0.926,0.911,0.898,0.891]

plt.plot(years,apples,marker='o')

plt.plot(years,oranges,marker='s')

plt.xlabel("Years")

plt.title("Crop Yield in Kanto")

plt.ylabel("Yield(Tons per hectare)")

plt.legend(["Apples","Oranges"])


<img width="818" height="577" alt="image" src="https://github.com/user-attachments/assets/61decd3c-d0e8-404a-bb01-0b7ebce58a8c" />


x=[1,2,3,4,5]

y1=[10,12,14,16,18]

y2=[5,7,9,11,13]

y3=[2,4,6,8,10]

plt.fill_between(x,y1,color="blue")

plt.fill_between(x,y2,color="green")

plt.plot(x,y1,color='red')

plt.plot(x,y2,color='black')

plt.legend(['area1','area2'])


<img width="820" height="599" alt="image" src="https://github.com/user-attachments/assets/c3805b29-abcb-45a2-b458-c836a54a93a3" />


values=[5,6,3,7,2]

names=["A","B","C","D","E"]

c1=['green','yellow','black']

plt.bar(names,values,color=c1,edgecolor='red')

plt.xlabel("Names")

plt.ylabel("Values")

plt.title("Starting letter of names")

plt.show()

<img width="822" height="625" alt="image" src="https://github.com/user-attachments/assets/9cbdfae9-01fe-4f52-9c7d-c80fd7d91619" />


x=np.arange(1,11)

y=np.array([2,3,5,7,8,8,9,10,11,12])

plt.scatter(x,y,label='stars',color='green',marker='*',s=200)

plt.xlabel("x-axis")

plt.ylabel("y-axis")

plt.title("My scatter plot")

plt.legend()

plt.show()


<img width="828" height="600" alt="image" src="https://github.com/user-attachments/assets/41e7a284-1ab6-431f-8988-588b00518581" />


activities=['eat','sleep','work','play']

slices=[3,7,8,6]

colors=['r','y','g','b']

plt.pie(slices,labels=activities,colors=colors,startangle=90,

    shadow=True,explode=(0,0,0.1,0),
       
    radius=1.2,autopct="%1.1f%%")
       
plt.legend(loc='upper left')

plt.show()



<img width="811" height="619" alt="image" src="https://github.com/user-attachments/assets/cae950ec-4114-441c-a94f-0881c9a9b99c" />

# Result:

Thus we have performed data visualisation using matplotlib library

 
