# Quantitative Investment Strategy Backtest (Long-Only) ( DON't trust this, i found a error so i fix it...)

A multi-period robust backtest analysis of a Long-Only quantitative trading strategy spanning from 2000 to 2024. The strategy evaluates performance across three distinct phases: In-Sample (Optimization), Validation (Walk-Forward), and Out-of-Sample (Forward Testing).
## 📊 Comprehensive Performance Metrics

| Metric | In-Sample (IS) <br> (2000 ~ 2014) | Validation (Val) <br> (2014 ~ 2020) | Out-of-Sample (OOS) <br> (2020 ~ 2024) |
| :--- | :---: | :---: | :---: |
| **Trading Direction** | Long-Only | Long-Only | Long-Only |
| **Data Period (Years)** | 14.99 Years | 7.00 Years | 5.00 Years |
| **Initial Capital** | \$10,000,000.00 | \$10,000,000.00 | \$10,000,000.00 |
| **Final Value** | \$55,076,868.89 | \$30,215,791.61 | \$41,959,362.31 |
| **CAGR** | 12.05% | 17.13% | **33.25%** |
| **MDD** | -38.66% | -38.45% | **-16.81%** |
| **Sharpe Ratio** | 0.444 | 0.517 | **1.069** |
| **BUY Counts** | 11 | 5 | 2 |
| **SELL Counts** | 11 | 4 | 2 |

## 🔍 Key Findings

* **No Overfitting Signs:** The strategy shows higher efficiency in unseen data segments. The Sharpe Ratio improves from 0.444 (IS) to 0.517 (Val), and peaks at **1.069** during the final Out-of-Sample period.
* **Exceptional Recent Regime Adaptation:** During the volatile 2020–2024 macro regime, the system achieved a **33.25% CAGR** while suppressing the Maximum Drawdown (MDD) to just **-16.81%**.
* **Ultra-Low Turnover:** Executing only 2 round-trips over the last 5 years indicates a pure macro trend-following framework with negligible friction, transaction costs, or slippage decay.

## 💬 Q&A

**Q: Is Total Return (TR / dividend reinvestment) applied to this backtest?**  
**A:** No, it is not applied.

**Q: Did you factor in trading fees and slippage?**  
**A:** Yes, realistic transaction costs are strictly accounted for in the backtest settings as follows:
* `FEE = 0.0005` (0.05%)
* `SLIPPAGE = 0.0005` (0.05%)

**Q: Why are the OOS (Out-of-Sample) results so much better? Did you accidentally mix up the dates with the In-Sample (IS) data?**  
**A:** To be completely honest, I have no idea either! Why on earth did that specific period perform so insanely well? (But hey, no dates were mixed up!)

---
**Author:** Just a regular 8th-grade middle schooler 
*Written by Gemini *
