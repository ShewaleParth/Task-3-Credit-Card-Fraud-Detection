# Credit Card Fraud Detection using Random Forest Classifier

This script uses a Random Forest Classifier to predict fraudulent credit card transactions based on features provided in the dataset.

## Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn (sklearn)

## Dataset

The dataset used (`creditcard.csv`) contains transactions made by credit cards in September 2013 by European cardholders. It contains a mix of numerical features that have undergone PCA transformation due to privacy concerns.

## Setup

1. **Download the dataset**: Ensure the `creditcard.csv` file is placed in the same directory as this script or update `file_path` variable in the script to point to its location.

2. **Install dependencies**: Make sure you have installed all the necessary Python libraries mentioned in the requirements.

## Usage

1. **Run the script**: Execute the script in your Python environment.

   ```bash
   python credit_card_fraud_detection.py
   Replace credit_card_fraud_detection.py with the actual filename where you have saved this script.

2. **Output**: The script will output the evaluation metrics of the model including Accuracy, Precision, Recall, and F1 Score.
## Evaluation Metrics
1. **Accuracy**: Measures the overall correctness of the predictions.
2. **Precision**: Measures the proportion of true positive predictions (fraudulent transactions) among all positive predictions made.
3. **Recall**: Measures the proportion of true positive predictions (fraudulent transactions) among all actual positive instances.
4. **F1 Score**: Harmonic mean of Precision and Recall, providing a single metric to evaluate the model's performance.
## Notes
1. The dataset is highly imbalanced with the majority of transactions being non-fraudulent. Therefore, evaluation metrics like Precision, Recall, and F1 Score are more informative than Accuracy.

2. This script uses train_test_split to split the dataset into training and testing sets. Adjust test_size parameter for different split ratios.

3. The RandomForestClassifier is initialized with 100 decision trees (n_estimators=100). You can adjust this parameter based on your computational resources and desired model performance.
