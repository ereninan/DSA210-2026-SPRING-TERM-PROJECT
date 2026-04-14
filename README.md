# DSA210-2026-SPRING-TERM-PROJECT

# The Impact of Typhoon Signals on Hong Kong Stock Market Volatility and Returns 🌪️📉

## 📌 Overview
This repository contains the term project for **DSA 210 (Introduction to Data Science)** at Sabancı University. The project investigates whether the issuance of typhoon warning signals in Hong Kong affects the Hang Seng Index (HSI) daily returns and volatility. By categorizing trading days based on typhoon signal levels, the study analyzes market behavior and price fluctuations during extreme weather conditions.

## 👨‍💻 Author
**Hamza Eren İnan** ## 📂 Repository Structure
* `EDA_and_Hypothesis_Testing.ipynb`: The main Jupyter Notebook containing data loading, preprocessing, exploratory data analysis (EDA), and statistical hypothesis testing.
* `DSA 210 Term Project Proposal.pdf`: The initial project proposal outlining the research question, data sources, and planned methodology.
* `HSI.csv`: Historical daily Hang Seng Index prices (Open, High, Low, Close, Volume) ranging from 1986 to 2023.
* `Typhoon.csv`: Historical tropical cyclone warnings sourced from the Hong Kong Observatory.
* `requirements.txt`: List of Python dependencies required to reproduce the analysis.

## 📊 Dataset Details
The analysis merges two primary datasets:
1. **Hang Seng Index (HSI.csv):** Contains continuous daily observations of the Hong Kong stock market.
2. **Typhoon Warnings (Typhoon.csv):** Contains categorical and temporal data representing the intensity of tropical cyclones. The warning signals are grouped into:
   * **Normal:** No active warnings.
   * **Low-alert:** Signals 1 & 3.
   * **High-alert:** Signals 8 and above.

## 🔬 Methodology
1. **Data Cleaning:** Standardized date formats, removed irrelevant directional characters from typhoon signals using Regular Expressions, and merged the datasets on overlapping dates (2000–2023).
2. **Exploratory Data Analysis (EDA):** Visualized market return distributions and volatility across different typhoon alert levels.
3. **Hypothesis Testing:** Conducted statistical tests to determine if HSI returns on typhoon-affected days significantly deviate from normal trading days.

## 📈 Key Findings & Limitations
* **Findings:** The analysis indicates that average daily returns are not significantly impacted by typhoon warnings. Market participants appear to price in these short-term weather disruptions efficiently without causing major deviations in closing prices.
* **Limitations:**
  * *Temporal Mismatch:* Typhoon warnings span specific hours, whereas the index data provides only daily summaries, making intraday effects harder to capture.
  * *Confounding Variables:* The analysis does not control for broader macroeconomic events or global financial crises that occurred on the same days.
* **Future Work:** Future iterations could focus exclusively on intraday volatility or trading volume changes, which may exhibit higher sensitivity to sudden weather alerts than daily closing returns.

## 🚀 How to Run
1. Clone this repository to your local machine.
2. Install the required dependencies using pip:
   ```bash
   pip install -r requirements.txt
