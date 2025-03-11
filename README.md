# neural-network-challenge-1
# Student Loan Risk Prediction with Deep Learning

## Overview
This project uses a deep neural network model to predict student loan repayment success. The model is designed to help a student loan refinancing company predict borrower risk and offer accurate interest rates.

---

## Data
The dataset contains information about student loan recipients, including their credit ranking and other financial details. The goal is to predict the likelihood of loan repayment based on these features.

---

## Files
- `student_loans_with_deep_learning.ipynb` — Main Jupyter Notebook containing the full workflow.
- `student_loans.keras` — Saved deep learning model.
- `student-loans.csv` — Dataset containing student loan data.

---

## Project Steps
### 1. Data Preparation
- Load the dataset into a Pandas DataFrame.
- Define the target (`y`) as the `credit_ranking` column.
- Define the features (`X`) as all remaining columns.
- Split the data into training and testing sets.
- Scale the features using `StandardScaler`.

### 2. Neural Network Model
- Created a deep neural network using TensorFlow/Keras.
- Two hidden layers:
  - First layer: 8 neurons with `relu` activation.
  - Second layer: 4 neurons with `relu` activation.
- Output layer with 1 neuron using the `sigmoid` activation function.
- Compiled with `binary_crossentropy` loss, `adam` optimizer, and `accuracy` as the evaluation metric.
- Trained the model with 50 epochs.

### 3. Model Evaluation
- Evaluated the model using the test data to measure loss and accuracy.
- Saved the trained model as `student_loans.keras`.

### 4. Predictions
- Reloaded the saved model.
- Made binary predictions on the test data.
- Generated a classification report to assess model performance.

### 5. Recommendation System Discussion
- Identified key data points required for a student loan recommendation system.
- Justified content-based filtering as the optimal method.
- Addressed real-world challenges like data privacy and fairness.

---

## Technologies Used
- Python
- Pandas
- TensorFlow/Keras
- Scikit-learn

---

## Installation
1. Clone the repository:
