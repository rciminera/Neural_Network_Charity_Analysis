# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to develop a model that will accurately predict sound charity investments for the Alphabet Soup foundation using neural networks as a potential solution.  

The goal of the model to create a binary classifier that is capable of predicting successful investments with an accuracy greater than 75%.


## Results

Using various modules from Tensor Flow along with Google Colab notebook the following steps were followed:

- Data Preprocessing
- Compiling, Training, and Evaluation the Neural Network Model
- Optimizing the Neural Network model for the highest possible accuracy.

#### Data Preprocessing

1. The "IS_SUCCESSFUL" variable was set as the target of the model.
2. The variables used as features for the model included:

    + APPLICATION_TYPE—Alphabet Soup application type
    + AFFILIATION—Affiliated sector of industry 
    + CLASSIFICATION—Government organization classification
    + USE_CASE—Use case for funding
    + ORGANIZATION—Organization type
    + STATUS—Active status
    + INCOME_AMT—Income classification
    + SPECIAL_CONSIDERATIONS—Special consideration for application
    + ASK_AMT—Funding amount requested  


3. The variables "EIN" and "NAME" identification columns were neither targets nor features, and were removed from the input data.

#### Compiling, Training, and Evaluating the Model
4. In the base neural network model, 110 neurons and 2 hidden layers were selected to support the 43 variables.  The number of neurons were selected based on a rule of 2 to 3 times the number of input variables.  In addition, the relu activation function was used for the inner layers and sigmoid was used for the output layer.  These functions were selected because of the binary nature of the model.

5. At 72.57% the target performance was not acheived.

#### Optimizing the Model
6. To optimize the model and increase performance a number of steps were taken to increase performance to above 75%:

    ✓ Noisy variables were removed from features  
    ✓ Additional neurons were added to the hidden layers.   
    ✓ Additional hidden layers were added  
    ✓ The activation function of hidden layers were changed for optimization. 



#### Checkpoints and Saving

For the base and optimization models, checkpoints were taken every 5 epochs and the model was saved in the following HDF5 files:  

## Summary

Overall the various iterations of the model did not yiled 75% as shown below.

<img src="https://github.com/rciminera/Cryptocurrencies/blob/main/ScreenShots/crypto_df.png" width = "800" >

 Recommnedations for improving the accuracy of the outcome include further processing of the data as well as the structure of the model.  In addition, a Random Forest Model or other Deep Learning models should be explored.

