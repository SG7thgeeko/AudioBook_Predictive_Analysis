# Audiobooks Data Classification with Neural Network

This repository contains Python code for building a neural network model using TensorFlow and scikit-learn to perform binary classification on audiobooks data.

## Dataset

1.The data set contains data sourced from an audiobook application. Each customer in the database has made a purchase atleast once.The data represents two years worth of engagement.
2.One can predict if the customer will make a purchase again from the audiobook company.
3.The main idea is that the company shouldn't spend its advertising budget targeting individuals who are unlikely to come back. If we can focus our efforts on customers likely to convert again, we can obtain improved sales and profitability figures.
4.The dataset is loaded from 'Audiobooks_data.csv', consisting of input features and binary target labels.

## Data Preprocessing

1. Inputs are scaled using standardization (`preprocessing.scale`).
2. Shuffling and splitting into training, validation, and test sets are performed.

## Neural Network Model

The neural network architecture is defined as follows:

- Input layer: 10 nodes
- Hidden layers: Two layers with 50 nodes each and ReLU activation
- Output layer: 2 nodes with softmax activation for binary classification

## Model Training

The model is compiled with Adam optimizer and sparse categorical crossentropy loss. Training includes early stopping to prevent overfitting, with a batch size of 100 and a maximum of 100 epochs.

## Model Evaluation

The trained model is evaluated on the test set, and test loss and accuracy are printed.

## Prediction on Additional Data

Additional data from 'Audiobooks_data_testing.csv' is loaded for predictions. Predicted classes are added as a new column to 'Audiobooks_data_pt.csv'.

## Usage

1. Ensure you have the required libraries installed (`tensorflow`, `numpy`, `scikit-learn`, `pandas`).
2. Run the provided Python script.

## File Structure

- `Audiobooks_data.csv`: Original dataset
- `Audiobooks_data_pt.csv`: Updated dataset with predicted classes
- `Audiobooks_data_train.npz`, `Audiobooks_data_validation.npz`, `Audiobooks_data_test.npz`: Saved numpy arrays for training, validation, and test sets
- `README.md`: Documentation file

## Note

Ensure that file paths and data dimensions are correctly specified in the code.

Feel free to reach out for any questions or improvements!
