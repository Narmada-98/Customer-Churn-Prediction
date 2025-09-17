# Customer Churn Prediction

## Overview

This project predicts **customer churn** using machine learning techniques on the [Telco Customer Churn dataset](https://www.kaggle.com/datasets/blastchar/telco-customer-churn). The objective is to identify customers likely to discontinue services, enabling proactive retention strategies.

## Features

* **Exploratory Data Analysis (EDA)** – Insights into customer behavior and churn patterns
* **Data Preprocessing** – Handling missing values, encoding categorical variables
* **Class Imbalance Handling** – **SMOTE**
* **Model Selection** – Comparison of Decision Tree, Random Forest, and XGBoost
* **Hyperparameter Tuning** – **Optuna** 
* **Cross-Validation** – K-Fold for robust evaluation
* **Model Evaluation** – ROC-AUC, Precision, Recall, F1-Score, and confusion matrices

## Project Structure

```text
customer-churn-prediction/
│
├── data/                         # Dataset files 
├── 1_data_exploration.ipynb      # EDA: distributions, missing values, correlations
├── 2_data_preprocessing.ipynb    # Data cleaning, encoding, SMOTE, and splitting
├── 3_modelling_and_hyperparameter_tuning.ipynb  # Cross-validation & Optuna tuning
├── 4_evaluation_and_interpretation.ipynb        # Metrics, ROC-AUC, and confusion matrices
├── models/                       # Model files
├── requirements.txt              # Dependencies
└── README.md                     # Project documentation
```

## How to Run

### 1️⃣ **Clone the repository**

```bash
git clone https://github.com/Narmada-98/Customer-Churn-Prediction.git
cd customer-churn-prediction
```

### 2️⃣ **Create a virtual environment and install dependencies**

```bash
python -m venv venv
source venv/bin/activate      # On Mac/Linux
venv\Scripts\activate         # On Windows
pip install -r requirements.txt
```

### 3️⃣ **Run the notebooks in order**

1. `1_data_exploration.ipynb` – Perform EDA and note insights
2. `2_data_preprocessing.ipynb` – Clean and prepare the data
3. `3_modelling_and_hyperparameter_tuning.ipynb` – Train and tune models
4. `4_evaluation_and_interpretation.ipynb` – Evaluate and interpret results

## Results

* **Best Model**: Random Forest (AUC ≈ 0.85)

## Technologies Used

* **Programming Language**: Python
* **Libraries**: pandas, NumPy, scikit-learn, imbalanced-learn, Optuna, seaborn, matplotlib

