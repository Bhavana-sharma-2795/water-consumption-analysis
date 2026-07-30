import pandas as pd

import matplotlib.pyplot as plt

from sklearn.model\_selection import train\_test\_split

from sklearn.linear\_model import LinearRegression




data = pd.read\_csv("water\_usage.csv")

data.head()


X = data\[\['People','Temperature']]

y = data\['Water\_usage']






X\_train, X\_test, y\_train, y\_test = train\_test\_split(X,y,test\_size=0.2)







data.isnull().sum()



data = data.dropna()


data.isnull().sum()



