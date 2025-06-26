# 📊 Market Sentiment vs Trader Performance Analysis

This project investigates how market sentiment impacts trading performance using two datasets: a **Bitcoin Fear & Greed Index** and **historical trader data** from Hyperliquid.

---

## 🔍 Objective

Analyze the relationship between daily market sentiment and key trading performance metrics such as:

- 💰 **Profitability (Closed PnL)**
- 📊 **Trading Volume**
- 💸 **Fees Paid**

The goal is to uncover patterns that could inform smarter trading strategies.

---

## 📁 Datasets Used

- `fear_greed_index.csv`  
  → Contains daily sentiment values and classifications (e.g., Fear, Greed, Extreme Fear)

- `historical_data.csv`  
  → Includes detailed trade logs (account, coin, side, price, size, PnL, fees, timestamps, etc.)

---

## 🧪 Key Steps

1. **Data Preparation**
   - Parse and align timestamps
   - Merge both datasets on `date`

2. **Analysis**
   - Aggregate metrics (PnL, Fee, Trade Count) grouped by sentiment classification

3. **Visualization**
   - Bar plots showing average PnL and trade activity across different sentiment types

4. **Export Results**
   - Save insights to CSV and Excel for reporting or further modeling

---

## 📦 Output Files

- `sentiment_summary.csv`
- `sentiment_summary.xlsx`

Optional visualizations (charts) can also be saved if run in a Jupyter Notebook.

---

## 📈 Sample Insight

| Sentiment      | Avg PnL | Total Fee | # Trades |
|----------------|---------|-----------|----------|
| Extreme Greed  | 67.89   | 27,030    | 39,992   |
| Fear           | 54.29   | 92,457    | 61,837   |
| Greed          | 42.74   | 63,099    | 50,303   |
| Extreme Fear   | 34.54   | 23,889    | 21,400   |
| Neutral        | 34.31   | 39,374    | 37,686   |

---

## 🛠️ Technologies Used

- Python 3
- Pandas
- Matplotlib & Seaborn
- Jupyter Notebook (optional)
- Excel export via `openpyxl`

---

   
