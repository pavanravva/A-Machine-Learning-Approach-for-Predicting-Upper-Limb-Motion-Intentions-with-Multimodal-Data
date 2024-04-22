# A-Machine-Learning-Approach-for-Predicting-Upper-Limb-Motion-Intentions-with-Multimodal-Data

This repository contains five machine learning classification models as described in the associated paper. The models include:

Logistic Regression
K-Nearest Neighbors (KNN)
Support Vector Machine (SVM)
Neural Network (NN)
Combination of Long Short-Term Memory (LSTM) and Neural Network (NN)
These models utilize libraries such as Scikit-learn and TensorFlow. This guide covers dataset preparation, model training, prediction, and evaluation for each model.

Models and Evaluation:

Logistic Regression, K-Nearest Neighbors, Support Vector Machines (SVM):
Data Processing:
Drop selected columns
Normalize data
Split data into train and test sets
Evaluation Metrics:
F-1 Score
Accuracy

Neural Network (NN):
Configuration:
Two hidden layers with 64 neurons in the first layer and 32 neurons in the second layer
Trained for 50 epochs
Learning rate: 0.001
Data Processing: Same as above.
Evaluation Metrics: Same as above.

LSTM:
Configuration:
Two hidden layers with 64 neurons in the first layer and 32 neurons in the second layer
Trained for 50 epochs
Learning rate: 0.001
L2 regularization in the loss function
Data Processing: Same as above.
Evaluation Metrics: Same as above.

Two-Step Model:
Description:
This model is a combination of the LSTM and NN models. Only gaze data is fed into the NN, and the features from the NN are combined with raw resistance data for the prediction task.
The NN model predicts the four edges of the motion shape, while the LSTM model predicts the motion direction.
Configuration: Same parameters as the NN and LSTM models mentioned above.

# CSV Files Overview
The repository includes three CSV files, each containing specific sets of data collected from the participants' movements and corresponding gaze data. Here’s what each file contains:

Circle_original_Resistance.csv
Contents: Original resistance values collected from the sleeve, combined with gaze data for the circle motion of participants.
Purpose: Provides resistance measurements specifically for participants performing circle motions, alongside their gaze data to correlate visual focus and movement resistance.

Diamond_original_Resistance.csv
Contents: Original resistance values collected from the sleeve, combined with gaze data for the diamond motion of participants.
Purpose: Contains resistance data for diamond motion exercises, coupled with gaze tracking information to analyze the relationship between eye movements and resistance levels.

Diamond_Circle_Resistance_Time_Features.csv
Contents: Time-varying features of the resistance values, along with the gaze data for both circle and diamond motions of participants.
Purpose: Integrates both circle and diamond motion data, emphasizing the dynamic aspects of resistance and gaze data over time, useful for comprehensive motion analysis.






