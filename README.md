# Trader Performance vs. Bitcoin Market Sentiment
### Primetrade.ai — Data Science Internship Assignment

---

## Overview

This project explores the relationship between **Bitcoin market sentiment** (Fear & Greed Index) and **trader performance** on the Hyperliquid decentralized exchange. The goal is to uncover hidden patterns and deliver actionable insights that can drive smarter trading strategies.

---

## Datasets

| Dataset | Description | Rows |
|---|---|---|
| `historical_data.csv` | Hyperliquid trader data — accounts, coins, PnL, fees, trade direction, size, timestamps | 211,224 |
| `fear_greed_index.csv` | Daily Bitcoin Fear & Greed Index — score + classification (Extreme Fear → Extreme Greed) | 2,644 |

**Period covered:** May 2023 – May 2025

---

## Key Findings

- **Extreme Greed = best performance** — highest avg PnL ($67.89/trade) and win rate (46.5%)
- **SELL during Extreme Greed is the #1 edge** — short trades average $114.58 vs $10.50 for longs — a 10.9× difference
- **Traders deploy 2.5× larger positions during Fear** — contrarian capital allocation behavior
- **Best trader** achieves 81.09% win rate consistently across all sentiment regimes
- **December 2024** was the peak month with $3.01M PnL, driven by Bitcoin's post-halving bull run
- **Total cohort PnL:** $10.30M across 32 accounts over 2 years

---

## Project Structure

```
primetrade-assignment/
│
├── primetrade_assignment.ipynb   # Main analysis notebook (34 cells)
├── historical_data.csv           # Hyperliquid trader dataset
├── fear_greed_index.csv          # Bitcoin Fear & Greed Index
└── README.md                     # This file
```

---

## Notebook Structure

| Section | Description |
|---|---|
| 1. Imports & Setup | Libraries and plot configuration |
| 2. Load & Inspect | Data shape, types, samples |
| 3. Preprocessing & Merge | Date parsing, joining datasets |
| 4. Overall Statistics | Portfolio-level summary |
| 5. Sentiment Analysis | Avg PnL and win rate by regime |
| 6. Buy vs. Sell Dynamics | Direction edge by sentiment |
| 7. Trade Sizing | Position size vs. sentiment |
| 8. Monthly PnL Trend | Time-series performance chart |
| 9. Top Coins | Best-performing assets |
| 10. Account Performance | Trader-level bubble chart |
| 11. Sentiment Heatmap | Win rate per account × sentiment |
| 12. Strategic Insights | Actionable trading recommendations |
| 13. Final Summary | Key numbers printout |

---

## How to Run

```bash
# Clone the repo
git clone https://github.com/YOUR_USERNAME/primetrade-assignment.git
cd primetrade-assignment

# Install dependencies
pip install pandas numpy matplotlib

# Launch notebook
jupyter notebook primetrade_assignment.ipynb
```

> The two CSV files must be in the same folder as the notebook.

---

## Tools & Libraries

- **Python 3.10+**
- **pandas** — data manipulation and merging
- **numpy** — numerical analysis
- **matplotlib** — all visualizations

---

## Author

**Your Name**  
📧 mani787060@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/mani-ratan-159963289)

---

*Submitted as part of the Primetrade.ai Data Science Internship application process.*
