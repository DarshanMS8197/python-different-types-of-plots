# python-pychart

#creation of pychart using python code
#import library

from matplotlib import pyplot as plt

slices = [30, 40, 20, 50]

#sum needs not be 100
plt.pie(slices)
plt.show()
labels = ['thirty','fourty', 'twenty','fifty']
plt.pie(slices, labels=labels)
plt.show()

#setting edge color
plt.pie(slices, labels=labels, wedgeprops={'edgecolor':'black'})
plt.show()

# setting color of the slices
color = ['blue','red','yellow','green']

#hexadecimal color codes can also be used
plt.pie(slices, labels=labels, colors=color, wedgeprops={'edgecolor':'black'})
plt.show()

#plotting real world data
labels = ['JavaScript', 'HTML/CSS', 'SQL', 'Python', 'Java']
slices = [59219, 55466, 47544, 36443, 35917]
plt.pie(slices, labels=labels, wedgeprops={'edgecolor':'black'})
plt.show()

#Exploding the slice
explode = [0, 0, 0, 0.1, 0]
plt.pie(slices, labels=labels, explode=explode, wedgeprops={'edgecolor':'black'})
plt.show()

# adding shadow to the chart
plt.pie(slices, labels=labels, explode=explode, shadow=True, wedgeprops={'edgecolor':'black'})
plt.show()

# displaying percentage of each slices
plt.pie(slices, labels=labels, explode=explode, shadow=True, startangle=60, autopct="%0.1f%%", wedgeprops={'edgecolor':'black'})
plt.show()
