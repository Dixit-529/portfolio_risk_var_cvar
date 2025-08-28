# 📊 Portfolio Risk Analysis (VaR & CVaR) on S&P 500  

## 📌 Project Overview  
This project implements **portfolio risk measurement techniques** using **Value-at-Risk (VaR)** and **Conditional Value-at-Risk (CVaR)** on a portfolio of **S&P 500 stocks**.  
The goal is to quantify downside risk, perform stress testing, and visualize risk-adjusted performance under different market conditions.  

It serves as a practical application of **quantitative risk management** techniques widely used by banks, hedge funds, and asset managers.  

---

## 🔑 Key Concepts  
- **Value-at-Risk (VaR):** Estimates the maximum expected loss at a given confidence level (e.g., 95% or 99%).  
- **Conditional VaR (CVaR):** Also called Expected Shortfall, measures the *average loss* beyond the VaR threshold (tail risk).  
- **Stress Testing:** Evaluates portfolio resilience under extreme scenarios (e.g., financial crisis, market crash).  
- **Risk-Adjusted Performance:** Combines returns with risk metrics (e.g., Sharpe ratio).  

---

## ⚙️ Methodology  
1. **Data Collection:**  
   - Daily adjusted close prices of S&P 500 stocks (via Yahoo Finance / other APIs).  
   - Portfolio created with equal weights or custom allocations.  

2. **Data Preprocessing:**  
   - Calculated daily log returns.  
   - Constructed portfolio returns using weighted sum of asset returns.  

3. **Risk Modeling:**  
   - **Historical Simulation:** Estimated VaR & CVaR directly from empirical return distribution.  
   - **Parametric Method (Variance–Covariance):** Assumed normal distribution of returns.  
   - **Monte Carlo Simulation (optional):** Generated synthetic return distributions.  

4. **Backtesting & Stress Testing:**  
   - Compared predicted VaR with actual losses to check accuracy.  
   - Simulated portfolio behavior under crisis scenarios (e.g., 2008 GFC, 2020 COVID crash).  

5. **Visualization:**  
   - Plotted return distributions, VaR cutoffs, and CVaR tail losses.  
   - Dashboard-style risk reporting in Python.  

---

## 🛠️ Tech Stack  
- **Programming:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, SciPy  
- **Optional:** yfinance (for stock data), Jupyter Notebook for visualization  

---

## 📈 Example Outputs  
- 📉 Distribution plots with **VaR thresholds** marked.  
- 📊 Time series of portfolio returns vs. VaR predictions.  
- 🚨 Stress-test results showing extreme drawdowns.  

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/Dixit-529/portfolio_risk_var_cvar.git
   cd Portfolio-Risk-Analysis
   
