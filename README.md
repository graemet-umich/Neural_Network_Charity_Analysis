# Neural Network Charity Analysis
Module 19: Neural Networks and Deep Learning Models

## Overview

## Results

### Data Preprocessing

- **Variable as model target.** The `IS_SUCCESSFUL` variable is the only model target. A value of 1 or 0 indicates that the funding money was uses either successfully or unsuccessfully. 

- **Variables as model features.** 
    - The numerical feature variables are `STATUS` and `ASK_AMT`. They are suitable for modelling as is.           

    - The categorical feature variables are 
 `APPLICATION_TYPE`,
 `AFFILIATION`,
 `CLASSIFICATION`,
 `USE_CASE`,
 `ORGANIZATION`,
 `INCOME_AMT`, and
 `SPECIAL_CONSIDERATIONS`. Using `OneHotEncoder()`, they are fit and transformed to numerical values suitable for modelling. 

- **Variables that are neither targets nor features.** The `EIN` and `NAME` variables are not useful for modelling, as they are unique. They are removed.

### Compiling, Training, and Evaluating the Model

| cvc bins | anno | act. | input | layer1 | layer2 | layer3 | layer4 | layer5 | loss | accuracy | 
| ---: | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 6 | no | relu | 80 | 30 | | | | | 0.653 | 0.628 |
| 6 | yes | relu | 25 | 22 | 24 | 26 | | | 0.681 | 0.550 |
| 6 | yes | relu | 25 | 22 | 24 | 26 | 8 |  | 0.748 | 0.533 |
| 6 | yes | relu | 25 | 22 | 24 | 26 | 8 | 10 | 0.694 | 0.527 |
| 7 | no | relu | 80 | 30 | | | | | 0.700 | 0.697 |
| 13 | no | relu | 80 | 30 | | | | | 0.881 | 0.696 |
| 7 | yes | relu | 65 | 8 | 4 | 10 | 6 | 8 | 0.692 | 0.533 |




- **How many neurons, layers, and activation functions did you select for your neural network model, and why?** Use the automated NN finder.
- Were you able to achieve the target model performance?
- **What steps did you take to try and increase model performance?** Use the automated NN finder.

## Summary

- Summarize results
- **Recommend and justify a different model to solve the classification problem.** Choose from logistic regression, random forest, or SVN.
