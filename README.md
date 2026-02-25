#  Risk–Return Analysis of Indian Stocks (2020–2025)

This project applies Modern Portfolio Theory to analyze five NSE stocks using Python.

---

##  Stocks Analyzed

- HDFCBANK
- ICICIBANK
- INFY
- RELIANCE
- TCS

---

# 1️ Risk vs Return

<img width="913" height="547" alt="ebe7e87e-85ea-4341-bc6e-42b5d5334b67" src="https://github.com/user-attachments/assets/d0630c09-92a8-4941-9ac6-560da4905601" />


###  Numerical Evidence

| Stock | Return | Volatility |
|---|---:|---:|
| INFY | **25.46%** | 27.86% |
| ICICIBANK | 23.33% | **31.74%** |
| TCS | 17.94% | **24.47%** |
| RELIANCE | 16.30% | 29.73% |
| HDFCBANK | 11.21% | 27.26% |

**Observation:**
- INFY delivered highest return.
- ICICIBANK carried highest risk.
- TCS had lowest volatility.

This confirms the positive risk–return relationship.

---

# 2️ Sharpe Ratio (Risk-Adjusted Performance)


Risk-Free Rate Used: 7%

| Stock | Sharpe Ratio |
|---|---:|
| INFY | **0.6628** |
| ICICIBANK | 0.5145 |
| TCS | 0.4471 |
| RELIANCE | 0.3127 |
| HDFCBANK | 0.1547 |

**Insight:**
INFY provides the highest return per unit of risk.
HDFCBANK shows weakest risk-adjusted performance.

---

# 3️ Correlation Matrix

<img width="731" height="547" alt="d2ed4ad4-acb8-403c-acc8-f3b921af5d19" src="https://github.com/user-attachments/assets/9bd9df53-71ab-4ecf-9fbb-834236976448" />


###  What It Shows

- Banking stocks (HDFCBANK & ICICIBANK) show higher correlation.
- IT stocks (TCS & INFY) also move similarly.
- Diversification benefit exists due to less-than-perfect correlation.

---

# 4️ Efficient Frontier

<img width="813" height="547" alt="797b7c81-f0ba-4b33-81da-54ef5b7b9078" src="https://github.com/user-attachments/assets/054e8e86-14db-4e6b-ae0a-363d9dc9a905" />


10,000 portfolios simulated.

###  Maximum Sharpe Portfolio

- Return: **23.89%**
- Volatility: **23.85%**

Comparison:
- Highest individual risk: 31.74% (ICICIBANK)
- Portfolio risk reduced to 23.85%

Diversification reduced overall risk.

---

# 5️ Beta (Market Sensitivity)

| Stock | Beta |
|---|---:|
| ICICIBANK | **1.29** |
| RELIANCE | 1.11 |
| HDFCBANK | 1.08 |
| INFY | 0.89 |
| TCS | 0.75 |

**Interpretation:**
- ICICIBANK is highly sensitive to market movements.
- TCS is more defensive (Beta < 1).

---

# 6️ Value at Risk (95%)

| Stock | Daily VaR |
|---|---:|
| ICICIBANK | **-2.53%** |
| INFY | -2.46% |
| HDFCBANK | -2.44% |
| RELIANCE | -2.41% |
| TCS | **-2.15%** |

TCS has the lowest extreme downside risk.
ICICIBANK carries highest tail risk.

---

#  Final Conclusion

- Higher returns generally came with higher volatility.
- INFY delivered best risk-adjusted performance (Sharpe = 0.6628).
- Portfolio optimization reduced risk from 31.74% to 23.85%.
- Diversification improved efficiency.
- Sharpe Ratio is more informative than raw return alone.

---

Full implementation available in `Project.ipynb`.
