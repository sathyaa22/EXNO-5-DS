# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## NAME: SATHYAA R
## REG NO: 212223100052

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

```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
```
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
```
```
plt.plot(x,y,label='line1')
```

![image](https://github.com/user-attachments/assets/16613192-843c-4dd8-bc1c-100d2bf531bc)

```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]
```
```
plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/c60dfb25-6ee6-4f39-b77d-42e0ebd7045b)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```

![image](https://github.com/user-attachments/assets/ac152b6f-09d7-4e8a-bc90-9496f41b236c)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![image](https://github.com/user-attachments/assets/f8ea9468-01ea-432a-918e-edf9b7790107)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![image](https://github.com/user-attachments/assets/137bc1c7-886e-4a28-bac9-8a50fccb8b5b)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```

![image](https://github.com/user-attachments/assets/437558ce-df82-4b86-8539-e950a22854c1)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```

![image](https://github.com/user-attachments/assets/4177b95e-c867-4aa9-9abc-50c5b61d9b20)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

![image](https://github.com/user-attachments/assets/84a5b7a7-59b1-4a39-99c1-04aca9547f21)

```
y
```

![image](https://github.com/user-attachments/assets/4351944d-a4c9-402d-b712-80262cdf202d)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```

![image](https://github.com/user-attachments/assets/f12ea980-c418-4989-af47-587d3e1f0c2b)

```
y=x*x
y
```

![image](https://github.com/user-attachments/assets/db7d50a2-ef43-4080-9f10-0ef8c89e92cc)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```

![image](https://github.com/user-attachments/assets/8f887b0e-3fd4-4807-9c43-c7875c83dd59)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```

![image](https://github.com/user-attachments/assets/350b8054-c576-41fb-ad7e-e0478f87f9ab)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='beige')
plt.fill_between(x,y2,color='brown')
```

![image](https://github.com/user-attachments/assets/b2e2974c-1e68-4335-910a-caa3ed9743bc)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='yellow')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```

![image](https://github.com/user-attachments/assets/d152ea0e-eb57-406f-9ed9-a575d8d51476)

```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['aqua','pink']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```

![image](https://github.com/user-attachments/assets/cb00e068-9317-4225-8d82-39badc8158d6)

```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='b')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```

![image](https://github.com/user-attachments/assets/358267b3-6d37-443b-bd5e-f3d22dc4dc96)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='m',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```

![image](https://github.com/user-attachments/assets/12b6175c-63f4-4f73-934f-7b0b7589cc57)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![image](https://github.com/user-attachments/assets/d208345a-7d66-4288-aa8e-0c81ac29211a)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

![image](https://github.com/user-attachments/assets/82ff5edc-1242-4509-a050-1070745de8ea)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![image](https://github.com/user-attachments/assets/ce6160ff-fe60-4dfc-92f3-ae42d36e9e43)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['y','aqua','g','m']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```

![image](https://github.com/user-attachments/assets/4b7c66e8-8ef6-442f-823b-51b460138145)


# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
