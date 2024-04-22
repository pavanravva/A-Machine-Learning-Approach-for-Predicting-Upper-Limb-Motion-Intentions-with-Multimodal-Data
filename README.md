# A-Machine-Learning-Approach-for-Predicting-Upper-Limb-Motion-Intentions-with-Multimodal-Data


This repository has five machine learning classification models along with two step model proposed in the paper: Logistic Regression, K-Nearest Neighbors (KNN), Support Vector Machine (SVM), and a Neural Network (NN) and combinatation of Long Short Term Memory (LSTM) + Neuaral Network (NN). These models uses libries as scikit-learn and TensorFlow. This guide will cover the dataset preparation, model training, prediction, and evaluation of each model.

Logistic Regression, K-Nearest Neighbour, Support Vector Machines (SVM):

Data Processing:
Few columns are dropped, data is normalized and split into train and test. 

Evaluation:
F-1 score and accuracy are used to estimate the performance. 

Neural Network:

In Neural Network, we have used 2 hidden layers of 64 neurons in the first and 32 neurons in the second one, we have trained the model for 50 epochs, and the learning rate is 0.001. 

Data Processing:
Few columns are dropped, data is normalized and split into train and test. 

Evaluation:
F-1 score and accuracy are used to estimate the performance. 

LSTM:

In LSTM, we have used 2 hidden layers of 64 neurons in the first and 32 neurons in the second one, we have trained the model for 50 epochs, and the learning rate is 0.001 with l2 regulirization in loss function. 

Data Processing:
Few columns are dropped, data is normalized and split into train and test. 

Evaluation:
F-1 score and accuracy are used to estimate the performance. 


Two-Step Model:

This model is combination of both the LSTM and NN model, where only the gaze data is feed into the neural network model, and the features of neural network model is combined with raw resistance data, for prediction task. The first model is used to predict the 4 edges of the shape of motion, and the LSTM model is used to predict the direction of motion.

This Model has same parameters as the above NN and LSTM.






