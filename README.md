# Stock Sentiment Analysis and Stock Price Prediction

## Project Overview

This project investigates the relationship between news sentiment and stock price movements for major technology companies. Using historical stock data combined with sentiment analysis from related news headlines, we build a predictive model that estimates stock closing prices. The aim is to explore how public sentiment, as reflected in news, influences stock market behavior.

---

## Data Sources

- **Stock Price Data:** Historical daily stock prices for Apple, Google, Amazon, Tesla, and Microsoft.
  - Data includes columns such as `Date`, `Close`, `High`, `Low`, `Open`, and `Volume`.
  - Source CSV files are located in the `data/` folder.
  
- **News Headlines:** Headlines related to each company are analyzed for sentiment using the VADER sentiment analyzer to generate polarity scores (`compound`, `positive`, `negative`, `neutral`).

---

## Key Steps and Methodology

1. **Data Loading and Preparation**
   - Load daily stock price data from CSV files.
   - Convert date columns to datetime format for proper time-series handling.
   - Sort data chronologically.

2. **Sentiment Analysis**
   - Use the VADER sentiment analysis tool from the `nltk` library.
   - Calculate sentiment polarity scores for news headlines.
   - Aggregate sentiment scores by date.

3. **Data Integration**
   - Merge daily stock data with daily aggregated sentiment scores based on dates.
   - Align sentiment data with stock prices for modeling.

4. **Feature Engineering**
   - Create lagged features for both stock closing prices and sentiment scores to capture temporal trends.
   - Handle missing data by dropping or imputing where necessary.

5. **Model Training**
   - Use a Linear Regression model to predict stock closing prices.
   - Train the model on combined features of historical stock prices and sentiment polarity.

6. **Evaluation**
   - Evaluate the model using Mean Squared Error (MSE) and R-squared (R²) metrics.
   - Visualize regression results and feature relationships.

---

## Results

- **Mean Squared Error (MSE):** 0.0000  
- **R-squared (R²):** 1.0000  

These results indicate a near-perfect fit on the provided dataset, suggesting that the model captures the relationship between sentiment and stock price exceptionally well. However, such perfect scores are unusual in real-world financial modeling and may indicate data leakage or overly simplistic modeling assumptions.

---

## Usage Instructions

### Prerequisites

- Python 3.7 or higher
- Required libraries:
  ```bash
  pip install pandas numpy matplotlib scikit-learn nltk

---

**Project Structure**
stock-sentiment-analysis/
│
├── data/
│   ├── apple.csv
│   ├── google.csv
│   ├── amazon.csv
│   ├── tesla.csv
│   └── microsoft.csv
│
├── stock_sentiment_analysis.ipynb
├── README.md
└── requirements.txt (optional)

---

**Acknowledgments**

Sentiment analysis powered by the VADER tool from the nltk library.

Stock price data sourced from publicly available datasets.

---

Contact Me, I'm Balbir Singh

Email: balbirbhatia.20@gmail.com

---

**Thank you for exploring this project!**

If you want, I can help you customize the placeholders (like your GitHub username or email). Just let me know!
Updated for: Balbir Singh – https://github.com/Balbir89

---

## Author

**Balbir Singh**  
GitHub: [https://github.com/balbir89](https://github.com/balbir89)


