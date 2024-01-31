# Audiobook Classification Project

## Overview

This repository contains the code for a neural network-based audiobook classification project. The project involves preprocessing audiobook data, training a neural network model, and making predictions on new data.

## Files

- **Audiobooks_data_pt.csv:** Preprocessed data containing features and target labels.
- **Audiobooks_data_testing.csv:** New input data for prediction.
- **your_trained_model_path:** Trained neural network model saved during or after training.
- **Audiobooks_data_train.npz, Audiobooks_data_validation.npz, Audiobooks_data_test.npz:** Intermediate data files used during data splitting.

## Code Structure

1. **Data Preprocessing:**
   - Load preprocessed data into a DataFrame (`df`).
   - Load new input data for prediction.

2. **Model Prediction:**
   - Load the trained neural network model.
   - Predict classes for the new input data.
   - Print the predicted class.

3. **Updating DataFrame and Saving Results:**
   - Update the DataFrame with predicted classes.
   - Save the updated DataFrame to a new CSV file (`Audiobooks_data_pt.csv`).

## Usage

1. Ensure all required dependencies are installed (`tensorflow`, `numpy`, `pandas`, `scikit-learn`).
2. Place the preprocessed data file (`Audiobooks_data_pt.csv`), new input data file (`Audiobooks_data_testing.csv`), and the trained model file (`your_trained_model_path`) in the same directory as the script.
3. Execute the script to make predictions on new data and update the DataFrame.

## Dependencies

- TensorFlow
- NumPy
- Pandas
- scikit-learn

## License

This project is licensed under the [MIT License](LICENSE).
