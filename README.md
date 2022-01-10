# Task-1-The-Sparks-Foundation-data-science-and-Business-analytics
## Task Name :- Prediction using supervised ML
### Tasks to do
In this section, we will see how we can perform machine learning using R programming language , which can be used to implement regression functions.

In this machine learning task we will predict the score that a student is expected to get based upon the number of hours they studied.

Model involved in this is simple linear regression model as it involves just two variables- Hours( studied by student) and Scores(Scores obtained by student )

### 1) About the dataset 
data.frame:	25 obs. of  2 variables:

 $ Hours : num  2.5 5.1 3.2 8.5 3.5 1.5 9.2 5.5 8.3 2.7 ...

 $ Scores: int  21 47 27 75 30 20 88 60 81 25 ...
 
####  dataset has 25 observations and 2 variables which are hours & scores scores are in the form of integer and hours are in the form of numeric. 
#### also there are no missing values in dataset

### 2) Plotting and Studying the relationship between variables:- 
![image](https://user-images.githubusercontent.com/96919264/148707408-79bceb37-abe3-486b-b56b-69de1fd0637c.png)

from above graph we can clearly observe the __strong positive relationship___ between the hours studied by the student and score obtained and that amount of correlation is __0.976190656022089__ ( We Calculated )

### 3)Fitting the Simple Linear Regression Model
From above summary we can clearely observe , From the P-value we can observe our model is significant at 1% error.

Fitted model is Y = 2.4837 + 9.7758*X ( where Y is score obtained and x is hours studied as mentioned earlier )

using this formula of model we can predict the values of scores given the amount of hours studied Also value of R-SQUARED is 0.9529 that indicates 95.29 % amount of variablity in the scores is explained by amount of hours studied. which implies our model is good fit.

![image](https://user-images.githubusercontent.com/96919264/148707509-72ead221-0683-4eae-9f9d-e89cf809e438.png)
In the above plot dots represnt the actual values and yellow straight line represents the fitted values of the model

### 4) compairing actual V/s Fitted values

![image](https://user-images.githubusercontent.com/96919264/148707569-9a064b9d-4ca1-4fcc-bf32-1b4fb5d2083f.png)
Clearly from above graph we can see that observed and fitted values of the scores are almost same which indicates that we have appropriately fitted the model


### 5) Prediction of Score 
Using simple linear regression model Y = 2.4837 + 9.7758*X we can easily predict that ; 
If a student studies for __9.25 hours__ per day then he can approximately score __93 marks__(marks given as integer) in the examination
