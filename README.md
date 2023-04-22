# SC1015 - Gaming the Data

Done by: Gan Kai Feng, Ng Zi Xuan, Nicholas Loh Hui Kean
<br></br>
Lab Group: B140

## About
This mini-project is part of our module SC1015 (Introduction to Data Science & Artificial Intelligence) which focuses on popularity of video games in 2016. 

![Metacritic Platform](https://duet-cdn.vox-cdn.com/thumbor/0x0:1316x894/828x552/filters:focal(658x447:659x448):format(webp)/cdn.vox-cdn.com/uploads/chorus_asset/file/20095893/Screen_Shot_2020_07_17_at_2.36.15_PM.png) <br>
(Image from: https://www.theverge.com/2020/7/17/21328597/metacritic-user-reviews-delayed-review-bombing)

>"2016 was another enormous year for the interactive entertainment industry...The industry's innovative genius and ability to engage and delight billions of gamers worldwide delivered another record performance. Congratulations to the developers, storytellers, creators, and investors who defined the leaderboard for entertainment." - Michael D. Gallagher, president and CEO of the ESA (Entertainment Software Association)

Given the expansive and growing video game industry, we are aware how data analysis on video games sales may be helpful to budding companies or start-ups which want to break through into the market. While doing so, individuals who are keen to enter the market may be inspired and produce some sort of disruptive innovation. Therefore, our project attempts to identify relatively popular (and not so popular) video games, and the contributing factors to their successes.

The dataset we used can be accessed from the links below:
- [Dataset](https://github.com/ngzxzxzx/SC1015---Gaming-The-Data/blob/main/VideoGamesDataset.zip)
- The original dataset is titled "Video_Games_Sales_as_at_22_Dec_2016.csv" and the cleaned dataset we used subsequently for our notebooks is titled "vidgames_cleaned.csv".
- Alternatively, you may access the original dataset on [Kaggle](https://www.kaggle.com/datasets/dileepsahu/video-games-sale-data-set-dec-2016)

<br> </br>
For easy navigation, you may also look at the individual notebooks split into different junctures of the project:

1. [Data Cleaning](https://github.com/ngzxzxzx/SC1015/blob/main/Data%20Cleaning.ipynb)
2. [Problem Formulation 1, Exploratory Data Analysis (EDA)](https://github.com/ngzxzxzx/SC1015/blob/main/Problem%20Formulation%20and%20Exploratory%20Data%20Analysis.ipynb)
3. [Regression Models](https://github.com/ngzxzxzx/SC1015/blob/main/Regression%20Models.ipynb)
4. [Problem Formulation 2, Classification Models](https://github.com/ngzxzxzx/SC1015/blob/main/Classification_Methods.ipynb)


## Problem Formulation
1. Are we able to predict Global Sales (Response) using other variables (Predictors) from our data? 
2. What is the most important feature in predicting Global Sales? (Feature Importance)
3. Are we able to identify whether a video game is popular or not? (Classification) 


## Models Used
<br> </br>
Regression Models:
- Linear Regression
- Random Forest Regression
- Ridge Regression
- XG Boost

<br></br>
Classification Models:
- K Nearest Neighbours (KNN)
- Decision Tree
- Random Forest Classification


## Conclusion and Key Insights
- Regression models were not very successful in predicting Global Sales, given the low R^2 values.
- However, we can identify (the most) important features while trying to predict Global Sales. In our results, we found that the number of Metacritic subscribers who gave a score was the most important feature.
- Classification models are relatively accurate in determining whether a video game will be a hit or not.
- Through our findings, we suggest for video game companies to:
1. Emulate established companies like Nintendo. Our results have shown that games under Nintendo are likely to become a hit.
2. Encourage their playerbase to leave more reviews on metacritic, as the number of reviews on metacritic is shown to be the strongest predictor for 
   Global Sales
3. Ensure that the quality of games produced is high enough for critics to leave a positive review on metacritic, as a high critic score is indicative
   of high Global Sales


## What Did We Learn From This Project?
- Aggregation of variables for data points with the same name. 
- Long-tailed distributions affect the performance of our models. In fact the accuracy and usefulness of our models drop drastically.
- Removing outliers for a long-tailed distribution can be iffy. Nevertheless, we removed outliers until we are able to visibly see the distribution on a graph, even though it may be slightly skewed.
- Why the overfitting of data occurs, and how it affects the R^2 values of test and train data
- Different regression and classification models outside the scope of this module: Random Forest Regression and Classification, Ridge Regression and XGBoost
- Regression models have their own strengths. For example, Ridge Regression is good for overcoming overfitting, which may be useful for some datasets, and Random Forest Regression provides us the function to identify feature importances
- One-hot encoding is extremely useful in representing categorical data in numerical form
- We have to ensure that we avoid the dummy trap when using one-hot representations in our code



| Member | Contributions |
|:---:|:---:|
| Zi Xuan | Data Cleaning, EDA |
| Nicholas | Regression Models |
| Kai Feng | Classification Models |


