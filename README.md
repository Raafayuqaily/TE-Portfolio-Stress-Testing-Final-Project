## FOMC Statement Scraping and Sentiment Analysis Project

### Overview:
This project involves scraping the text of Federal Open Market Committee (FOMC) statements from January 2000 to the present, analyzing their tone, and examining the impact of FOMC decisions on the financial markets. Key tasks include sentiment analysis of the statements, computing changes in Federal Funds Rate (FFR) targets, and performing regression analyses to evaluate the influence of FOMC statements on bond and stock markets.

### Steps:
1. **Scraping FOMC Statements**:
   - Use BeautifulSoup to scrape statements from:
     - 2019-2024: [FOMC Calendars](https://www.federalreserve.gov/monetarypolicy/fomccalendars.htm)
     - 2000-2018: [FOMC Historical Years](https://www.federalreserve.gov/monetarypolicy/fomc_historical_year.htm)
   - Extract URLs, download, and clean the text by removing HTML tags.
   - Extract release dates from URLs and calculate word count statistics (mean, median, standard deviation).

2. **Sentiment Analysis**:
   - Follow Tadle (2022) to analyze tone:
     - Tokenize text using `nltk.sent_tokenize`.
     - Identify hawkish and dovish keywords, adjust for negation.
     - Compute and aggregate sentiment scores for each statement.
     - Plot sentiment scores over time.

3. **Federal Funds Rate Data**:
   - Retrieve FFR data from FRED (DFEDTAR and DFEDTARU).
   - Calculate FFR changes on each FOMC meeting date and plot alongside sentiment scores.

4. **Alternative Sentiment Measurement**:
   - Critique Tadle (2022) and propose a new method for measuring hawkish/dovish tone.

5. **Regression Analysis**:
   - Perform regressions to analyze the relationship between sentiment, FFR changes, and bond market responses:
     - Use FRED data (EFFR, DGS1MO, DGS10) to compute bond changes on FOMC meeting dates.
     - Analyze results and select the best regression specification.

6. **Stock Market Impact**:
   - Analyze FOMC sentiment impact on stock markets using industry return data from the French Data Library.
   - Regress industry returns on FOMC sentiment for each meeting date and compute the monetary policy risk premium.
   - Perform monthly regressions from Jan. 2000 to Aug. 2024 to assess long-term effects.

### Requirements:
- Python (BeautifulSoup, NLTK, Pandas, Matplotlib)
- Access to FRED and French Data Library datasets.

