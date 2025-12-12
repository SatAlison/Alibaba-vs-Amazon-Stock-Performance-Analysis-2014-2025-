<h1 align="center"> Alibaba vs Amazon Stock Performance Analysis (2014–2025)</h1>

<h3 align="center">by <strong>Satelite Alison Ndayikunda</strong></h3>

---

##  Overview
This project compares the stock performance of **Alibaba (BABA)** and **Amazon (AMZN)** from **2014 to 2025**, using daily stock data.  
It explores how both companies performed in terms of **growth, volatility, correlation, and investor attractiveness**.

Data is stored in **Microsoft SQL Server (MSSQL)** and queried into Python using **SQLAlchemy**, allowing a seamless connection between the database and Python environment.  
This setup combines **SQL data management** with **Python-based analytics and visualization**, enabling a **full-stack data analysis workflow** — from data extraction to insight generation.


![Stock Dashboard](https://github.com/SatAlison/Alibaba-vs-Amazon-Stock-Performance-Analysis-2014-2025-/blob/main/Images/Screenshot%20(106).png)


---

##  Objectives

| # | Objective |
|:-:|:--|
| 1 | Analyze and visualize stock trends for Amazon and Alibaba. |
| 2 | Compare volatility and daily returns between the two companies. |
| 3 | Examine relationships between price movement and trading volume. |
| 4 | Measure correlation between the two companies’ stock returns. |
| 5 | Identify which company shows stronger long-term growth. |

---

##  Data Sources

| Source | Description |
|:--|:--|
| **Kaggle** | Daily stock prices for Alibaba and Amazon. |
| **SQL Server** | Used for storing and querying data. |
| **Python (Pandas)** | Used for cleaning, analysis, and visualization. |

**Key Variables**
- `Date` – Trading date  
- `Adj Close` – Adjusted closing price  
- `Volume` – Number of shares traded  
- `Daily_Returns` – Percentage change in price from previous day  

---

##  Data Preparation

| Step | Action |
|:--|:--|
| 1 | Imported data from Yahoo Finance into SQL Server. |
| 2 | Cleaned and standardized column names (e.g., `adj_close`, `date`). |
| 3 | Filtered period between **2014–2025** for both companies. |
| 4 | Merged both datasets and added a new column `company` to differentiate them. |
| 5 | Calculated daily returns and rolling averages for trend analysis. |

---

<summary><h2> Exploratory Data Analysis (EDA)</h2></summary>

---

### 1️⃣ Relationship Between Price Movement and Trading Volume

| Company | Correlation | Interpretation |
|:--|--:|:--|
| **Alibaba** | -0.019 | Almost no correlation — price changes have little impact on trading volume. |
| **Amazon** | -0.220 | Weak negative correlation — volume slightly decreases as price rises. |

####  Insights
- **Alibaba’s** trading volume stays stable despite price movements.  
- **Amazon** shows a mild tendency for lower trading when prices increase.  
- Overall, **price and volume move mostly independently** for both companies.
 
![Price vs Volume](https://github.com/SatAlison/Alibaba-vs-Amazon-Stock-Performance-Analysis-2014-2025-/blob/390ce6f7c9bc8bcd85e16a133f5154c48ae2ab4c/Images/volume%20vs%20price.png)

---
### 2️⃣ How Have Their Stock Prices Evolved Over Time?

From **2014 to 2025**, **Amazon’s** stock shows steady long-term growth with a brief dip around **2020–2021** — likely caused by the **COVID-19 pandemic** — followed by a strong recovery.  
**Alibaba**, on the other hand, peaked around the same period but **declined sharply afterward**, partly due to both pandemic impacts and **China’s regulatory pressures** on the tech sector.

####  Insights
- **Amazon**: Consistent growth and quick post-pandemic recovery.  
- **Alibaba**: Strong pre-2021 performance but noticeable decline afterward.  
- **Overall**: Amazon demonstrates more **resilience and stability**, while Alibaba remains **more volatile**.

![Stock Price Trends](https://github.com/SatAlison/Alibaba-vs-Amazon-Stock-Performance-Analysis-2014-2025-/blob/a00facacda570b49b5a85d8c6ecbde6d86494761/Images/stockpricetrendslineplot.png)

---

### 3️⃣ Which Company Shows Higher Volatility and Better Daily Returns?

| Company | Average Daily Return (%) | Standard Deviation (%) | Interpretation |
|:--|--:|--:|:--|
| **Amazon** | **0.12** | **2.05** | Higher average return and lower volatility — more stable performance. |
| **Alibaba** | **0.04** | **2.62** | Lower average return and higher volatility — riskier with larger price swings. |

####  Insights
- **Amazon** offers better daily returns with less price fluctuation, suggesting a **more consistent and stable stock**.  
- **Alibaba** exhibits greater volatility, meaning **higher risk but potential for larger short-term gains**.  
- Investors prioritizing stability and predictable growth would lean toward **Amazon**, while those open to higher risk may consider **Alibaba**.

![Daily Returns Comparison](https://github.com/SatAlison/Alibaba-vs-Amazon-Stock-Performance-Analysis-2014-2025-/blob/a00facacda570b49b5a85d8c6ecbde6d86494761/Images/boxplot(distribution%20of%20daily%20returns).png)

---

### 4️⃣ How Correlated Are Alibaba and Amazon Stocks?

| Comparison | Correlation Coefficient |
|:--|:--:|
| **Amazon vs Alibaba (Daily Returns)** | **0.35** |

####  Insights
- The **moderate positive correlation (0.35)** suggests that the two stocks occasionally move in the same direction but not consistently.  
- **Amazon** and **Alibaba** operate in different economic and regulatory environments — the U.S. and China — which reduces direct price linkage.  
- This weak correlation can **benefit portfolio diversification**, as holding both stocks reduces overall risk.

---
### 5️⃣ Which Company Has Shown Stronger Growth Overall Since 2014?

| Company | Total Growth (%) |
|:--|--:|
| **Amazon** | **+1,290.6%** |
| **Alibaba** | **+31.8%** |

####  Insights
- **Amazon** demonstrated exceptional growth fueled by:
  - Global expansion and strong e-commerce dominance.  
  - Diversification into **AWS cloud services** and digital media.  
  - High investor confidence and innovation-driven business model.  

- **Alibaba** initially grew rapidly but faced setbacks after **China’s 2021 regulatory crackdown**, which restricted the tech sector and reduced market valuation.  

####  Conclusion
Amazon has shown **stronger, consistent, and long-term growth**, while Alibaba’s trajectory has been **more volatile** and influenced by external market and regulatory pressures.

---

##  Key Insights

| # | Insight |
|:-:|:--|
| 1 | Amazon showed consistent upward momentum with strong recovery after market corrections. |
| 2 | Alibaba peaked in 2020 but declined due to Chinese government regulations. |
| 3 | Both companies show volatility, but Amazon offers better long-term stability. |
| 4 | Weak correlation (0.35) suggests different market dynamics influence their stock behavior. |
| 5 | Amazon’s overall growth (~1290%) far exceeds Alibaba’s (~32%) since 2014. |

---

##  Conclusion & Investment Advice

- **Amazon** offers **stronger long-term growth** and **greater resilience**, making it suitable for investors seeking stability and consistent returns.  
- **Alibaba** presents a **riskier but potentially undervalued** opportunity — it could rebound if China’s regulatory climate eases or global expansion accelerates.  
- The **2021 regulatory crackdown** in China played a major role in slowing Alibaba’s growth momentum.  

###  Investor Summary

| Investor Type | Recommended Stock | Reason |
|:--|:--|:--|
| **Long-term / Stability-seeking** | 🟩 Amazon | Strong growth, diversified income streams, global trust. |
| **Short-term / Risk-tolerant** | 🟧 Alibaba | Possible rebound if market conditions improve. |

---

##  Tools & Technologies

| Category | Tools |
|:--|:--|
| **Data Storage** | Microsoft SQL Server |
| **Data Analysis** | Python (Pandas, NumPy) |
| **Visualization** | Matplotlib, Seaborn |
| **Environment** | VS Code|

---

## 🚀 Future Work
- Extend analysis to other tech companies like **JD.com**, **eBay**, or **Meta**.  
- Build a **machine learning model** (e.g., ARIMA, LSTM) to forecast stock prices.  
- Integrate **macroeconomic indicators** (GDP growth, inflation, interest rates) to understand external factors.  

---

## 👩‍💻 Author

**Satelite Alison Ndayikunda**  
📍 *Data Analyst | Growth-Minded Learner*  
📧 [satalisonn@gmail.com]  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/satelite-alison-ndayikunda/)


