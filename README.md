# DataAnalysis - Diploma Project


Spatial analysis of tourist areas using social networks is the study and deepening of the concepts and processes of data extraction, data analysis and visualization. The study also contains the use of Machine Learning techniques making a small introduction to the field of data science.

The project presents the technologies used, the theoretical aspects and the implementation of the software project, problems encountered, but also solving or finding alternative solutions to apply the study in a practical format. The site of interest around which the work focused is Airbnb.

All information resulting from the end of the project is attributed to the city of Brașov, Romania. On the Airbnb site it contains about 300 diverse listings. Prices, room type, reviews are just a few criteria applied to this analysis.
 
Finally, the resulting graphs and numbers will show both the average prices of these listings and the most areas of interest in the city. 
The reference source of the project were similar projects developed in Berlin and Madrid.

What I wanted to prove through this project? 
This project shows the price level on Airbnb of Brasov. E.g:
-268 listings;

-minimum price per night 81 RON;

-maximum price per night 550 RON;

- average prices 204.60;

-sum of prices of all listings 54833.37;

-prices worth 140.0 represented 25% of the listings;
etc.

What is Machine Learning doing in this project?
Listing Price Prediction - Economy
How?

## Moving Average
Introduction

‘Average’ is easily one of the most common things we use in our day-to-day lives. For instance, calculating the average marks to determine overall performance, or finding the average temperature of the past few days to get an idea about today’s temperature – these all are routine tasks we do on a regular basis. So this is a good starting point to use on our dataset for making predictions.

The predicted closing price for each day will be the average of a set of previously observed values. Instead of using the simple average, we will be using the moving average technique which uses the latest set of values for each prediction. In other words, for each subsequent step, the predicted values are taken into consideration while removing the oldest observed value from the set. Here is a simple figure that will help you understand this with more clarity.

We will implement this technique on our dataset. The first step is to create a dataframe that contains only the Date and Close price columns, then split it into train and validation sets to verify our predictions
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/6.JPG)

## Linear Regression
Introduction

The most basic machine learning algorithm that can be implemented on this data is linear regression. The linear regression model returns an equation that determines the relationship between the independent variables and the dependent variable.

The equation for linear regression can be written as:
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/9.JPG)
Here, x1, x2,….xn represent the independent variables while the coefficients θ1, θ2, …. θn  represent the weights. You can refer to the following article to study linear regression in more detail:



For our problem statement, we do not have a set of independent variables. We have only the dates instead. Let us use the date column to extract features like – day, month, year,  mon/fri etc. and then fit a linear regression model.
Implementation

We will first sort the dataset in ascending order and then create a separate dataset so that any new feature created does not affect the original data.
Auto ARIMA
Introduction

ARIMA is a very popular statistical method for time series forecasting. ARIMA models take into account the past values to predict the future values. There are three important parameters in ARIMA:

    p (past values used for forecasting the next value)
    q (past forecast errors used to predict the future values)
    d (order of differencing)

Parameter tuning for ARIMA consumes a lot of time. So we will use auto ARIMA which automatically selects the best combination of (p,q,d) that provides the least error. To read more about how auto ARIMA works, refer to this article:

    
    
 # So far, we have presented the economic part of the prediction, but we have approached another slightly easier option, in order to balance the results. Do both methods give the same results?
 ## The K-nearest neighbors algorithm

The K-nearest neighbors (KNN) algorithm works similarly to the three-step process we outlined earlier to compare our listing to similar listings and take the average price. Let’s look at it in some more detail:

First, we select the number of similar listings k, that we want to compare with. 
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/10.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/11.JPG)
 ## Euclidean distance

When trying to predict a continuous value like price, the main similarity metric that’s used is Euclidean distance. Here’s the general formula for Euclidean distance: \(d = \sqrt{(q_1-p_1)^2 + (q_2-p_2)^2 + \cdots + (q_n-p_n)^2}\) where \( q_1 \) to \( q_n \) represent the feature values for one observation and \( p_1 \) to \( p_n \) represent the feature values for the other observation.

If your head just exploded, don’t worry! We’re going to break that down into smaller pieces. We’ll start by…
## Building a Basic KNN Model
 # Introduction to scikit-learn

We’ve been writing functions from scratch to train our k-nearest neighbor models. This is helpful to understand how the mechanics work, but now that we understand the underlying fundamentals, we can work much more quickly and efficiently using Python’s scikit-learn library.

Scikit-learn is the most popular machine learning library in Python. It has built-in functions for all of the major machine learning algorithms and a simple, unified workflow. Both of these properties allow data scientists to be incredibly productive when training and testing different models on a new data set.

# This is only part of the reasoning, of the total project. The full description of the project is in the attached documentation.
![Image of Project](https://github.com/ArianaAnd/DataAnalysis-Diploma-Project/blob/master/Licenta2020v3.docx)
# Or you can see some additional details about the look in
![Image of Project](https://github.com/ArianaAnd/DataAnalysis-Diploma-Project/blob/master/Clip.mp4)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis-Diploma-Project/blob/master/Diploma%20Project%20Presentation.pdf)


TOOLS: ANACONDA, JUPYTER NOTEBOOK, PARSEHUB(EXTRACT DATA), C#(EXTRACT DATA), PYTHON. NODEJS(EXTRACT DATA)


![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/Project.jpg)


![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/coordonates.png)

![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/1.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/2.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/3.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/5.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/7.JPG)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/Cluster.jpg)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/regresia.jpg)
![Image of Project](https://github.com/ArianaAnd/DataAnalysis/blob/master/map.png)
