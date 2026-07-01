# 12-loan-Lending-Club-Default-Analysis--EDA-

### Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on a vehicle marketplace dataset (loan_csv.csv) containing 39,717 peer-to-peer loan     records. The analysis focuses on understanding loan characteristics, customer profiles, financial risk signals, and identifying indicators that distinguish successful loans from defaults.
  
The target variable analyzed is loan_status, which highlights loans that have been "Fully Paid" versus those that have been "Charged Off" (defaulted).


### Business Problem
Credit risk and consumer loan defaults cause significant financial losses to lending platforms and financial institutions. Since predicting whether a borrower will default is a major operational challenge, data-driven credit risk assessment is vital.

  * This project aims to answer critical business questions such as:
  
  * What is the structural breakdown and default rate within the loan portfolio?
  
  * Does the requested loan amount significantly impact the likelihood of default?
  
  * How do interest rates correlate with the risk of a loan being charged off?
  
  * Does historical housing stability (home ownership) affect payment performance?
  
  * What primary financial purposes lead borrowers to high-risk loan structures?
  
  * How accurately do internal risk classifications (Grades A-G) predict actual default behavior?


### Dataset Information
  * The dataset contains information about 39,717 consumer loans, consisting of 111 raw features including:
  
  * Financial Metrics (Loan amount, funded amount, monthly installments, interest rates)
  
  * Borrower Profiles (Annual income, employment length, home ownership type)
  
  * Risk Indicators (Loan grade, sub-grade, debt-to-income ratio)
  
  * Target Metric (loan_status: 0 = Fully Paid, 1 = Charged Off)


### Project WorkflowData
  * Architecture Review: Checking data shapes, data types, and running structural completeness checks.
  
  * Data Cleaning: Removing columns with $>50\%$ missing values, filtering out active ("Current") loans, and dropping non-analytical attributes.
     
  * Univariate Analysis: Analyzing individual spreads for loan amounts, interest rates, annual income, and loan purposes.
  
  * Bivariate Analysis: Evaluating target interactions between loan status and financial risk indicators.
  
  * Categorical Matrix Evaluations: Segmenting default behavior across vehicle financing goals, employment benchmarks, and grades.
    
  * Business Problem Decomposition: Transforming data observations into risk management workflows.
    
  * Action Plan Suggestions: Delivering data-backed guidelines for safer underwriting margins.


## Tools Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook


## Key Analysis Performed

### Data Cleaning

* High-Null Exclusion (Dropped columns with $>50\%$ missing data)
* Irrelevant Attribute Removal (Removed IDs, URLs, descriptions, and text titles)
* Target Binarization (Mapped "Fully Paid" to 0 and "Charged Off" to 1; excluded ongoing loans)
* Text Token Refinement (Cleaned and parsed employment length into numerical continuous indicators)

### Univariate Analysis

* Portfolio-wide Default Distribution
* Continuous Distribution of Interest Rates and Loan Amounts
* Structural Breakdown of Stated Loan Purposes (e.g., Debt Consolidation)
* Categorical Housing Profile Ratios

### Bivariate Analysis

* Loan Amount Distributions across Credit Outcomes
* Impact of Interest Rate Thresholds on Default Velocity
* Grade Assignment Accuracy vs. True Charged-Off Outcomes
* Debt-to-Income (DTI) Impact on Repayment

### Business Analysis

* Core Default Drivers Matrix
* Risk-Based Pricing Integrity Assessment
* Behavioral Purpose Risk Profiling
* Portfolio Quality Assessment by Credit Tier


## Project Outcome

The analysis establishes that borrower risk profiles are strongly tied to their credit grades, with lower tiers showing significantly higher default velocities. Furthermore, debt consolidation requests dominate portfolio volume but represent a critical concentration of risk. These analytical outputs provide consumer lending teams with clear, data-driven baseline triggers to optimize standard credit tiers, balance portfolio margins, and safely expand profitable lending volume.

## How to Run This Project

###  The Quick Way (No Git Required)
1. Click the green **Code** button at the top right of this GitHub page.
2. Click **Download ZIP** and unzip the files into a folder on your computer.
3. Move your dataset (`loan_csv.csv`) into the same folder if it isn't already there.
4. Open your terminal or command prompt, navigate to that folder, and run:
   ```bash
   pip install pandas numpy seaborn notebook
   jupyter notebook


## Author

Priya Patel  
Aspiring Data Analyst  
Email: patelpriya18217@gmail.com    
GitHub: [priyapatel96140](https://github.com/priyapatel96140)  

If you like this project, feel free to give it a star!
