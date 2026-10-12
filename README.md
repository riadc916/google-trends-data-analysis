# google-trends-data-analysis

An exploratory time-series data analysis and visualization project investigating how Google Trends search popularity correlates with real-world financial and macroeconomic indicators.

## 📌 Project Overview
This project explores the relationship between web search behavior and market reality across three main case studies:
1. **Tesla Stock vs. Web Search:** Comparing TSLA stock closing prices against Google search interest over time.
2. **Bitcoin Price vs. Search Popularity:** Aligning daily cryptocurrency price data with monthly search interest to study hype cycles.
3. **U.S. Unemployment vs. Search Trends:** Analyzing searches for "Unemployment Benefits" against FRED unemployment rates (including the 2008 financial crisis and the 2020 spike) as a leading economic indicator.

## 🛠️ Key Data Skills & Techniques
- **Time-Series Preprocessing:** Handling date formats with `pd.to_datetime()` and resolving missing/NaN values.
- **Resampling:** Converting daily Bitcoin pricing data into monthly frequencies (`.resample('ME').last()`) to match Google Trends periodicity.
- **Dual-Axis Plotting:** Using Matplotlib's `.twinx()` to plot two different metric scales on the same chart cleanly.
- **Noise Reduction & Trend Smoothing:** Calculating rolling averages (`.rolling(window=6).mean()`) to identify macroeconomic trends and seasonality.
- **Visual Styling:** Configuring custom DPI, gridlines (`linestyle='--'`), color accents, and tick locators for publication-ready charts.

## 🧰 Tech Stack
- **Python**
- **Pandas**
- **Matplotlib**
- **Google Colab / Jupyter Notebook**
