# Piotroski F-Score Strategy for Stock Selection

### 1. Get Historical Price & Financial Data of 200 Stocks in 6 Years with 1 Month Interval
- **Data Source**: 
  - The notebook begins by importing and loading historical price and financial data for 200 stocks.
  - This data spans a period of six years and is segmented into one-month intervals.
- **Data Cleaning**: 
  - The data undergoes cleaning to handle missing values, remove any inconsistencies, and ensure it is ready for analysis.
- **Data Transformation**: 
  - The notebook then transforms the data into a suitable format for subsequent analysis.
  - This includes converting dates, aligning data points, and possibly calculating additional financial metrics.

### 2. Function to Calculate Piotroski F-Score
- **Function Definition**: 
  - A function is defined to calculate the Piotroski F-Score for each stock.
  - This score is a financial metric used to determine the financial health of a company based on various accounting criteria.
- **Criteria Calculation**: 
  - The function evaluates several criteria such as profitability, leverage, liquidity, and operational efficiency.
  - Each criterion contributes to the overall F-Score.
- **Score Assignment**: 
  - The function assigns a score based on the calculated criteria, with a higher score indicating a healthier financial status.

### 3. Create Dataframe Containing Piotroski F-Score for All Stocks
- **Dataframe Initialization**: 
  - A new DataFrame is initialized to store the Piotroski F-Scores for all 200 stocks.
- **Score Calculation**: 
  - The previously defined function is applied to each stock to calculate its Piotroski F-Score.
- **Data Storage**: 
  - The calculated scores are stored in the DataFrame alongside other relevant financial data for each stock.
- **Verification**: 
  - The notebook includes steps to verify the correctness of the scores, possibly through summary statistics or sample checks.

### 4. Create Dataframe to Store Profit and Loss of Each Stock in Each Year
- **Profit and Loss Calculation**: 
  - The notebook calculates the annual profit and loss for each stock.
  - This is based on historical price data and possibly includes dividends and other financial events.
- **Dataframe Structure**: 
  - A DataFrame is created to store these profit and loss values, with each row representing a stock and each column representing a year.
- **Aggregation**: 
  - The annual profit and loss data might be aggregated to provide a clearer picture of performance over time.
- **Validation**: 
  - There are likely steps to validate these calculations, ensuring accuracy and consistency with historical data.

### 5. Dataframe to Backtest Strategy
- **Backtesting Framework**: 
  - A framework is set up to backtest the investment strategy using historical data.
  - This involves simulating trades based on predefined rules and assessing the strategy's performance.
- **Strategy Implementation**: 
  - The notebook implements the strategy, which may involve selecting stocks based on their Piotroski F-Scores and holding them for specific periods.
- **Performance Metrics**: 
  - Key performance metrics such as cumulative return, Sharpe ratio, and drawdown are calculated and stored in a DataFrame.
- **Result Analysis**: 
  - The results of the backtest are analyzed, often through visualizations such as plots of cumulative return and Sharpe ratio against the number of top stocks selected.

### Limitations
- **Data Availability**: Financial report data is limited to only three years.
- **Missing Data**: Due to missing data, the number of stocks reduced from 200 to approximately 100 after processing.
- **Date Selection**: The chosen date for post-release is January of the following year, which may not align precisely with the official financial report release dates of some stocks.
- **Applicability**: Research suggests Piotroski F-Score is more effective for small to medium-sized companies. However, due to data limitations, the stocks in this analysis include various types, potentially reducing strategy effectiveness.
- **Costs Exclusion**: The analysis does not account for transaction costs and other associated expenses.

### Conclusion
This notebook provides a comprehensive analysis of a stock selection strategy based on Piotroski F-Scores. It covers data preparation, score calculation, profit and loss analysis, and backtesting, with a focus on deriving actionable insights from historical financial data.
