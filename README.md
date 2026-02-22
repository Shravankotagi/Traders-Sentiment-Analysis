# 📊 Trader Behavior Analysis using Market Sentiment

## 🧠 Overview

This project analyzes how market sentiment (Fear vs Greed) influences trader behavior and performance. By combining sentiment data with historical trading activity, the goal is to uncover patterns that can inform smarter trading strategies.

---

## 🎯 Objective

* Understand the relationship between market sentiment and trader performance
* Analyze behavioral changes in different sentiment conditions
* Derive actionable trading insights

---

## 📂 Datasets

1. **Market Sentiment Data**

   * Contains Fear/Greed classification by date

2. **Trader Data (Hyperliquid)**

   * Includes trade-level information such as:

     * Account
     * Trade size (USD)
     * Side (Buy/Sell)
     * Closed PnL
     * Timestamp

---

## ⚙️ Methodology

### 1. Data Preparation

* Cleaned column names
* Converted timestamps to datetime format
* Created a common `date` column
* Filtered sentiment data to match trading dates
* Merged both datasets on date

### 2. Feature Engineering

* Created `win` column (PnL > 0)
* Computed:

  * Average PnL
  * Win rate
  * Average trade size

### 3. Analysis

* Grouped data by sentiment categories
* Compared performance metrics
* Visualized results using bar plots and box plots

---

## 📈 Key Insights

* Trader performance does not consistently improve during Greed periods; Fear showed slightly higher profitability in this dataset.
* Larger trade sizes were observed during Fear, indicating higher risk-taking behavior.
* Higher profitability during Fear may be driven by aggressive position sizing.
* Extreme Greed showed lower win rates, suggesting possible overconfidence in bullish markets.

---

## 👥 Trader Segmentation

* **High Performers** → Consistently profitable traders
* **Medium Performers** → Moderately profitable
* **Low Performers** → Loss-making traders

---

## 💡 Strategy Recommendations

* Reduce risk exposure during Fear despite higher potential returns
* Maintain disciplined trading during Greed to avoid overconfidence
* Adjust position sizing dynamically based on sentiment
* Use sentiment as a supporting indicator, not a standalone signal

---

## ⚠️ Note

The analysis is based on the available overlapping time window between trader activity and sentiment data. Expanding the time coverage could further strengthen the robustness of insights.

---

## 🛠️ Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Google Colab

---

## 🚀 How to Run

1. Upload datasets (`fear_greed_index.csv`, `historical_data.csv`)
2. Open the notebook in Google Colab
3. Run all cells step-by-step

---

## 📊 Output

* Cleaned and merged dataset
* Performance metrics by sentiment
* Visualizations:

  * Avg PnL
  * Win rate
  * Trade size
  * PnL distribution

---

## 💼 Author

**[Your Name]**
Data Science Intern Candidate

---

## ⭐ Final Note

This project demonstrates how market sentiment influences trading behavior and highlights the importance of risk management and disciplined execution in volatile markets.

---
