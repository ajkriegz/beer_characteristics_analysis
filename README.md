# Beer Characteristics Profiling 

[Click here for the presentation.](https://docs.google.com/presentation/d/1Rn_7RCTm9UO72irvWF4ho0fOMzaHRWQAoMQVw0SUD4k/edit#slide=id.p)

## Overview

The scope of the project is the flavor profile of successful beers. Since the data analytics program is based in Wisconsin, it seemed like a suitable and fun topic to explore.

The dataset used, Beer Profile and Ratings dataset, is a combination of two datasets available on Kaggle. The first contains flavor profiles of successful beers and the second contains over a million reviews of beers.

The data will be analyzed to understand the what contributes to a high rating for a beer overall and for specific styles listed in the dataset. Our group also intends to investigate how much the appearance of a beer factors into a very positive review. 

Descriptions to add:
* Description of the data exploration phase of the project
* Description of the analysis phase of the project
prelim feature testing
prelim 

## Communication Protocols

Our team has decided on a variety of tools to utilize for the duration of the project. Github is the resource for filesharing and collaborating on code. A group calendar has been created with Google Calendar to assess availability and schedule meetings to work together. Trello is helping to manage tasks and expectations for the deliverables of each milestone in the project. Slack is being used for messaging between teammates and arranging calls. 

## Dashboard

The project's visualization will be created using Tableau. The interactive elements under consideration are changing data based on style and by brewery. Other ideas are to show where each brewery is located on a map.

## Machine Learning Model

### Model Choice 

A supervised machine learning model was chosen as the ideal approach for the flavor profile investigation. Implementing a random forest algorithm will be useful since it will have a less likelihood of overfitting, it can manage many inputs, and it can rank the features easily. The classification model will effectively return the most important characteristics for predicting a popular beer. 

### Data Preprocessing

#### Feature Selection and Engineering 

After reading in the data and examining the features, there were some that were filtered and others, identified as unnecessary for the model, that were dropped. 

To avoid having the analysis skewed by beers with only a few reviews, the dataframe was refined to include only beers with a number of reviews greater than or equal to the upper quartile.   

The target variable, the overall review, was separated into binary values. A successful beer will have a rating greater than or equal to a 4 star score and classified as a 1. If it doesn't meet this criteria it is classified as a 0. 

#### Training and Testing 