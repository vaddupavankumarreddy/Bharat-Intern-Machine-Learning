Housing_Price_Prediction_In_Beijing

Installation Guide

Clone or Fork the Project
Create a Virtual Enviroment
go to same virtual enviroment and write below cmd
pip install -r requirements.txt
Project Highlights

Research Paper
User Friendly
Accuracy
Open Source
Table Of Content

Project Descriptiom
A. Problem Statement
B. Best Possible Solutions
C. Introduction About Project
D. Tools and Libraries
Data Collection
Generic Flow Of Project
EDA
A. Data Cleaning
B. Feature Engineering
C. Data Normalization
Choosing Best ML Model
Model Creation
Model Deployment
Model Conclusion
Project Innovation
Limitation And Next Step
Working Project Video
1. Project Description

A. Problem Statement

Thousands of houses are sold everyday. There are some questions every buyer asks himself like: What is the actual price that this house deserves? Am I paying a fair price?

B. Best Possible Solutions

a.Housing Expert
b.Intuition About House
c.Using Machine Learning

C. Introduction About Project

House Price prediction are very stressful work as we have to consider different things while buying a house like the structure and the rooms kitchen parking space and gardens. People don’t know about the factor which influence the house price. But by using the Machine learning we can easily find the house which is to be prefect for us and helps to predict the price accurately.

D. Tools and Libraries

Tools

a.Python
b.Jupyter Notebook
c. Flask
d. HTML
e. CSS
f. JS
g. Heroku
h. GitHub

Libraries

a.Pandas
b.Scikit Learn
c.Numpy
d.Seaborn
e.Matpoltlib

2. Data Collection

For this project we used the data that is available on kaggle.(click here for data).There are 26 columns and 318851 Rows. These are the major point about the data set.
url: the url which fetches the data
id: the id of transaction
Lng: and Lat coordinates, using the BD09 protocol.
Cid: community id
tradeTime: the time of transaction
DOM: active days on market
followers: the number of people follow the transaction.
totalPrice: the total price
price: the average price by square
square: the square of house
livingRoom: the number of living room
drawingRoom: the number of drawing room
kitchen: the number of kitchen
bathroom the number of bathroom
floor: the height of the house. I will turn the Chinese characters to English in the next version.
buildingType: including tower( 1 ) , bungalow( 2 )，combination of plate and tower( 3 ), plate( 4 ).
constructionTime: the time of construction
renovationCondition: including other( 1 ), rough( 2 ),Simplicity( 3 ), hardcover( 4 )
buildingStructure: including unknow( 1 ), mixed( 2 ), brick and wood( 3 ), brick and concrete( 4 ),steel( 5 ) and steel-concrete composite ( 6 ).
ladderRatio: the proportion between number of residents on the same floor and number of elevator of ladder. It describes how many ladders a resident have on average.
elevator: have ( 1 ) or not have elevator( 0 )
fiveYearsProperty: if the owner have the property for less than 5 years.

3. Generic Flow Of Project



4. EDA



A.Data Cleaning

we have 26 columns ,from these we don't want some column(i.e. url,id,cid) then we will perform data cleaning wich involve following steps. our target variable is totalPrice
a. Impute/Remove missing values or Null values (NaN)
b. Remove unnecessary and corrupted data.
c. Date/Text parsing if required.


we handle NAN value using appropriate solutions.


DOM Column have more than 50% value are missing it's better to delete that column


some column have unique character. we solve these problem using split method and create seprate column for unique character.

We also have a categorical data we handle such kind of data using dummies variable concept. following are the columns which have categorical data.
a. renovationCondition
b. buildingStructure
c. buildingType
d. district
e. elevator
f. floor_type

