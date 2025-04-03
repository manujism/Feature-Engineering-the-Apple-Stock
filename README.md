# Feature-Engineering-the-Apple-Stock


**This project aims to perform a comprehensive Feature Engineering and Exploratory Data Analysis (EDA) on Apple ( AAPL ) stock data.**

------

Feature engineering is the process of selecting, transforming, and creating relevant input variables (features) that improve the predictive power of a machine learning model. In stock price prediction, good features can help capture market trends, patterns, and signals.

------

**2. Methodology**

**Data Collection:** Historical stock data for Apple was fetched using the yfinance API.

**Data Preparation:** Reset the index to use Date as a column and then Verify and convert Date to datetime format.

**Feature Engineering:** Derived various stock-related features for analysis.

**Visualization:** Analyzed trends using matplotlib and seaborn.


------

**3. EDA and Feature Engineering**

**1. Daily Returns:** Calculated percentage change in daily closing prices.

**2. Price Change:** Difference in closing prices between consecutive days.

**3. 5-Day Moving Average:** Average closing price over a rolling 5-day window.

**4. High-Low Spread:** Difference between daily high and low prices.

**5. Volatility:** Standard deviation of daily returns over a 20-day rolling window.

**6. 10-Day Simple Moving Average (SMA):** Average closing price over a rolling 10-day window.

**7. 10-Day Exponential Moving Average (EMA):** Weighted average of closing prices over 10 days, giving more weight to recent days.

**8. Lagged Features:**
  
  Lagged Closing Price: Previous day's closing price.
  
  Lagged Returns: Previous day's returns.

**9. Temporal Features:**

  Day of the Week: Weekday (0=Monday, ..., 6=Sunday).
    
  Month: Month of the year.
    
  Year: Extracted from the Date.

**10. Cumulative Returns:** Total compounded return over the period.

**11. Scaled Volume:** Daily trading volume scaled for visualization (in millions).


-------

**5. Results**


**1. Daily Returns:** Highlighted the variability in stock price movements.

**2. Volatility:** Showed periods of high/low market activity.

**3. Moving Averages:** Demonstrated short-term trends and price smoothness.

**4. Temporal Features:** Identified trends based on the day of the week and month.

**5. Cumulative Returns:** Illustrated the growth trajectory of the stock.

**6. Heatmap:** Showed strong correlations between price features (e.g., Adj Close vs Close).

-----

**6. Limitations and Future Scope**

**Limitations**

  1. Focused only on Apple stock; results may not generalize to other securities.
    
  2. Temporal scope limited to 1 year.
    
  3. Does not include macroeconomic factors or market-wide trends.


**Future Scope**

  1. Expand analysis to multiple stocks and perform comparative analysis.
  
  2. Build predictive models using the engineered features:
  
  3. Predict future prices using regression models.
  
  4. Classify price movements using machine learning classifiers.
  
  5. Integrate sentiment analysis using news data.
  
  6. Use advanced techniques like GARCH for volatility modeling.







