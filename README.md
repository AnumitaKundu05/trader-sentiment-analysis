# 📊 Trader Behavior vs Market Sentiment Analysis

## 📌 Overview
This project analyzes the relationship between **market sentiment (Fear vs Greed)** and **trader performance & behavior** using Hyperliquid trading data.

The goal is to identify patterns that can inform **better trading strategies**.

---

## ⚙️ Dataset
Two datasets were used:

1. **Market Sentiment Data**
   - Fields: timestamp, classification (Fear, Greed, etc.)

2. **Trader Data**
   - Fields: account, execution price, size, side, closed PnL, timestamp, etc.

---

## 🧹 Data Preparation
- Converted timestamps to proper datetime format
- Normalized timestamps to daily level
- Aggregated sentiment to one value per day
- Merged datasets on date
- Handled missing values and verified data integrity

---

## 🧠 Feature Engineering
Created key metrics:
- Profit/Loss (PnL)
- Win/Loss indicator
- Trade frequency
- Trade size (USD)
- Trader segmentation:
  - Frequent vs Casual traders
  - Winners vs Losers

---

## 📈 Analysis

### 1. Performance vs Sentiment
- **Greed → Higher profitability (~77.8)**
- **Fear → Lower profitability (~50.0)**

👉 Traders perform better during bullish conditions.

---

### 2. Behavioral Patterns

#### 🔹 Trade Frequency
- Higher during Fear → reactive behavior

#### 🔹 Long/Short Bias
- SELL trades dominate in both conditions  
→ Indicates profit booking / defensive strategy

#### 🔹 Trade Size
- (Based on analysis) varies with sentiment

---

### 3. Trader Segmentation

#### 🔹 Frequent vs Casual
- **Casual traders outperform frequent traders**
→ Overtrading reduces profitability

#### 🔹 Winners vs Losers
- Winners maintain consistent positive returns

---

## 💡 Key Insights

1. Greed-driven markets produce higher profits  
2. Fear increases trading activity (panic/overreaction)  
3. Overtrading negatively impacts performance  
4. Traders act cautiously even during Greed  

---

## 🚀 Strategy Recommendations

### ✅ Strategy 1
During **Greed periods**, avoid overtrading and maintain disciplined position sizing to prevent losses due to overconfidence.

### ✅ Strategy 2
During **Fear periods**, reduce trading frequency and avoid reactive decisions, as increased activity does not improve returns.

### ✅ Strategy 3
Focus on **low-frequency, high-quality trades**, as casual traders consistently outperform frequent traders.

---

## ⚠️ Limitations
- Leverage data was not available, so leverage-based analysis was excluded.

---

## ▶️ How to Run

1. Open the notebook (`.ipynb`)
2. Run all cells sequentially
3. Ensure datasets are in the same directory

---

## 📌 Conclusion
This analysis shows that **market sentiment significantly influences trader behavior**, and disciplined trading strategies outperform reactive or high-frequency approaches.
