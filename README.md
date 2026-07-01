# 12-loan-Lending-Club-Default-Analysis--EDA-

### Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a vehicle marketplace dataset (loan_csv.csv) containing 39,717 peer-to-peer loan records. The analysis focuses on understanding loan characteristics, customer profiles, financial risk signals, and identifying indicators that distinguish successful loans from defaults.

The target variable analyzed is loan_status, which highlights loans that have been "Fully Paid" versus those that have been "Charged Off" (defaulted).


### Business Problem
Credit risk and consumer loan defaults cause significant financial losses to lending platforms and financial institutions. Since predicting whether a borrower will default is a major operational challenge, data-driven credit risk assessment is vital.

This project aims to answer critical business questions such as:

What is the structural breakdown and default rate within the loan portfolio?

Does the requested loan amount significantly impact the likelihood of default?

How do interest rates correlate with the risk of a loan being charged off?

Does historical housing stability (home ownership) affect payment performance?

What primary financial purposes lead borrowers to high-risk loan structures?

How accurately do internal risk classifications (Grades A-G) predict actual default behavior?


### Dataset Information
The dataset contains information about 39,717 consumer loans, consisting of 111 raw features including:

Financial Metrics (Loan amount, funded amount, monthly installments, interest rates)

Borrower Profiles (Annual income, employment length, home ownership type)

Risk Indicators (Loan grade, sub-grade, debt-to-income ratio)

Target Metric (loan_status: 0 = Fully Paid, 1 = Charged Off)


### Project WorkflowData
  1. Architecture Review: Checking data shapes, data types, and running structural completeness checks.
  
  2. Data Cleaning: Removing columns with $>50\%$ missing values, filtering out active ("Current") loans, and dropping non-analytical attributes.
     
  3. Univariate Analysis: Analyzing individual spreads for loan amounts, interest rates, annual income, and loan purposes.
  
  4. Bivariate Analysis: Evaluating target interactions between loan status and financial risk indicators.
  
  5. Categorical Matrix Evaluations: Segmenting default behavior across vehicle financing goals, employment benchmarks, and grades.
    
  6. Business Problem Decomposition: Transforming data observations into risk management workflows.
    
  7. Action Plan Suggestions: Delivering data-backed guidelines for safer underwriting margins.


### Tools Used
  
  Python
  Pandas
  NumPy
  Matplotlib
  Seaborn
  Jupyter Notebook
  

## Key Analysis Performed

### Data Cleaning
  High-Null Exclusion (Dropped columns with $>50\%$ missing data)
  Irrelevant Attribute Removal (Removed IDs, URLs, descriptions, and text titles)
  Target Binarization (Mapped "Fully Paid" to 0 and "Charged Off" to 1; excluded ongoing loans)
  Text Token Refinement (Cleaned and parsed employment length into numerical continuous indicators)

### 

