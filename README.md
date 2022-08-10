## Table of Content

1. [Problem Statement](#section1)<br>    
2. [Data Description](#section2)<br>
3. [Data cleaning](#section3)<br>
4. [Exploratory Data Analysis](#section4)<br>
5. [Training linear regression model](#section5)<br>
    - 5.1 [Splitting data into trainset and testset](#section501)<br>
    - 5.2 [Rescaling the features](#section502)<br>
    - 5.3 [Splitting into X_train and y_train on training dataset](#section503)<br>
6. [Testing Linear regression model](#section6)<br>

7. [Model evaluation](#section7)<br>

8. [Conclusion](#section8)<br>
    
## 1. Problem Statement

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

 

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.



-  Which variables are significant in predicting the price of a house, and
-  How well those variables describe the price of a house.

## 2. Data Description

   ##### You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for   management to understand the pricing dynamics of a new market.


### Conclusions

 __Optimal value of Lambda for Ridge Regression is 5__.
- __Optimal Value of Lambda for Lasso is 0.001__.
- Variables that play important role in predicting house price are.
 - GrLivArea, OverallQual , RoofMatl_WdShngl, BsmtFinSF1,Neighborhood_NoRidge ,MasVnrArea ,OverallCond,Neighborhood_NridgHt,Neighborhood_StoneBr,TotalBsmtSF 
  
  
  
  - __R-Squared Value__
  - Ridge Train : 0.892578
  - Ridge Test  : 0.881025
  - Lasso Train : 0.900947
  - Lasso Test  : 0.885886