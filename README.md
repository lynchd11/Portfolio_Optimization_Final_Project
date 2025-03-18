# Portfolio_Optimization_Final_Project
# Portfolio Optimization with Machine Learning - LSTM Neural Network

## Project Overview

This repository contains a portfolio optimization model that combines modern portfolio theory with machine learning techniques to create optimized investment portfolios tailored to different risk profiles. The project uses historical market data to generate efficient portfolios that maximize expected returns while minimizing risk through diversification.

## Key Features

- **Multiple Risk Profile Portfolios**: Conservative, Moderate, and Aggressive investment strategies
- **Asset Allocation Optimization**: Optimal weights for different asset classes across various sectors
- **Portfolio Performance Analysis**: Expected returns, volatility, and Sharpe ratio calculations
- **Diversification Analysis**: Correlation analysis between assets to ensure proper diversification
- **Machine Learning Price Prediction**: LSTM model for forecasting asset prices
- **Portfolio Rebalancing Simulation**: Backtesting with periodic rebalancing strategies

## Key Findings

- Maximum Sharpe Ratio Portfolio has expected annual return of 12.6% with volatility of 21.6%
- Minimum Volatility Portfolio has expected annual return of 12.0% with volatility of 19.3%
- Optimal rebalancing frequency is based on backtesting results
- Asset correlations reveal effective diversification opportunities

## Technical Implementation

### Data Handling
- Historical market data fetched via yfinance
- Data preprocessing for multiple asset classes
- Combined dataframe creation for multiple stocks

### Portfolio Optimization
- Modern Portfolio Theory implementation
- Efficient frontier calculation
- Sharpe ratio optimization
- Risk-based portfolio construction

### Machine Learning Models
- LSTM model for price prediction
- Time series forecasting with sequence-to-sequence approach
- Feature engineering for improved model performance

### Visualization
- Portfolio performance charts
- Correlation heatmaps
- Efficient frontier plot
- Backtesting results visualization

## Risk Profiles

### Conservative Risk Profile
- Expected Annual Return: 8.13%
- Annual Volatility: 13.4%
- Sharpe Ratio: 0.608
- Sector Allocation: 
  - Technology: 34.0%
  - Banking: 34.0%
  - Healthcare: 30.7%

### Moderate Risk Profile
- Expected Annual Return: 8.77%
- Annual Volatility: 16.1%
- Sharpe Ratio: 0.545
- Sector Allocation:
  - Technology: 36.1%
  - Banking: 31.6%
  - Healthcare: 32.4%

### Aggressive Risk Profile
- Expected Annual Return: 9.33%
- Annual Volatility: 21.0%
- Sharpe Ratio: 0.445
- Sector Allocation:
  - Technology: 40.0%
  - Banking: 0.0%
  - Healthcare: 31.4%

## Asset Correlation Analysis

- High Correlation (>0.7): 52 pairs
- Moderate Correlation (0.4-0.7): 125 pairs
- Low Correlation (<0.4): 139 pairs

## Evaluation Metrics
- RMSE
- MSE
- MAE

## Usage

1. Clone the repository
2. Install required dependencies:
   ```
   pip install pandas numpy matplotlib seaborn yfinance scikit-learn tensorflow
   ```
3. Run the Jupyter notebook to:
   - Load and preprocess data
   - Optimize portfolios for different risk profiles
   - Generate visualizations
   - Run backtesting simulations

## Investment Recommendations

1. For conservative investors: Consider the Minimum Volatility Portfolio
2. For balanced investors: Consider the Maximum Sharpe Ratio Portfolio
3. For growth-oriented investors: Consider a portfolio weighted towards the top LSTM predicted performers
4. Optimal rebalancing frequency based on backtesting: Rebalance quarterly

## Future Enhancements

- Integration with real-time market data
- Additional machine learning models for comparison
- Interactive dashboard for portfolio visualization
- Expanded asset universe for greater diversification opportunities
- Optimization for additional constraints (e.g., ESG factors, tax efficiency)

## Technologies Used

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- scikit-learn
- TensorFlow/Keras
- yfinance
- Jupyter Notebook

## License

This project is licensed under the MIT License - see the LICENSE file for details.
