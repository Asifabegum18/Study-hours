# Study-hours
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_absolute_error
data=pd.read_csv('http://bit.ly/w-data')
print("Data is pubished")

#Print the first 10 values
data.head(10)

#Check there is any null value
data.isnull==True
sns.set_style('darkgrid')
sns.scatterplot(y=data['Scores'], x=data['Hours'])
plt.title("Marks vs Study Hours", size=20)
plt.ylabel("Marks Percentage",size=12)
plt.xlabel("Hours studied",size=12)
plt.show()
