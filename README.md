# Fraud Detection Capstone Project

## Project Overview

This capstone project focuses on building a **fraud detection model** aimed at identifying fraudulent transactions in a financial dataset. The model is designed to analyze transaction data and predict whether a transaction is legitimate or fraudulent based on various features.

## Installation Instructions

### Prerequisites

Before running the project, make sure you have the following installed:
- Python 3.8 or higher
- pip (Python package manager)

How to install the dependencies using pip or conda.
   ```bash
   pip install -r requirements.txt
   ```

### Setting Up the Environment

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/cura1994roynel-eng/fraud-detection-capstone.git
2. Navigate to the project folder:
  ```
  cd fraud-detection-capstone
  ```
3. Navigate to the project folder:
  ```
  cd fraud-detection-capstone
  ```
### Requirements
Create a `requirements.txt` file with the following (update based on your project):
  ```
pandas
numpy
scikit-learn
matplotlib
seaborn
jupyter
  ```
### Usage
## Running the Fraud Detection Model
1. Open a terminal or command prompt and navigate to the project directory.
2. To run the fraud detection script, execute the following command:
  ```
  python src/fraud_detection.py
  ```
Replace `src/fraud_detection.py` with the path to your main script.

3. Alternatively, you can open the Jupyter notebook to visualize the model's progress step by step:
  ```
  jupyter notebook
  ```
This will open the notebook in your web browser, where you can follow the model development process.

### Dataset Information
This project uses a credit card transaction dataset to train the model for fraud detection.
The dataset contains 1,048,575 rows and 24 columns. Each row represents a single transaction, and the columns capture various
attributes related to the transaction and the cardholder. The target variable is `is_fraud`, where `1` indicates a fraudulent transaction and `0` indicates a legitimate one.

Key columns in the dataset include:
- cc_num: Credit card number used in the transaction
- merchant: Name of the merchant where the transaction took place
- category: Category of the transaction (e.g., retail, services)
- amt: Amount of the transaction in dollars
- gender: Gender of the cardholder (Male/Female)
- lat/long: Latitude and longitude of the transaction location
- city_pop: Population of the cardholder's city
- trans_date_trans_time: Timestamp of the transaction
- is_fraud: Target variable, indicating whether the transaction is fraudulent (1) or legitimate (0)

Fraud Rate:
The dataset is imbalanced, with only 0.57% of transactions being fraudulent, which makes the problem challenging due to class imbalance.

### Folder Structure
The project is organized as follows:
  ```
fraud-detection-capstone/
├── README.md # Project description and instructions
├── requirements.txt # List of Python dependencies
├── .gitignore # Git ignore file
├── src/ # Source code for fraud detection model
│ ├── fraud_detection.py # Main script for fraud detection
│ └── utils.py # Helper functions
├── notebooks/ # Jupyter notebooks for exploration
│ ├── data_exploration.ipynb # Data exploration notebook
│ └── model_development.ipynb # Model development notebook
└── data/ # Folder for datasets (consider using Git LFS)
└── transaction_data.csv # Example dataset file
  ```
### Contribution Guidelines
If you'd like to contribute to this project, please fork the repository and submit a pull request with your changes. Make sure to follow these guidelines:
- Write descriptive commit messages.
- Ensure your code passes all existing tests.
- Add new tests if you introduce new features.

### Acknowledgments
- Dataset Source: This project uses the credit card transaction dataset from [https://www.kaggle.com/datasets].
The dataset is essential for training the fraud detection model and testing its accuracy in identifying fraudulent transactions.
- Libraries and Tools:
   - Scikit-learn: Used for machine learning algorithms such as Logistic Regression, Random Forest, and XGBoost.
   - XGBoost: For implementing the XGBoost algorithm, a powerful tool for classification tasks.
   - SHAP: For model interpretability, providing insights into how features affect the model’s predictions.
   - Matplotlib & Seaborn: Used for data visualization, including correlation heatmaps and performance metrics.
  ```
