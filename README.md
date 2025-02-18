## Equity Portfolio Stress Testing Project

### Overview:
This project focuses on performing a stress test on an equity portfolio using macroeconomic variables (MEVs) from the Federal Reserve's stress testing for bank capital (CCAR). The goal is to predict the average performance of a portfolio in hypothetical adverse scenarios using a reliable model for out-of-sample prediction and robustness across different scenarios. Key tasks include forming a portfolio, preparing data, performing regression analysis, and comparing results under baseline and adverse scenarios.

## Portfolio Construction

We selected at least 15 individual stocks for our portfolio, ensuring diversification across sectors. Each stock's weight in the portfolio was carefully chosen to reflect the overall risk and return preferences. The data for stock returns, market returns, and Fama-French factors were obtained from various sources including the WRDS database, with some additional factors downloaded from Professor French’s database.

## Data Transformation and Preprocessing

The data used for the stress test included monthly stock returns (1963-2023), MEVs, and macroeconomic factors. We performed stationarity tests on all MEVs and transformed the data as needed (e.g., first differencing or log transformations). Missing data was addressed by appropriate imputation techniques, particularly when grouping stocks into sub-portfolios. We also created summary statistics for all data used in the analysis.

## Stress Testing with Fama-French Model

Using the Fama-French three-factor model, we analyzed the impact of chosen MEVs on stock returns. We performed linear regressions to assess how macroeconomic variables affected Fama-French factors, with results reported including point estimates, standard deviations, and goodness-of-fit.

### Scenario Selection

We selected a subset of MEVs to represent severely adverse scenarios based on economic rationale, focusing on factors like high unemployment rates, financial instability, and sharp market declines. These MEVs were used to model the impact of a potential economic downturn on the portfolio’s performance.

### Model Results

We ran regressions using data from all periods and from “stressed times” (periods of financial instability). The results provided insights into the portfolio's performance under both supervisory baseline and severely adverse scenarios. We plotted the projected performance for the next five quarters and discussed the potential economic implications of the results, assuming an Asset Under Management (AUM) of $100 million.

## Generalized Factor Model for Stress Testing

We proposed a generalized factor model to predict stock returns, using additional factors and lagged values of MEVs. Our model aimed to provide more flexibility in modeling and estimating the impact of macroeconomic shocks. We compared our predictions with those from the Fama-French model and analyzed the differences in robustness, goodness-of-fit, and back-testing results.

### Model Risk and Reliability

We discussed potential model risks such as complexity, overfitting, and issues like the Law of Small Numbers. These risks were taken into account during model construction and testing to ensure the reliability of the projections.

## Conclusion

The stress testing analysis provided valuable insights into the portfolio's sensitivity to macroeconomic shocks. By comparing baseline and severely adverse scenarios, we highlighted the risks associated with each scenario and presented a more comprehensive view of potential portfolio performance under stress.

### Requirements:
- Data: Excel files with historical return data (1963–2023) for 20 stocks, market returns, Fama-French factors, and MEVs from the Federal Reserve.
- Tools: Statistical software (e.g., Excel, Python, R) for regression analysis, data processing, and model construction.

