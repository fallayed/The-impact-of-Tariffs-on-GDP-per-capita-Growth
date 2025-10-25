# The-impact-of-Tariffs-on-GDP-per-capita-Growth
What is the impact of tariffs on the U.S economy?
Tariffs have become a big economic discussion point, to really understand impacts of Tariffs on the economy I have analyzed the US GDP growth from 2000 to 2024. There are different metrics that have also been impacted by the use of tariffs through the years such as Unemployment, and Inflation rate. The relations between these metrics is important

# Libraries Used:

import pandas as pd   #Library for Data manipulation and Analysis

import numpy as np    #Library for Data manipulation

import matplotlib.pyplot as plt #Library for Data visualization

import seaborn as sns  #Library for data visualization

from sklearn import metrics #Library for Models score

from sklearn.model_selection import train_test_split #Splitting the data into training and test set

from sklearn.model_selection import train_test_split #Splitting the data into training and test set

from sklearn.tree import plot_tree  # plot the decision tree

from sklearn.model_selection import KFold, cross_val_score #Lets bring in the cross validation function to improve the score

import xgboost as xgb #lets import the xgboost model library

from xgboost import XGBClassifier #lets import the XGBclassifir

#Libraries to get different metric scores
from sklearn import metrics
from sklearn.metrics import (
    confusion_matrix,
    accuracy_score,
    precision_score,
    recall_score,
    f1_score,
)




# Libraries installed
%pip install sklearn  #Lets install Sklearn

%pip install Xgboost  #lets install Xgboost
