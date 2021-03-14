# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to create, train, and refine a neural network model for the purposes of predicting the status of future investments by Alphabet Soup.

## Results

### Data Preprocessing
* The IS_SUCCESSFUL column is the target of our model
* The following columns are considered features of my model: ASK_AMT, SPECIAL_CONSIDERATIONS, INCOME_AMT, APPLICATION_TYPE, STATUS
* The CLASSIFICATION column is considered neither a feature or a target, and was removed (in addition to EIN and NAME)

### Compiling, Training, and Evaluating the model
* Due to the relatively large number of features, the model contains 5 hidden layers, each with a decreasing # of neurons. Relu activation function was used throughout
![Model](https://github.com/noble190/Neural_Network_Charity_Analysis/blob/main/Images/Optimization_Attempt8_Details.png)
<hr>
