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
```
Developed By : Prasannalakshmi G
Reg No : 212222240075
```
### Simple two lines
```python
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[1,4,1]
plt.plot(x1,y1, label="line 1", color="maroon", linewidth=2)

x2=[1,2,3]
y2=[4,1,4]
plt.plot(x2,y2, label="line 2", color="black", linewidth=2)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on same graph")
plt.legend()
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/d67d8648-71f3-480a-acaa-c1ca36bf825b)

### Customization of plots
```python
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x, y, color='green', linestyle='dashed', linewidth = 3, marker='o', markerfacecolor='blue', markersize=12)

plt.xlim(1,8)
plt.ylim(1,8)

plt.xlabel('x - axis')
plt.ylabel('y - axis')

plt.title('Some cool customizations!')
plt.show()
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/83f8ab1f-5553-4f33-853c-f1a6b642a50b)


### Implementation using Matplotlib
```python
yield_orange=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(yield_orange, color='sienna', linewidth=3)
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/3c50f2d7-b836-47dd-83d5-2bce865dfd3d)


```python
years= [2010, 2011, 2012, 2013, 2014, 2015]
yield_apples=[0.895, 0.91, 0.919, 0.926, 0.929, 0.931]
plt.plot(years, yield_apples, color='chocolate', linewidth=3)
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/98dd1e0c-69ed-433d-832d-a5d4ed419810)


```python
years = range(2000, 2012) 
apples = [0.895, 0.91, 0.919, 0.926, 0.929, 0.931, 0.934, 0.936, 0.937, 0.9375, 0.9372, 0.939]
oranges = [0.962, 0.941, 0.930, 0.923, 0.918, 0.908, 0.907, 0.904, 0.901, 0.898, 0.9, 0.896, ] 
 
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)'); 


plt.plot(years, apples)
plt.plot(years, oranges)

plt.xlabel( 'Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend(['Apples', 'Oranges'])
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/7f0eb919-9dd1-457e-8c2c-4e9ef60c86f3)


```python
plt.figure(figsize=(12, 6))
plt.plot(years, oranges, marker='o')
plt.title("vield of Oranges (tons per hectare)") 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/9b5f0950-eb2f-4cb4-bb4e-5e6019e60e8d)


```python
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker="x")
plt.xlabel('Year') 
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yields in Kanto")
plt.legend([ 'Apples', 'Oranges']) 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/2246215a-f424-43a1-a773-62991aea6559)


### Scatter Plot
```python
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.scatter(x_values, y_values,s=30, color="blue") 
plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/bcfcb2e8-4ed1-4cad-bb0d-bd647a600aea)

```python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/43e28f7f-4de4-4c12-a853-08996e2bc385)

```python
plt.scatter(x,y,c="r")
plt.xlabel( 'X axis')
plt.ylabel('Y axis')
plt.title( 'Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/965891d9-5d6d-418f-9502-9bfb4c058c7f)

![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/26f95676-fe1a-4133-9515-eff91333a120)


```python
plt.plot(x,y, 'g*',linestyle='dashed' ,linewidth=2, markersize=12)
plt.xlabel( 'X axis') 
plt.ylabel( 'Y axis')
plt.title('2d Diagram') 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/052dce90-be7d-4749-8e79-3b5bf1049c83)


```python
x = np.arange(0, 4 * np.pi, 0.1) 
y= np.sin(x)
plt.title('sine wave form')
plt.plot(x, y)
plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/004fe020-753d-4f74-9bdc-63868a2e210d)


### Area Chart
```python
import matplotlib.pyplot as pit
import numpy as np
x=[1,2,3,4,5]
y1=[10, 12, 14, 16, 18]
y2=[5,7,9, 11, 13]
y3=[2,4,6,8,10]
pit.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green') 
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/c23aa4bd-d828-4ba7-95ad-0a401d23aaf3)


### Bar Chart
```python
import matplotlib.pyplot as plt

height = [10, 24, 36, 40, 5]
names = ['one','two"', 'three’', 'four', 'five']

c1 =['chocolate', 'darkgreen']
c2 =['skyblue', 'blue'] 
plt.bar(names, height, width=0.8, color=c1)

plt.xlabel('x - axis')

plt.ylabel('y - axis')

plt.title('My bar chart!')

plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/f437f77a-602f-4b37-bcbf-b8089c870ac3)


```python
x = [2,8,10]
y = [11,16,9]
x2 = [3,9,11]
y2 = [6,15,7] 
plt.bar(x, y,color='chocolate')
plt.bar(x2, y2, color = 'darkgreen')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/74f7521d-5e34-45db-acab-87926b68f917)


### Histogram
```python
import matplotlib.pyplot as plt

ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range = (0, 100)
bins = 10

plt.hist(ages, bins, range, color='darkgreen' , histtype='bar', rwidth=0.8)

plt.xlabel('age') 

plt.ylabel('No.Of.People')

plt.title('My Histogram')

plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/daa9282d-ed77-4afc-8738-5b4a0ba9c351)


### Box Plot
```python
import matplotlib.pyplot as plt
import numpy as np 

np.random.seed(0) 
data = np.random.normal(loc=0, scale=1, size=100)
data 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/074f18ee-7fe3-4034-ae23-b774c1a0b05b)


```python
fig, ax = plt.subplots() 
ax.boxplot(data) 
ax.set_xlabel('Data') 
ax.set_ylabel('values')
ax.set_title('Box Plot') 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/2e379507-db20-4c69-b144-1a5a082ddbb6)

### Pie Chart
```python
labels = 'Python', 'C++', 'Ruby', 'Java'
sizes = [215, 130, 245, 210]
colors = ['gold', 'yellowgreen', 'lightcoral', 'lightskyblue']
explode = (0, 0.4, 0, 0.5)

plt.pie(sizes, explode=explode, labels=labels, colors=colors, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show() 
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/b2af2b2d-546b-4708-8587-9b7445a15e05)

```python
activities = ['eat', 'sleep', 'work', 'play']

slices =[3,7,8,6]

colors=['r', 'y', 'g', 'b']

plt.pie(slices, labels = activities, colors=colors, startangle=90, shadow = True, explode = (0, 0, 0.1, 0), radius = 1.2, autopct = '%1.1F%%')

plt.legend()
```
![image](https://github.com/Prasannalakshmiganesan/EXNO-5-DS/assets/118610231/bee5e5ff-61f8-47f5-b7d4-edeff81a42d4)


# Result:
Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
