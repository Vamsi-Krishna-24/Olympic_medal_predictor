# Olympic_medal_predictor
Employing regression modeling, this project predicts a country's medals in sports events based on historical data. Cleaned and prepared datasets are used to train and optimize the model. Insights gained from the predictive analysis aid athletes and stakeholders in strategizing for upcoming competitions.

#Importing libraries necessary
import pandas as pd
import numpy as np

#reading the data sets and naming it.
teams = pd.read_csv("/Users/surisettivamsikrishna/Downloads/Projects /Olympic data sets /teams.csv")
teams

#knowing the data types
teams.dtypes

#removing the null values
teams=teams.drop(columns=['height','weight'],axis=1)
teams.dropna()
teams

#data visualisation to check whether the data makes sense 
import seaborn as sns
sns.lmplot(x='athletes',y='medals',data=teams,fit_reg=True, ci= None)
sns.lmplot(x='age',y='medals',data=teams,fit_reg=True, ci= None)

#importing libraries to train data set, here as the problem is simple and relation is between two variables, linear regression is used
from sklearn.linear_model import LinearRegression
reg = LinearRegression()

#Training and testing the data sets
predictors = ["athletes","prev_medals"]
target = 'medals'

#Fitting the data into the model and testing 
reg.fit(train[predictors],train["medals"])
test['predictions']=predictions

test['predictions']=test['predictions'].round()


#checking the error calculation of our model
from sklearn.metrics import mean_absolute_error
error=mean_absolute_error(test['medals'],test['predictions'])

#If the error popping is less then the deviation then the model is saod to be a good working model or else there is a mistake either in data sets or else in the code.
