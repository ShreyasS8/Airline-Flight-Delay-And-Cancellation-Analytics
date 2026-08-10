# ✈️ Airline Flight Delay & Cancellation Analytics

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow.svg)
![Data Analysis](https://img.shields.io/badge/Data-Analysis-green.svg)

## 📌 Project Overview
This project involves a comprehensive end-to-end data pipeline and analytics dashboard for a massive dataset of 3 million commercial flight records. The goal is to investigate flight delays and cancellations, identify patterns in airline operational performance, and extract actionable business insights using Python for data processing and EDA, culminating in an interactive Power BI dashboard for executive reporting.

## 🎯 Business Problem & Objectives
Flight delays and cancellations cause significant revenue loss for airlines and result in poor customer satisfaction. Understanding the root causes, seasonal trends, and airline-specific performance metrics is critical for operational optimization.

**Key Objectives:**
- **Data Engineering:** Build a robust, high-performance data cleaning pipeline to handle a large-scale dataset (3M rows).
- **Quality Assurance:** Address structural nulls (e.g., handling missing times for cancelled flights) and preserve extreme delay signals for accurate operational analysis.
- **Exploratory Data Analysis (EDA):** Perform univariate, bivariate, and multivariate analysis to identify delay patterns across airlines, airports, and timeframes.
- **Data Visualization:** Develop a professional-grade Power BI dashboard to present key operational performance indicators (KPIs) to stakeholders.

## 🛠️ Tech Stack & Tools
- **Data Cleaning & Processing:** Python, Pandas, NumPy
- **Exploratory Data Analysis:** Jupyter Notebook, Matplotlib, Seaborn
- **Data Visualization & Dashboarding:** Power BI
- **Documentation & Reporting:** Microsoft Word, PowerPoint

## 📂 Repository Structure

```text
📦 Airline-Flight-Analytics
 ┣ 📂 EDA/
 ┃ ┗ 📜 flights_eda.ipynb                 # Comprehensive Exploratory Data Analysis
 ┣ 📂 Power_BI/
 ┃ ┣ 📜 Flight Delay-Dashboard.pbix       # Interactive Power BI Report (Git LFS)
 ┃ ┗ 📜 Flight Delay-Dashboard.pdf        # Executive Dashboard Summary (PDF)
 ┣ 📜 data_clearning_and_processing.ipynb # Core data cleaning & feature engineering pipeline
 ┗ 📜 README.md                           # Project Documentation
```
*(Note: Raw datasets are excluded due to file size limits. Power BI dashboard source files (`.pbix` managed via Git LFS) and PDF exports are included in the `Power_BI/` directory).*

## 🔍 Key Project Phases

### 1. Data Cleaning & Processing (`data_clearning_and_processing.ipynb`)
- **Handling Structural Nulls:** Implemented domain-accurate handling for cancelled and diverted flights to ensure logical consistency rather than blind imputation.
- **Outlier Treatment:** Preserved genuine extreme delay signals (which are critical operational anomalies) while treating erroneous data entry points.
- **Feature Engineering:** Derived new time-based and delay-category features to enrich the dataset for deeper analysis.
- **Optimization:** Converted data types to reduce memory footprint and optimized storage using Parquet formats.

### 2. Exploratory Data Analysis (`flights_eda.ipynb`)
- Analyzed distribution of delays across different carriers and origin-destination pairs.
- Investigated the correlation between time of day, day of the week, and likelihood of delays.
- Generated over 15 distinct, insight-driven visualizations interpreting the business impact of the findings.

### 3. Executive Dashboarding (`Power_BI/`)
- **Interactive Power BI Report (`Flight Delay-Dashboard.pbix`):** Dynamic reporting tool supporting interactive filtering across carriers, time periods, and delay types.
- **Executive Summary PDF (`Flight Delay-Dashboard.pdf`):** A pre-rendered visual presentation of the complete dashboard for easy previewing.
- **Key Dashboard Features & Visuals:**
  - **KPI Scorecards:** Total Flights (3M records analyzed), Average Delay Minutes, and Cancellation Rate.
  - **Carrier Comparison:** Visual rankings highlighting most reliable vs delay-prone airlines.
  - **Temporal Heatmaps:** Flight congestion and delay probability across hours of the day and days of the week.
  - **Root Cause Analysis:** Operational breakdown across Carrier, Weather, National Air System (NAS), Security, and Late Aircraft delays.

## 📈 Key Insights
*(You can customize this section once you pull the final insights from your EDA/Presentation)*
- **Carrier Performance:** Identified specific airlines that consistently struggle with turnaround times and weather-related delays.
- **Temporal Trends:** Pinpointed specific days of the week and times of day where the probability of severe delays spikes.
- **Operational Bottlenecks:** Mapped out high-traffic airports that contribute disproportionately to the network's overall delay minutes.

## 🚀 How to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Airline-Flight-Analytics.git
   ```
2. Install the required Python packages:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
3. Open the Jupyter Notebooks to view the code:
   ```bash
   jupyter notebook
   ```

## 👨‍💻 Author
**Shreyas**
- Analytical problem solver with a passion for transforming raw data into strategic business insights.
