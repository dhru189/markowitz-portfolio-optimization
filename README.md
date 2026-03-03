# markowitz-portfolio-optimization with CVXPY


## What This Notebook Does
Implements the classic Markowitz Mean-Variance portfolio 
optimization model using CVXPY — the open-source Python 
library for convex optimization.

## Covers
- Real stock data (AAPL, MSFT, GOOGL, JPM, GS, JNJ, 
  PFE, XOM, CVX) via yfinance
- Minimum Variance Portfolio
- Maximum Sharpe Ratio Portfolio
- Full Efficient Frontier with Capital Market Line
- Real-world constraints (long-only, weight caps, sector caps)
- Portfolio comparison summary table

## Why CVXPY?
Portfolio optimization is a Quadratic Program (QP).
CVXPY lets you express it exactly as the math states:

    minimize    w^T Σ w
    subject to  1^T w = 1
                w >= 0

The same workflow is used at quantitative hedge funds 
and trading desks globally.

## Tech Stack
- Python 3.10+
- CVXPY 1.8+
- yfinance, NumPy, pandas, matplotlib, seaborn

## Run It
```bash
pip install cvxpy yfinance numpy pandas matplotlib seaborn
jupyter notebook markowitz_portfolio_optimization.ipynb
```

## Author
Dhruv | Quantitative Finance + Open Source  
GSoC 2026 Applicant — CVXPY Sub-Org (NumFOCUS)  
GitHub: github.com/dhru189
