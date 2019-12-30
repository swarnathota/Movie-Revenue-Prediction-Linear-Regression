# Movie  domestic total gross prediction

## Data collection and EDA:

1. Movie data Title, Rating, Genre, Budget, Runtime, Distributor and Domestic Total Gross are selected as features.

2. Data is collected by web scraping using Beautiful soup from https://www.boxofficemojo.com/ and Budget is from https://www.the-numbers.com/. 

3. Data is cleaned and performed EDA:

   . Top 10 distributors and Distributor vs DTG

   . Top 10 genre and Genre vs DTG

   . Effect of seasonal release of movie on DTG

   . Effect of Rating on DTG

## Linear Regression Analysis

1. Linear regression analysis is performed using SKlearn
2. Diognostic plots like  residual vs predict and probability plot suggested that there is no direct linear relationship between target and features.
3. Introduced polynomials using sklearn PolynomialFeatures followed by Lasso regularization.
4. Found that Movie Budget has the direct effect on DTG compared to other features.

## What can be done to improve model 

Although introducing polynomials could improve the model, it needs to be further improved by incuding other features such as cast and crew, Director, writer, studios and movie rating etc.