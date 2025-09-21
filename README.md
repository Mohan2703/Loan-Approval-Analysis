# Loan Approval Analysis - **EDA** *Using* **Python**

[![View Portfolio](https://img.shields.io/badge/View%20Portfolio-%23000000.svg?style=for-the-badge&logo=firefox&logoColor=#FF7139)](https://www.datascienceportfol.io/mohan_Srinivas)
[![View EDA Insights](https://img.shields.io/badge/View%20Analysis-%23000000.svg?style=for-the-badge&logo=Python&logoColor=blue)](https://github.com/Mohan2703/Loan-Approval-Analysis/blob/main/Loan%20Approval%20Analysis.ipynb)

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset Features](#dataset-features)
3. [Objective](#objective)
4. [Methodology](#methodology)
5. [Metric Calculations](#metric-calculations)
6. [Key Findings](#key-findings)
7. [Software/Hardware Requirements](#softwarehardware-requirements)
8. [Conclusion](#conclusion)

## Introduction
This project analyzes loan application data to uncover patterns in approval decisions and identify the most significant factors influencing loan approvals. The dataset consists of 45,000+ entries with 14 columns, containing demographic, financial, credit, and loan-related information about applicants.

- The goal is to predict whether a loan will be approved (1) or rejected (0), making this a binary classification problem. Insights from this analysis can help financial institutions improve decision-making, streamline approvals, and reduce default risks.

## Dataset Features
**Demographic Information**
- person_age: Age of the applicant
- person_gender: Gender of the applicant
- person_education: Highest education level
- person_emp_exp: Years of employment experience

**Financial Information**
- person_income: Annual income
- person_home_ownership: Home ownership status (rent, own, mortgage)

**Loan Information**
- loan_amnt: Loan amount requested
- loan_intent: Purpose of the loan (medical, education, business, etc.)
- loan_int_rate: Loan interest rate
- loan_percent_income: Loan amount as a percentage of annual income

**Credit Information**
- cb_person_cred_hist_length: Credit history length (years)
- credit_score: Applicant’s credit score
- previous_loan_defaults_on_file: Indicator of previous loan defaults

**Target Variable**
- loan_status: Loan approval status (1 = Approved, 0 = Rejected)

## Objective
- To identify the most common loan types and approval trends.
- To analyze factors influencing loan approval decisions.
- To examine loan default rates and risk factors.
- To assess the impact of loan approval conditions (interest rates, loan term, etc.).
- To determine the most important financial indicators for loan approval.
- To analyze loan approval trends over time and predict future demand.

## Methodology
1. **Data Collection:**
   - Data Source: Kaggle
2. **Data Preprocessing:**
    - Handle missing values (e.g., impute missing income or credit score values).
    - Remove duplicates and irrelevant data points (e.g., multiple applications by the same individual).
3. **Data Transformation:**
    - Normalize income levels, debt-to-income ratios, and credit scores for consistency.
    - Convert time-related variables (application date, loan approval date) for time-series analysis.
   - Derive additional metrics like loan eligibility score based on financial indicators.
4. **Exploratory Data Analysis (EDA):**
    - Distribution analysis of age, income, loan amount, and credit history.
    - Loan approval patterns by demographics, loan purpose, and credit score.
    - Correlation analysis between predictors and loan approval status.
5. **Data Visualization:**
    - Use Matplotlib and Seaborn to plot loan approval trends over time (e.g., approvals by month or quarter).
    - Histograms and KDE plots for demographic and financial variables.
    - Bar charts for loan approval by intent, education, and gender.
    - Trend analysis across approval rates, income groups, and credit scores.

## Metric Calculations
- **Approval Rate Calculation:** Compute loan approval rates for different loan types, demographics, and locations.
- **Risk Factor Analysis:** Identify high-risk applicant categories based on credit score, income, and debt ratios.
- **Correlation Analysis:** Analyze how different factors (e.g., credit score, income, loan amount) interact with loan approval/rejection decisions.
- **Trends by Location and Time:** Evaluate how loan approval rates vary by geographic location and over time (e.g., regional differences or seasonal variations).
- **Influence of External Factors:** Identify patterns linking economic factors (e.g., inflation, interest rates) to loan approval trends.
- **Impact of Loan Terms:** Analyze how loan terms (interest rate, repayment period) influence approval decisions and defaults.

## Key Findings
- Loan approval rates are imbalanced, with a majority of applications approved.
- Age and experience distributions are skewed, with younger applicants dominating.
- Gender distribution is fairly balanced, with slightly more male applicants.
- Most applicants either rent or have a mortgage.
- Income distribution is bell-shaped but skewed to the right.
- Loan purposes vary, with medical, education, and business loans being common.
- Applicants with higher credit scores and longer credit histories have higher approval rates.
- Previous defaults strongly reduce chances of approval.

## Software/Hardware Requirements
- **Software:**
    - Operating System: Windows/Linux/MacOS.
    - Tools: Python 3.x (Google Colab, Jupyter Notebook, or Visual Studio Code).
    - Data Analysis Libraries: Pandas, NumPy for data handling.
    - Data Visualization: Matplotlib, Seaborn, Plotly.
- **Hardware:**
    - Processor: Intel i3 or above.
    - RAM: 4GB or above.

## Conclusion
This project highlights the importance of demographic, financial, and credit-related variables in loan approval decisions. By analyzing applicant profiles and loan histories, lenders can improve risk management, optimize approval processes, and reduce defaults.

**The insights can help:**
- Financial institutions streamline approvals and reduce biases.
- Lenders personalize loan offerings for different applicant segments.
- Policymakers design fairer lending guidelines.
