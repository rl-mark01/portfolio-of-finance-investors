# 📈 Financial Portfolio Optimization Using Linear Programming (LP)

This project implements a **financial portfolio optimization framework based on Linear Programming (LP)**.
Assets are allocated according to **investor risk preferences** to maximize after-tax returns
while satisfying realistic risk constraints.

---

## 🔍 Project Overview

- **Methodology**: Linear Programming (LP)
- **Investment Horizons**: 1-year, 3-year, 5-year
- **Investor Types**:
  - Conservative
  - Neutral
  - Aggressive
- **Assets Considered**:
  - Stocks
  - Long-term Bonds
  - Short-term Bonds
  - Gold
  - Cash (Risk-Free Asset)

Each portfolio is optimized based on the investor’s risk tolerance.

---

## 🧠 Optimization Strategy

The optimization is conducted in two stages:

### 1️⃣ Cash Allocation (Risk Hedging Stage)
- Determines the optimal cash ratio to hedge downside risk
- Risk constraints vary by investor type
- Ensures volatility and maximum drawdown (MDD) remain within predefined thresholds

### 2️⃣ Asset Allocation (Return Optimization Stage)
- Allocates remaining capital among risky assets
- Objective:
  - Maximize **after-tax expected return**
- Subject to:
  - Volatility constraints
  - Maximum drawdown (MDD) constraints
  - Asset weight summation constraint

---

## ⚙️ Mathematical Model

- **Decision Variables**: Asset allocation weights
- **Objective Function**:
  - Maximize after-tax portfolio return
- **Constraints**:
  - Sum of asset weights equals 1
  - Volatility limit by investor type
  - Maximum drawdown (MDD) limit by investor type
- **Solver**:
  - IBM DOcplex (CPLEX)

---

## 🧪 Technologies Used

- Python
- Linear Programming (LP)
- IBM DOcplex / CPLEX
- NumPy

---

## 📌 Key Takeaways

- Investor-type-specific portfolio optimization
- Explicit risk control using volatility and MDD
- Practical application of linear programming to financial decision-making

---
