# Financial API ETL Pipelines 📡📊

A collection of automated Python ETL pipelines designed to extract live financial market data via REST APIs, parse nested JSON responses, and generate clean, structured datasets for quantitative analysis.

## ⚙️ Core Architectures

### 1. Crypto Market Cap Pipeline (CoinGecko API)
* **Function:** Pings the CoinGecko REST API to retrieve real-time pricing, volume, and market cap data for the top 50 cryptocurrencies.
* **Transformation:** Flattens JSON payloads and standardizes data types into a Pandas DataFrame.
* **Output:** Generates `live_crypto_market_data.csv`.

### 2. Global Forex Exchange Pipeline (Frankfurter API)
* **Function:** Extracts live fiat exchange rates against the US Dollar (USD).
* **Transformation:** Parses deeply nested JSON dictionaries and appends parent-level metadata (timestamps, base currency) to child records.
* **Output:** Generates `live_forex_usd_rates.csv`.

## 🛠️ Technical Stack & Reproducible Workflow
* **Language:** Python 3.x
* **Data Engineering:** Pandas
* **Network Requests:** `requests` library (REST API / JSON handling)

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Financial-API-ETL-Pipelines.git](https://github.com/YOUR_USERNAME/Financial-API-ETL-Pipelines.git)
