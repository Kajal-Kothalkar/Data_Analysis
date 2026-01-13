# Trader Behavior vs Market Sentiment Analysis


## Project Overview
This project analyzes how trader behavior aligns or diverges from overall market sentiment (Fear vs Greed) in the Bitcoin market.

The analysis focuses on profitability, trading volume, and risk behavior using historical trader data merged with the Bitcoin Fear & Greed Index.  
All work has been performed in **Google Colab**, as per instructions.

---

## Objective
- Analyze the impact of market sentiment on trading behavior
- Study variations in:
  - Profitability (Closed PnL)
  - Trading volume (trade size in USD)
  - Risk behavior (using proxy indicators)
- Identify sentiment-driven signals to support smarter trading strategies

---

## Datasets Used

### 1. Bitcoin Market Sentiment Dataset
- Daily sentiment classification: Fear, Extreme Fear, Greed, Extreme Greed, Neutral
- Source: Fear & Greed Index

### 2. Historical Trader Dataset
- Trade-level data including:
  - Trade size (USD)
  - Closed Profit & Loss (PnL)
  - Fees
  - Trade direction and timestamps
- Source: Hyperliquid historical trader data

Both datasets were merged on a common **Date** column.

---

## Data Preparation
The following preprocessing steps were performed:
1. Converted timestamp columns to datetime format
2. Extracted date values for dataset alignment
3. Merged trader data with sentiment data
4. Verified column integrity and resolved naming inconsistencies
5. Conducted exploratory data analysis (EDA)

---

## Key Findings

### 1. Profitability vs Market Sentiment
- Greed phases show higher profit and loss variability
- Fear phases demonstrate more stable and conservative outcomes
- Indicates increased risk-taking during optimistic market conditions

### 2. Trading Volume vs Market Sentiment
- Larger average trade sizes during Greed
- Reduced trade sizes during Fear
- Reflects confidence-driven capital exposure

### 3. Risk Behavior and Leverage (Important Note)
⚠️ **Explicit leverage data was NOT provided in the dataset**

- No leverage or margin column was available
- No assumptions were made about leverage values
- Risk behavior was analyzed using **professionally accepted proxy measures**:
  - Trade size (USD exposure)
  - Profit and loss variability

This approach is commonly used in financial analytics when direct leverage data is unavailable.

---

## Hidden Trends & Signals
- Greed amplifies risk through larger positions and higher volatility
- Fear encourages capital preservation and conservative strategies
- Market sentiment can be used as a **dynamic position-sizing indicator**

---

## Limitations
- Leverage data was not available in the dataset
- Risk analysis relied on proxy indicators
- Future analysis can improve precision if leverage or margin data becomes available

---

## Tools & Technologies
- Python
- pandas, seaborn, matplotlib
- Google Colab

---

## Google Colab Notebooks
All notebooks are publicly accessible:

- **Notebook 1 (Main Analysis):**  
https://colab.research.google.com/drive/1RYqzQEsIhoRQVPB_SM-wGoYdR0m9G1-L?usp=sharing


Access setting: **Anyone with the link can view**

---


---

## Notes
- All work was completed in Google Colab
- The same directory structure is maintained locally and on GitHub
- This submission strictly follows the provided instructions

