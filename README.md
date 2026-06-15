# Systematic RSI Momentum & Trend-Following Backtester

A Python-based, vectorized backtesting framework implementing a rule-based trading strategy that pairs momentum filters with dynamic macro trend identification. This framework tests structural alpha on historical equity data using strict risk-reward thresholds and precise exit logging.

---

## 📈 Strategy Architecture

The system is designed around two key technical criteria to ensure trades are only executed when momentum aligns with the broader market regime:

1. **Trend Filter (200-day EMA):** Dictates overall market direction. Long entries are restricted exclusively to environments where the asset price closes above the 200 EMA, protecting capital from structural bear markets.
2. **Momentum Confirmation (14-period RSI):** Tracks localized oversold and overbought conditions to time specific execution entry windows.

### ⚙️ Execution & Risk Parameters
* **Asset Class Focus:** Liquid Equities (Daily Horizon)
* **Risk-Reward Ratio:** Strict 1:2 Profile
* **Exits:** Hard Stop-Loss (SL) and Profit Target thresholds calculated deterministically upon trade entry.

---

## 🛠️ Repository Structure

```text
├── .gitignore               # Standard Python environment filter
├── LICENSE                  # MIT Open-Source Permissive License
├── README.md                # Comprehensive system documentation
├── requirements.txt         # Minimum deployment dependency stack
└── RSI_(14)_+_200_EMA_+_SL_Target (1).ipynb   # Production research & backtest notebook
