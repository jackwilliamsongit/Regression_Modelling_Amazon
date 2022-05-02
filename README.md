# Regression_Modelling_Amazon
## Description
The purpose of this project is to create a machine learning regression model to predict the score rating a product review was given, using the corresponding review text. A large dataset of reviews for a wide multiple projects was used as the data source and the classifier chosen for prediction was logistic regression.

The data used is a very large file (303 MB) and therefore cannot be made available in this github repository. It can be found at the link at the end of this REAM ME file.

## Breif Code Walkthrough
The data was explored breifly and prepared for analysis. The review text was vectorised and scaled using the 'bag of words' vectorisation method. The data to be modelled was split into testing and training groups, to develope the model and to test the effectiveness of the model prediction. 

The model was then trained and the accuracy was assessed for varying degrees of precision.

## Results
The final accuracy of the review rating prediction was 78% for the exact rating 1-5. The final accuracy with an error of 1 'star' was 92.14%

Although 78% may seem lower than optimal for the prediction accuracy, it is very difficult to accurately predict the exact rating as it is very subjective. 2 reviews could contain the exact same language, but one reviewer could consider the score to be 3 and another to be 4. Thus, the accuracy of the rating with an error of 1 'star' was considered and provided a very high accuracy.

## Possible Improvements
Since the review score is discrete, the model is built around training the model to predict discrete scores. This limits the rangle of classifiers available and also presents the issue of the model predicting individual strings that are actually related along a range. This could prehaps be overcome by predicting a score value along a continuous range and discretising the output to the nearest exact score. This would allow the model to closer relate the scores of 4-5 than 4-1 and could lead to improvements in accuracy.

## Data Sourcing
The dataset was sourced through kaggle and is available at https://www.kaggle.com/code/jillanisofttech/nlp-amazon-data-preparation-prediction-with-99-acc/data
