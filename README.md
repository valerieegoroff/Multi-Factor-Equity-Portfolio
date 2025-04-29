# Multi-Factor-Equity-Portfolio
Factor-based stock selection model using market exposure, size, value, and momentum factors (2015–2025).

# Multi-Factor Equity Portfolio (Market, Size, Value, Momentum)

This project builds and backtests a simple multi-factor equity portfolio strategy from 2015 to 2025.

The strategy selects stocks based on four classic investment factors:
- **Market Exposure (Beta)**: Sensitivity to broad market movements
- **Size (Market Cap)**: Preference for smaller-cap companies
- **Value (P/E Ratio)**: Preference for lower-priced stocks relative to earnings
- **Momentum (12-Month Return)**: Preference for stocks with strong recent performance

All factors are standardized (z-scored) and combined into an equally weighted composite score.  
Each month, the top 5 stocks by composite score are selected and equally weighted.

## Methodology
- Pulled adjusted price data and fundamental data using `yfinance`
- Calculated Beta, Market Cap, P/E Ratio, and 12-month returns
- Standardized factor exposures and blended into a composite ranking
- Backtested portfolio performance over a 10-year period
- Plotted cumulative returns to evaluate strategy effectiveness

## Tools Used
- Python
- pandas, NumPy
- matplotlib
- yfinance

## Results
The multi-factor portfolio consistently selected a diversified set of companies based on combined risk, valuation, and momentum characteristics. The backtested performance demonstrated robust cumulative returns over the period.

This project was designed to apply fundamental quantitative investing concepts using publicly available data.
