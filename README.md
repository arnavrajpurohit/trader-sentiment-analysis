# Trader Performance & Bitcoin Market Sentiment Analysis

## Overview

This project analyzes the relationship between trader performance and Bitcoin market sentiment (Fear/Greed). It aims to uncover patterns that can guide trading strategies in Web3 markets.

## Datasets Used

- **Market Sentiment Data** (`market_sentiment.csv`):
  - Columns: `timestamp`, `value`, `classification`, `date`
  - Source: Bitcoin Fear & Greed Index

- **Trader Data** (`trader_data.csv`):
  - Columns include: `Account`, `Coin`, `Execution Price`, `Size USD`, `Side`, `Timestamp`, `Closed PnL`, etc.
  - Source: Hyperliquid

## Key Steps

1. **Data Cleaning**:
   - Parsed timestamps
   - Filtered out erroneous/unusable rows
   - Removed trades outside sentiment data range

2. **Data Merging**:
   - Joined trader data with sentiment classification on the date field

3. **Exploratory Data Analysis (EDA)**:
   - Trade volume by sentiment classification
   - Average profit/loss under Fear vs Greed conditions

4. **Insights**:
   - Trader behavior varies significantly based on sentiment.
   - Higher PnL trends during certain sentiment conditions.

## Tools & Libraries

- Python
- Pandas
- Matplotlib
- Seaborn
- Jupyter Notebook

## Folder Structure

1. Clone the repository or download the project folder.
2. Set up a Python virtual environment and install dependencies:
   ```bash
   pip install -r requirements.txt