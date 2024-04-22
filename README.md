# A-Machine-Learning-Approach-for-Predicting-Upper-Limb-Motion-Intentions-with-Multimodal-Data

This repository corresponds to the study titled 'A Machine Learning Approach for Predicting Upper Limb Motion Intentions with Multimodal Data.' To reference this paper, please use the following citation:


## Used Models and Evaluation:

### Logistic Regression, K-Nearest Neighbors, Support Vector Machines (SVM):

- **Data Processing:**
  - Drop selected columns
  - Normalize data
  - Split data into train and test sets
- **Evaluation Metrics:**
  - F-1 Score
  - Accuracy

### Neural Network (NN):

- **Configuration:**
  - Two hidden layers with 64 neurons in the first layer and 32 neurons in the second layer. Trained for 50 epochs with a learning rate of 0.001.
- **Data Processing:**
  - Drop selected columns
  - Normalize data
  - Split data into train and test sets
- **Evaluation Metrics:**
  - F-1 Score
  - Accuracy

### Long Short-Term Memory (LSTM):

- **Configuration:**
  - Two hidden layers with 64 neurons in the first layer and 32 neurons in the second layer. Trained for 50 epochs with a learning rate of 0.001 and L2 regularization.
- **Data Processing:**
  - Drop selected columns
  - Normalize data
  - Split data into train and test sets
- **Evaluation Metrics:**
  - F-1 Score
  - Accuracy

### Two-Step Model (Combination of LSTM and NN):

- **Description:** Combines LSTM and NN models. NN predicts motion shape edges using gaze data, while LSTM predicts motion direction using raw resistance data.
- **Configuration:** Same as the NN and LSTM models.

## CSV Files Overview:

1. **Circle_original_Resistance.csv:**
   - **Contents:** Original resistance values from the sleeve, combined with gaze data for circle motion of participants.
   - **Purpose:** Provides resistance measurements for participants performing circle motions along with gaze data to correlate visual focus and movement resistance.

2. **Diamond_original_Resistance.csv:**
   - **Contents:** Original resistance values from the sleeve, combined with gaze data for diamond motion of participants.
   - **Purpose:** Contains resistance data for diamond motion exercises, useful for analyzing eye movement and resistance levels relationship.

3. **Diamond_Circle_Resistance_Time_Features.csv:**
   - **Contents:** Time-varying features of resistance values with gaze data for both circle and diamond motions of participants.
   - **Purpose:** Integrates circle and diamond motion data, focusing on dynamic aspects of resistance and gaze data over time for comprehensive motion analysis.









