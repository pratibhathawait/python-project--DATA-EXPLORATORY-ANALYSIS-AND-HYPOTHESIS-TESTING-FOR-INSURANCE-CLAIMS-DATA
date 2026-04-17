# python-project
EXPLORATORY Data ANALYSIS AND HYPOTHESIS TESTING FOR INSURANCE CLAIMS DATA
🚀 Project Overview
This project performs Exploratory Data Analysis (EDA) and Statistical Hypothesis Testing on insurance claims data by combining customer and claims datasets to create a 360-degree analytical view.

The goal is to uncover insights related to customer behavior, claim patterns, fraud detection, and business risk factors.

📂 Dataset
Two datasets were used:
claims_data.csv → Contains claim-related information
cust_data.csv → Contains customer demographic details
These datasets were merged using Customer ID to create a unified dataset.

🧹 Data Preprocessing & Cleaning
✔️ Steps Performed:
     🧹 Data Preprocessing & Cleaning
✔️ Steps Performed:
        1. Data Merge
            Combined claims and customer datasets to create a unified view
        2. Data Audit
            Checked data types and corrected inconsistencies
            Ensured alignment with business meaning
        3. Data Type Conversion
            Converted claim_amount from string to numeric
            Removed $ symbols using string operations
        4.Feature Engineering
            Created alert flag (1/0) for injury claims not reported to police
        5.Duplicate Handling
            Retained only the most recent record per customer
            Removed duplicate customer_id entries
        6.Missing Value Treatment
            Continuous variables → imputed using mean
            Categorical variables → imputed using mode
        7.Age Calculation & Categorization
            Calculated age from date of birth
            Created age groups:
                Children (<18)
                Youth (18–30)
                Adult (30–60)
                Senior (>60)

📊 Exploratory Data Analysis (EDA)
        🔍 Key Business Questions Answered:
        Average claim amount across customer segments
        Total claim amount by incident cause (filtered by date condition)
        Number of adult claims from specific states (TX, DE, AK)
        Fraudulent claims distribution across age groups
        Monthly claim trends (chronological order)

📈 Data Visualizations
      📊 Bar Charts → Claim comparisons across categories
      🥧 Pie Chart → Claim distribution by gender and segment
      📉 Line Chart → Monthly claim trends
      📊 Faceted Charts → Fraud vs non-fraud comparisons        

🧪 Hypothesis Testing
      ✔️ Tests Conducted:
      T-Test → Gender vs claim amount
      Chi-Square Test → Age category vs segment
      ANOVA → Age group vs claim amount
      Correlation Analysis → Claim count vs claim amount
                                    Adult (30–60)
Senior (>60)
