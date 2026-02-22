# Loan Approval Prediction Project 🏦📊

https://img.shields.io/badge/Python-3.12-blue.svg

https://img.shields.io/badge/Pandas-2.0+-green.svg

https://img.shields.io/badge/License-MIT-yellow.svg

# 📋 Project Overview

This project performs comprehensive analysis and preprocessing of loan application data to understand the key factors influencing loan approvals. Through extensive exploratory data analysis and data cleaning, we uncover valuable insights that can help financial institutions make more informed lending decisions.

# 🎯 Key Objectives

Clean and preprocess raw loan application data

Analyze patterns in applicant demographics and financial profiles

Visualize relationships between various features and loan approval status

Handle missing data using appropriate statistical techniques

Generate insights for better loan approval strategies

# 🛠️ Technologies Used

Python 3.12 - Core programming language

Pandas - Data manipulation and analysis

NumPy - Numerical computations

Matplotlib - Data visualization

Seaborn - Statistical data visualization

Jupyter Notebook - Interactive development environment

# 📊 Dataset Features

The dataset contains 614 loan applications with the following features:

Feature	Description

Loan_ID	Unique loan identifier, 
Gender	Applicant gender (Male/Female), 
Married	Marital status (Yes/No), 
Dependents	Number of dependents, 
Education	Education level (Graduate/Not Graduate), 
Self_Employed	Self-employment status (Yes/No), 
ApplicantIncome	Applicant's income, 
CoapplicantIncome	Co-applicant's income, 
LoanAmount	Requested loan amount, 
Loan_Amount_Term	Loan repayment term, 
Credit_History	Credit history (1 = good, 0 = bad), 
Property_Area	Property location (Urban/Semiurban/Rural), 
Loan_Status	Target variable (Y = Approved, N = Rejected), 

# 📈 Visualizations & Insights

1. Loan Status Distribution
422 approved (68.7%) vs 192 rejected (31.3%) applications

Insight: Majority of applications get approved

2. Gender Analysis
Male applicants dominate at 489 (79.6%)

Female applicants at 112 (18.2%)

Insight: Loan approval ratio similar across genders

3. Marital Status Impact
Married applicants: 401 (65.4%)

Single applicants: 213 (34.6%)

Insight: Married applicants have slightly higher approval rates

4. Dependents Analysis
Most applicants have 0 dependents (58.6%)

Approval rates remain consistent across all dependents categories

5. Education Factor
Graduates: 480 (78.2%)

Non-graduates: 134 (21.8%)

Key Finding: Graduates show significantly higher approval rates

6. Credit History Impact
Strongest predictor of loan approval

Applicants with good credit history have much higher approval chances

# 🔍 Key Findings

Credit History is the most influential factor in loan approval decisions

Graduate applicants have better chances of approval

Married applicants show slightly higher approval rates

Income levels show correlation with loan amounts requested

Property Area influences approval rates (Urban > Semiurban > Rural)

# 🛠️ Data Cleaning Process

The project implements comprehensive data cleaning:

Removed non-essential columns (Loan_ID)

Handled missing values:

Categorical variables: Mode imputation

Numerical variables: Median imputation

Outlier detection using boxplots

Distribution analysis of numerical features

# 📁 Project Structure

text

loan-prediction-project/

│

├── Loan_Predication_Project.ipynb     # Main Jupyter notebook

├── loan_prediction.csv                  # Dataset

├── README.md                            # Project documentation

├── requirements.txt                      # Dependencies

│

└── visualizations/                       # Generated plots
   
    ├── loan_status_pie.png
   
    ├── gender_analysis.png
   
    ├── education_impact.png
    
    └── ...

# 🚀 Getting Started

## Prerequisites

bash

Python 3.12+
pip install -r requirements.txt

## Installation

### Clone the repository

bash

git clone https://github.com/Princechaudhary22/loan-prediction-project.git

cd loan-prediction-project

### Install dependencies

bash

pip install pandas numpy matplotlib seaborn jupyter

### Run the notebook

bash

jupyter notebook Loan_Predication_Project.ipynb

# 📊 Sample Code

 ## python

  import pandas as pd

  import seaborn as sns

  import matplotlib.pyplot as plt

 ## Load and explore data

  df = pd.read_csv('loan_prediction.csv')

  df.drop(columns="Loan_ID", inplace=True)

 ## Visualize loan status distribution

  sns.countplot(x='Loan_Status', data=df)

  plt.title('Loan Approval Distribution')

  plt.show()

# 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

# 🙏 Acknowledgments

Dataset source

Inspiration from real-world lending practices

Open-source community for amazing tools

# ⭐ If you found this project helpful, please consider giving it a star!
