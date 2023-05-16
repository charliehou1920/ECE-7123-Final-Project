# ECE-GY-7123-Final-Project
##  Difference Between our Final Project and Proposal

(1) Dataset: In Proposal, we claimed that we would use SP500 Index, CSI 300 Index and BTC Index as our dataset. However, for Final Project we only applied our models on SP500 Index because these 3 indexes are quite similar to each other.

(2) Models: In Proposal, we said that we would use LSTM as the only network. However, in final project, we add GRU, Simple RNN and TCN these 3 networks to broaden the range of our models.

(3) Metrics: In Proposal, we said we would use Accuracy, Precision and Recall for our metrics. However, in our final project we used mean absolute percentage error (MAPE) and mean absolute error (MAE) as our metric because our task is not a classification task.

(4) Back Test: In proposal, we said we would create a back test for our strategy based on the results from our network. However, in final project we deleted this part because it's irrelevant to deep learning.

--------------------------------------------------------------------

## A Guide for this repository

This Repository contains 4 files:

(1) Final_Project.ipynb: This file contains everything for this final project. We recommend you to run it on Google Colab.

(2) Best_Model_Loss_history.PNG: This is a screen shot which records the loss (MSE) per epoch in our best mode

(3) Best_Model_MAE_history.PNG: This is a screen shot which records the MAE (Mean Absolute Error) per epoch in our best model

(4) Best_Model_Correlation.PNG: This is a screen shot which records Predicted Price vs Real Price

(5) README.md: The README file provides a generalization for this mini project

------------------------------------------------------------------------------------------------------

## Final Model Architecture / Parameters / Hyper-parameters

| Final model parameters |                   Values for the parameter                   |
| :--------------------: | :----------------------------------------------------------: |
|       Batch Size       |                              64                              |
|         Epoch          |                              50                              |
|    Layer Structure     | Two stacked GRU layers with 32 units, one Dropout layer with 0.5 rate, and one Dense layer |
|     Input Features     |                  Closed price and Momentum                   |
|     Loss Function      |                      Mean Squared Error                      |
|       Optimizer        |                Adam with learning rate 0.0003                |
|       Time step        |                              50                              |

