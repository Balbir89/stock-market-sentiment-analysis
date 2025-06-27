# Stock Sentiment Analysis and Stock Price Prediction

## Project Overview

This project explores how news sentiment impacts stock prices for major tech companies by analyzing historical price data alongside sentiment from news headlines. A predictive model is built to estimate closing prices based on public sentiment trends.

---

## Data Sources

- **Stock Price Data:** Historical daily stock prices for Apple, Google, Amazon, Tesla, and Microsoft.
- Stock Price Data
-Daily price data for:
-Apple, Google, Amazon, Tesla, and Microsoft
-Includes: Date, Close, High, Low, Open, and Volume
-Located in the data/ directory
  
- **News Headlines:** Headlines related to each company are analyzed for sentiment using the VADER sentiment analyzer to generate polarity scores (`compound`, `positive`, `negative`, `neutral`).

---

## Project Workflow

Load Stock Data

- Read CSVs, convert dates, and sort for time-series accuracy.

Analyze Sentiment

- Apply VADER to headlines and aggregate daily scores.

Merge & Align

- Combine stock and sentiment data by date.

Feature Engineering

- Add lagged features (previous day’s stock/sentiment) to model temporal trends.

Model Training

- Fit a Linear Regression model using sentiment and historical stock features.

Evaluation

- Evaluate using MSE and R², and visualize the regression outcome.

---

## Results

- **Mean Squared Error (MSE):** 0.0000  
- **R-squared (R²):** 1.0000  

The model shows perfect prediction on the dataset — highly accurate but may indicate overfitting or data leakage.

---

## 🛠️ How to Run

Run the project easily on Google Colab:  
[Open notebook on Google Colab](https://colab.research.google.com/gist/Balbir89/7eda694a4fecb656fb92e6a49d6dd67a/stock_sentiment_analysis.ipynb#scrollTo=a319ymQs68q_)

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

Sentiment Analysis: VADER - NLTK

Stock data: From publicly available sources

---

**Thank you for exploring this project!**

 I'm Balbir Singh, If you want, I can help you customize the placeholders (like your GitHub username or email). Just let me know!
Updated for: Balbir Singh – https://github.com/Balbir89

---

## Author

**Balbir Singh**  
GitHub: [https://github.com/balbir89](https://github.com/balbir89)

---

Feel free to clone, explore, and adapt this project for your own financial analysis experiments.
Thanks for visiting!
