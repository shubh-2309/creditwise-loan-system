# CreditWise - Loan Approval Prediction System

CreditWise is a Machine Learning project that predicts whether a loan application is likely to be approved based on applicant information. The project focuses on data preprocessing, exploratory data analysis, feature engineering, and evaluating multiple classification models.

---

## Project Overview

The objective of this project is to build a loan approval prediction model using supervised machine learning techniques. The workflow includes:

- Handling missing values
- Exploratory Data Analysis (EDA)
- Encoding categorical features
- Feature scaling
- Model training and evaluation
- Comparing multiple classification algorithms

---

## Dataset Features

The dataset contains information related to loan applicants, including:

- Applicant ID
- Gender
- Education Level
- Employment Status
- Marital Status
- Loan Purpose
- Property Area
- Employer Category
- Income-related attributes
- Loan details
- Loan Approval Status (Target Variable)

> Note: `Applicant_ID` is removed before training since it does not contribute to prediction.

---

## Data Preprocessing

The following preprocessing techniques were applied:

### Handling Missing Values

- Numerical columns → Mean Imputation
- Categorical columns → Most Frequent Value Imputation

### Feature Engineering

- Label Encoding:
  - Education Level
  - Loan Approved (Target Variable)

- One-Hot Encoding:
  - Employment Status
  - Marital Status
  - Loan Purpose
  - Gender
  - Property Area
  - Employer Category

### Feature Scaling

- StandardScaler was used to normalize numerical features before model training.

---

## Exploratory Data Analysis

The project includes:

- Loan approval distribution visualization
- Gender ratio visualization
- Correlation analysis
- Correlation heatmap of numerical features

These visualizations help identify patterns and relationships within the data.

---

## Machine Learning Models Used

The following classification models were implemented and compared:

| Model | Purpose |
|------|------|
| Logistic Regression | Baseline linear classifier |
| K-Nearest Neighbors (KNN) | Distance-based classification |
| Gaussian Naive Bayes | Probabilistic classification |

---

## Evaluation Metrics

Each model is evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score

These metrics provide a comprehensive understanding of model performance for loan approval prediction.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## Project Structure

```
CreditWise/
│
├── credit_wise.ipynb
├── loan_approval_data.csv
├── README.md
└── requirements.txt (optional)
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/CreditWise.git
```

Navigate to the project directory:

```bash
cd CreditWise
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Or install them manually:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## Running the Project

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run:

```
credit_wise.ipynb
```

Ensure that the dataset file:

```
loan_approval_data.csv
```

is present in the same directory as the notebook.

---

## Workflow

```
Dataset
   ↓
Missing Value Handling
   ↓
EDA & Visualization
   ↓
Feature Encoding
   ↓
Feature Scaling
   ↓
Train-Test Split
   ↓
Model Training
   ↓
Prediction
   ↓
Performance Evaluation
```

---

## Future Improvements

- Hyperparameter tuning
- Cross-validation
- Ensemble learning models
- Model deployment using Flask or Streamlit
- Interactive loan approval prediction interface

---

## License

This project is intended for educational and learning purposes.
