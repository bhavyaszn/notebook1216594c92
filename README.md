** AI-Based NIFTY Stock Market Analyzer
**
This project uses machine learning to analyze intraday price behavior of NIFTY stocks and generate Buy, Hold, or Sell signals along with a confidence score.

 Project Overview

1.  Dataset: NIFTY stock data (Kaggle)
2. Task: Intraday stock analysis and signal generation
3. Approach: Supervised Machine Learning
4. Model: Random Forest Classifier

Features Used

The model goes beyond simple price change and includes:

1.  Opening vs Closing Profit/Loss
2. Intraday Volatility (% range)
3. Close position within the day’s range
4. Candle body strength (price conviction)
5. Gap percentage (overnight sentiment proxy)
6. Relative return vs market
7. Volatility structure (range-to-body ratio)
8. Z-score normalized returns
9. Market regime indicator (bullish / bearish)

AI Model

1. A Random Forest classifier is trained on engineered price-action features
2. Labels (Buy / Hold / Sell) are generated automatically based on return thresholds
The model outputs:
  ai signal: Buy / Hold / Sell
  confidence rate: Model confidence in prediction.

 Outputs

1. Opening vs Closing Profit/Loss for all companies  
2. Top 5 best-performing stocks  
3. AI-based Buy / Hold / Sell recommendations with confidence  

 Disclaimer

This project is for **educational purposes only**.  
The model is trained on single-day stock data and is **not intended for real-world trading** yet.

 🚀 How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install pandas numpy scikit-learn
