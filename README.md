# Stock Market Sentiment Analysis and Price Prediction

## Project Overview

This project explores how news sentiment impacts stock price movements for major technology companies (Apple, Google, Amazon, Tesla, Microsoft). By combining historical stock price data with sentiment analysis of related news headlines, we build a Linear Regression model to predict stock closing prices. The goal is to understand how public sentiment influences market behavior.

---

## Data Sources

- **Stock Price Data:** Daily historical prices (`Date`, `Open`, `High`, `Low`, `Close`, `Volume`) for five tech companies.  
  CSV files are located in the `data/` folder.

- **News Headlines:** News headlines related to the companies, analyzed using VADER sentiment analyzer to generate polarity scores (`compound`, `positive`, `negative`, `neutral`).

---

## Key Steps and Methodology

1. **Data Loading & Preparation**  
   Load and clean stock price CSVs, convert dates to datetime, and sort chronologically.

2. **Sentiment Analysis**  
   Use VADER from `nltk` to calculate sentiment polarity scores on news headlines.

3. **Data Integration**  
   Merge sentiment scores with stock prices by date for combined modeling data.

4. **Feature Engineering**  
   Create lagged features of stock prices and sentiment to capture temporal trends.

5. **Model Training**  
   Train a Linear Regression model using combined historical price and sentiment features.

6. **Evaluation**  
   Evaluate with Mean Squared Error (MSE) and R-squared (R²) metrics.

---

## Results

- **Mean Squared Error (MSE):** 0.0000  
- **R-squared (R²):** 1.0000  

These metrics indicate a near-perfect model fit on this dataset. However, such results may suggest data leakage or overly simple assumptions, so interpret them cautiously.

---

## How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/Balbir89/stock-market-sentiment-analysis.git
   cd stock-market-sentiment-analysis

---

2. Install dependencies:
   pip install pandas numpy matplotlib scikit-learn nltk

3. Run the Jupyter Notebook:

   Open stock_sentiment_analysis.ipynb locally or
   Use Google Colab version

---

**Project Structure**

stock-market-sentiment-analysis/
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
├── requirements.txt (optional)
└── LICENSE


---

**Acknowledgments**

Sentiment Analysis: VADER - NLTK

Stock data: From publicly available sources


---

## Author

Balbir Singh
GitHub: https://github.com/balbir89
Email: balbirbhatia.20@gmail.com

---

**Thank you for exploring this project!**

 I'm Balbir Singh, If you want, I can help you customize the placeholders (like your GitHub username or email). Just let me know!
Updated for: Balbir Singh – https://github.com/Balbir89


---

### What I did:
- Cleaned and organized sections clearly.
- Made instructions simple and concise.
- Added your GitHub link and email.
- Included how to run with cloning, installing, and running notebook.
- Highlighted project structure and results with cautions.

---

If you want, I can also help prepare a `requirements.txt` or a `.gitignore` if needed! Just let me know. Would you like me to do that then TRY ME!

