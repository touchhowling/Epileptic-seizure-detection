# Epilepsy Detection Using EEG Signals

This project aims to classify EEG signals as epileptic or non-epileptic using Long Short-Term Memory (LSTM) networks for improved epilepsy detection. Epilepsy, characterized by abnormal brain activity, can be caused by genetic disorders or acquired brain injuries. By automatically detecting epileptic seizures, this project contributes to enhancing the quality of life for patients.

## Seizure
A seizure is a sudden surge of electrical activity in the brain, resulting in temporary changes in a person's behavior or appearance. Seizures can manifest in various ways, and their occurrence can be unpredictable.

## Detection
Automatic detection of epileptic seizures can greatly benefit patients. However, it poses challenges due to non-stationary EEG signals and variations in seizure patterns among individuals. To address these challenges, a deep learning approach leveraging LSTM networks is employed to learn discriminative features from EEG signals. The learned representations are then used for training and classification, with the Softmax function being applied.

## Dataset
The dataset used for this project is sourced from the UCI Machine Learning Repository - Epileptic Seizure Recognition Data Set. It consists of EEG recordings from 500 individuals, with each recording spanning 23.6 seconds and comprising 4097 data points. The dataset is divided into five categories: eyes open, eyes closed, recording from a healthy brain area, recording from a brain area with a tumor, and recording of seizure activity. The goal is to classify the recordings as epileptic or non-epileptic.

## Procedure Followed for Binary Classification
In the binary classification task of distinguishing epileptic and non-epileptic signals, the following procedure was followed:

1. Model.ipynb:
   - Data visualization was performed for all five classes.
   - A recurrent neural network architecture with two LSTM layers was defined.
   - The optimizer was set to 'adam', and the loss function was set to 'binary_crossentropy'.
   - Data preprocessing involved selecting every fourth sample, normalizing the data, and using the previously split test data as validation data.
   - The model was trained for 50 epochs and saved.
   - Loss and accuracy rates were plotted to assess model performance.

2. Product_Final.ipynb:
   - The trained model was loaded and used for predictions on the validation set.
   - The predictions were converted to binary classes: 1 for epileptic signals and 0 for non-epileptic signals.
   - The same procedure was applied to the training set.

By leveraging the power of LSTM networks, this project contributes to the development of an accurate and automated epileptic seizure detection system.

Please refer to the respective Jupyter Notebook files for detailed implementation and code.
