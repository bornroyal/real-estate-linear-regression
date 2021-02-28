# Project 2: Decreasing the Odds of a Low Home Appraisal
---

### Contents:

- [Problem Statement](#Problem-Statement)
- [Executive Summary](#Executive-Summary)
- [Data Sources](#Data-Sources)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

---

### Problem Statement:

Many realtors in Ames, IA have had increased dissastisfaction rates and reviews from clients. Over 90% percent of these bad reviews on google and yelp list the client was unhappy with the realtors lack of housing knowledge. 
As a realtor in Ames, it is crucial to help the clients that list their homes with us to receive top dollar. In order to improve client rapport, realtors need to be experienced in what factors affect receiving a low appraisal rate. Appraisal rates are the assesors investigation on what each home is valued at based on many factors. As realtors knowing which factors affect home appraisal rate is very important to help our clients, receive what they are looking for when they come to us. The Data Science process can help answer this, and i will examine what features can increase a home's value to help our clients find areas of improvement. 



### Executive Summary

For this analysis, I leveraged the Ames Housing Datasets which were created by the Ames Assessors Office. This dataset includes statistics about roughly 3000 homes which were sold in Ames, Iowa between the years 2006 and 2010. The datasets, which are split in to training and testing files, contain over 80 features about the houses and properties sold in Ames. Through data cleaning, exploration and analysis, followed by creating various regression models, I have developed a model that identifies the key drivers of sale price with an eye toward features which the homeowner can improve prior to listing their house, in order to increase their selling price. 



### Data Sources
* [`train.csv`](./datasets/train.csv): Ames Housing Data Training Dataset | [data dictionary](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt))
* [`test.csv`](./datasets/test.csv): Ames Housing Data Training Dataset 
* [`ames_train.csv`](./datasets/test.csv): Cleaned Ames Housing Data Training Dataset 
* [`ames_test.csv`](./datasets/test.csv): Cleaned Ames Housing Data Testing Dataset 



### Conclusions and Recommendations
In conclusion, home square footage, garage and pool square footage, overall house quality,exterior quality, number of bathrooms,and number of car garages are the most correlated to sale price. This means that as these features increase, so does the value of the home. This means as a realtor directing your clients to improve these features can decrease the chances of receiving a low appraisal rate.  
During my analysis, i created a linear regression and lasso regression model to predict sale price based on these highly positive correlated features with sale price. The model currently has an r2 score of .90 and an RMSE of .13 in respects to the log of sale price. 
This means about ~90% of the variance in the data can be explained by my model compared to the baseline model, of just predicting the mean house price which is $180,558.
