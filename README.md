# Data-Visualisation-using-Charts 

## Install matplotlib for creating charts and graphs in python
pip install matplotlib

## Creating a small sample of countries and their GDP per capita 
Country = ['USA', 'Canada', 'Germany', 'UK', 'France']
GDPPerCapita = [45000, 42000, 52000, 49000, 47000]

# Column Chart 
## Creating a column chart in python using matplot
import matplotlib.pyplot as plt

plt.bar(Country, GDPPerCapita)
plt.title('GDP of Countries')
plt.xlabel('Country')
plt.ylabel('GDP Per Capita')
plt.show()

![download1](https://user-images.githubusercontent.com/90278106/136889182-c30b0fa2-ec2a-4f41-a3b9-4ff3aa81ea1c.png)

## To modify the Column Chart let's add some colors and grids to it 
import matplotlib.pyplot as plt
   
Country = ['USA','Canada','Germany','UK','France']
GDPPerCapita = [45000,42000,52000,49000,47000]

New_Colors = ['green','blue','purple','brown','teal']
plt.bar(Country, GDPPerCapita, color=New_Colors)
plt.title('Country Vs GDP Per Capita', fontsize=14)
plt.xlabel('Country', fontsize=14)
plt.ylabel('GDP Per Capita', fontsize=14)
plt.grid(True)
plt.show()
![download1](https://user-images.githubusercontent.com/90278106/136889266-5a300ef7-d913-4866-b2a5-1bae87fb50f3.png)

# Bar Chart 
## In case their is alot of data which can not be represented well in vertical columns 
## A good way to present them is using Bar Charts which are horizontal in nature

import matplotlib.pyplot as plt
   
Country = ['USA','Canada','Germany','UK','France','India', 'China']
GDPPerCapita = [45000,42000,52000,49000,47000,25000,38000]

New_Colors = ['green','blue','purple','brown','teal', 'orange', 'red']
plt.barh(Country, GDPPerCapita, color=New_Colors)
plt.title('Country Vs GDP Per Capita', fontsize=14)
plt.ylabel('Country', fontsize=14)
plt.xlabel('GDP Per Capita', fontsize=14)
plt.grid(True)
plt.show()

![download3](https://user-images.githubusercontent.com/90278106/136889361-9032f31c-d42d-4f64-8e4b-cd4b0c4dc243.png)

# Volumn Width Column Chart
## Let's try to work on Volumn Width Column Charts on some simple data
import matplotlib.pyplot as plt
Name = ['Ryan', 'Gerald', 'Heather', 'Krish']
Earnings = [5000, 2800, 7550, 3500] 
w = [0.8, 0.2, 1.1, 0.5 ]

plt.bar(Name, height = Earnings, width = w)
New_Colors = ['green','blue', 'brown', 'orange']
plt.bar(Name, Earnings, color=New_Colors)
plt.title('Earnings per Person', fontsize=14)
plt.ylabel('Name', fontsize=14)
plt.xlabel('Earnings', fontsize=14)
plt.show()

![download5](https://user-images.githubusercontent.com/90278106/136889476-ddbec230-9f92-4c1d-9369-9db976644d45.png)
