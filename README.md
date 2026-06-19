# 🪙 Cryptocurrency Price Tracker

A robust, real-time cryptocurrency data pipeline built using **Python** and **pandas**. This automation tool connects directly to live data streams to extract key market metrics for the top 10 cryptocurrencies, export them into structured formats, and maintain continuous historical logs for financial trend analysis.

---

## 📋 Project Description

In financial analytics and asset management, tracking historical data and asset volatility is crucial. The **Cryptocurrency Price Tracker** is engineered to automate this data collection process seamlessly. 

On every execution, the script fetches live market data—including **Asset Name, Ticker Symbol, Current Price (USD), 24-Hour Performance Fluctuations, and Market Capitalization**—for the top digital assets. The extracted data is immediately processed into clean tabular structures and securely appended to a localized CSV database with real-time timestamps. 

By prioritizing direct, light network stream configurations, the project ensures maximum execution stability, minimal resource overhead, and avoids common browser automation crashes (such as ChromeDriver version mismatches).

---

## 🌟 Key Features

1. **Real-Time Data Pipeline:** Auto-fetches live cryptocurrency prices and market metrics instantaneously upon execution.
2. **Top 10 Coins Extraction:** Captures comprehensive details (Name, Symbol, Price, 24h Change, Market Cap) for the top 10 digital assets by market cap.
3. **Structured CSV Export:** Cleans and formats raw numerical inputs dynamically into a well-structured `.csv` file.
4. **Continuous Historical Logging:** Implements smart logging functionality (`mode='a'`) to append new timestamped rows over time without overwriting existing entries.
5. **Dynamic Data Filtering:** Includes localized constraint filtering rules to easily sort or filter assets based on custom price thresholds.

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python
* **Data Manipulation:** pandas (for data cleaning, structuring, and CSV writing operations)
* **Networking & Parsing:** urllib, json (for secure, high-availability live data streaming)
* **Storage:** CSV Format (Optimized for database integrity and compatibility)

---

## 📂 Project Directory Structure

```text
CRYPTO_TRACKER/
│
├── crypto_tracker.py       # Core Python automation script
└── crypto_history.csv      # Generated continuous historical dataset
