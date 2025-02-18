## Equity Portfolio Stress Testing Project

### Overview:
This project focuses on performing a stress test on an equity portfolio using macroeconomic variables (MEVs) from the Federal Reserve's stress testing for bank capital (CCAR). The goal is to predict the average performance of a portfolio in hypothetical adverse scenarios using a reliable model for out-of-sample prediction and robustness across different scenarios. Key tasks include forming a portfolio, preparing data, performing regression analysis, and comparing results under baseline and adverse scenarios.

### Steps:

#### 1. **Portfolio Formation & Data Processing (50 points)**:
   - **Portfolio Selection (5 points)**:
     - Choose at least 15 stocks for the portfolio, avoiding short positions, and ensure the portfolio remains static (not dynamically rebalanced).
     - Provide rationale for stock selection.
   - **Missing Data Handling (15 points)**:
     - Process missing data, especially when grouping stocks by industry or size for prediction models.
     - Describe your strategy for handling missing data.
   - **Data Sources (5 points)**:
     - Document the sources of data used outside of the provided files.
   - **Stationarity Test (15 points)**:
     - Perform stationarity tests on all MEVs and transform the data as needed (e.g., first differences, logs).
   - **Summary Statistics (10 points)**:
     - Provide summary statistics of all data used, including time periods.

#### 2. **Stress Testing Using Fama-French Three-Factor Model (80 points)**:
   - **MEV Selection (20 points)**:
     - Choose a subset of MEVs to represent severely adverse scenarios and justify the choice based on economic reasoning.
   - **Fama-French Model Results (20 points)**:
     - Report results of the Fama-French three-factor model (Market, SMB, HML) for portfolio stress testing.
   - **Impact of MEVs on Fama-French Factors (10 points)**:
     - Use linear regression to identify the impact of MEVs on Fama-French factors across all data.
   - **Impact During Stressed Times (15 points)**:
     - Perform regression on “stressed times” (economic downturns, financial instability) to analyze MEV impact during severe scenarios.
   - **Predict Portfolio Performance (10 points)**:
     - Predict portfolio performance under supervisory baseline vs. severely adverse scenarios for 2024Q1–2025Q1.
   - **Error Bands Discussion (5 points)**:
     - Conceptually discuss ways to provide error bands for these projections.

#### 3. **Construct Your Own Model for Stress Testing (60 points)**:
   - **Model Plan (10 points)**:
     - Provide a detailed plan for the prediction model, including choices for factors and regressions.
   - **Intermediate Results (20 points)**:
     - Report intermediate results that are useful for further analysis.
   - **Model Comparison (20 points)**:
     - Compare your model with the Fama-French model from Section 4 in terms of goodness-of-fit, robustness, back-testing, and projection differences.
   - **Model Risk Discussion (10 points)**:
     - Discuss potential risks (complexity, overfitting, small sample sizes) that could affect the reliability of the model.

### Requirements:
- Data: Excel files with historical return data (1963–2023) for 20 stocks, market returns, Fama-French factors, and MEVs from the Federal Reserve.
- Tools: Statistical software (e.g., Excel, Python, R) for regression analysis, data processing, and model construction.

