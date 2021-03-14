# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to create, train, and refine a neural network model for the purposes of predicting the status of future investments by Alphabet Soup.

## Results

### Data Preprocessing
* The IS_SUCCESSFUL column is the target of our model
* The following columns are considered features of my model: ASK_AMT, SPECIAL_CONSIDERATIONS, INCOME_AMT, APPLICATION_TYPE, STATUS
* The CLASSIFICATION column is considered neither a feature or a target, and was removed (in addition to EIN and NAME)

### Compiling, Training, and Evaluating the model
Due to the relatively large number of features, the model contains 5 hidden layers, each with a decreasing # of neurons. Relu activation function was used throughout
![Model](https://github.com/noble190/Neural_Network_Charity_Analysis/blob/main/Images/Optimization_Attempt8_Details.png)

Unfortunately, I was not able to meet the stated performance goal of 75% on the test data. I saw close to the target when training the model, which suggests that overfitting may be an issue (likely due to the relatively high # of features). I noticed that the model became less accurate if the # of epochs were increased, which likely indicates overfitting.
 ![Model Results](https://github.com/noble190/Neural_Network_Charity_Analysis/blob/main/Images/Optimization_Attempt8_Results.png)

Before attempted optimization, I was looking at a model accuracy of ~53%. I've attempted a few approaches to improve this %.
<br>
The most significant improvement came as a result of creating buckets for the 'ASK_AMT' column, and incorporating this model as a feature. 
![Model Optimization](https://github.com/noble190/Neural_Network_Charity_Analysis/blob/main/Images/Optimization.png)

