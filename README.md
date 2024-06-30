# Boston house price prediction

## Installation Guide
1. Clone or Fork the Project
2. Create a Virtual Enviroment
3. go to same virtual enviroment and write below cmd
4. pip install -r requirements.txt


### 1. Project Description
#### A. Problem Statement

Thousands of houses are sold everyday. There are some questions every buyer asks himself like: What is the actual price that this house deserves? Am I paying a fair price?

#### B. Tools and Libraries
Tools<br><br>
a.Python<br>
b.Jupyter Notebook<br>
c. Flask<br>
d. HTML<br>
e. Render
f. GitHub

Libraries<br><br>
a.Pandas<br>
b.Scikit Learn<br>
c.Numpy<br>
d.Seaborn<br>
e.Matpoltlib<br>

### 2. Data Collection
For this project we used the data that is available on sklearn itself(from sklearn.datasets import load_boston)
There are 13 columns and 506 Rows. These are the major point about the data set.<br>
CRIM: per capita crime rate by town<br>
ZN: proportion of residential land zoned for lots over 25,000 sq.ft.<br>
INDUS: proportion of non-retail business acres per town<br>
CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)<br>
NOX: nitric oxides concentration (parts per 10 million)<br>
RM: average number of rooms per dwelling<br>
AGE: proportion of owner-occupied units built prior to 1940<br>
DIS: weighted distances to five Boston employment centres<br>
RAD: index of accessibility to radial highways<br>
TAX: full-value property-tax rate per 10,000usd<br>
PTRATIO: pupil-teacher ratio by town<br>
B: 1000(Bk - 0.63)^2 where Bk is the proportion of blacks by town<br>
LSTAT: % lower status of the population<br>

Target Column is Price which is specified as
MEDV: Median value of owner-occupied homes in $1000s<br>
If MEDV is 24.0 for a particular area (or observation in the dataset), it means that the median value of all the owner-occupied homes in that area is $24,000. This value is derived from actual housing prices and is intended to give a single, representative value for the home prices in that area.

### 3. EDA
#### A.Data Cleaning
We have 13 columns and no column contain any null values<br>
All columns are numerical also

#### B. Feature Engineering
No outiers are present in the data

#### C. Data Normalization
Normalization (min-max Normalization)<br>
In this approach we scale down the feature in between 0 to 1

we have numerical column where we can apply min-max Normalization.<br>

### 4. Choosing Best ML Model
List of the model that we can use for our problem<br>
a. LinearRegression model<br>
b. KNN Model<br>
c. Decesion Tree<br>
d. Random Forest

### 5. Model Creation
So,using a RandomForest we got good accuracy , we can Hyperparameter tuning  for best accuracy.

Algorithm that can be used for Hyperparameter tuning are :-

a. GridSearchCV<br>
b. RandomizedSearchCV<br>

Main parameters used by RandomForest Algorithm are :-

a. n_estimators --->    The number of trees in the forest.<br>
b. criterion--->{"mse", "mae"}-->The function to measure the quality of a split<br>
c. max_features--->{"auto", "sqrt", "log2"}-->    The number of features to consider when looking for the best split:


So, After Hyperparameter Tuning we got 90 % accuracy on test data and 94 % accuracy on train data. 

### 6. Model Deployment
After creating model ,we integrate that model with beautiful UI. for the UI part we used HTML and Flask. We have added extra validation check also so that user doesn't enter Incorrect data

### 7. Model Conclusion

Model predict 90% accurately on test data and 94% accurately on train data .

### 8. Project Innovation
a. Easy to use<br>
b. Open source<br>
c. Best accuracy<br>
d. GUI Based Application

### 9. Limitation And Next Step
Limitation are :-<br>
a. Mobile Application<br>
b. Accuracy can be improved more<br>
c. Model Size is heavy(~310 mb )<br>
d. Feature is limited

Next Step are :-<br>
a. we will work on mobile application<br>
b. we will reduce the size of model using PCA .

## Deployable Link
https://machine-learning-practical-assignment-01.onrender.com/predict