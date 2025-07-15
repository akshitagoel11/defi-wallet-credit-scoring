# Zeru Credit Scoring System

##  Overview

This project analyzes on-chain behavior of Ethereum wallets interacting with Aave V2 and assigns a credit score (0–1000) based on responsible DeFi activity.

##  Features Extracted

- Number of deposits, borrows, repayments, withdrawals, and liquidations
- Borrow-to-repay ratio
- Total number of transactions

##  Scoring Logic

- Base score: 400
- +5 per deposit
- +10 per repayment
- -2 per borrow
- -100 per liquidation
- -100 penalty if borrow > repay significantly

##  Output

- `wallet_scores.csv`: Wallet address + credit score
- `score_distribution.png`: Histogram of credit scores

##  How to Run

1. Install requirements: `pip install pandas seaborn matplotlib`
2. Run `notebook.ipynb` or main script.
3. View results and graphs.
