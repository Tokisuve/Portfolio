US Housing & Condo Market Data Analysis & Interactive Visualisation

📌 Project Overview
This repository contains an end-to-end data analysis and interactive visualization pipeline tracking the United States condo and housing market trends over time. Using historical monthly real estate data (`condo_month.csv`), 
the project processes raw wide-format time-series datasets into structured long-format frames, engineers core financial metrics (such as appreciation rates and market drawdowns), and builds advanced interactive dashboards using **Plotly**.

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation & Cleaning:** Pandas, NumPy
* **Data Visualization:** Plotly (Express, Graph Objects, Subplots), Matplotlib

 🧹 Data Engineering & Transformation Pipeline
1. **Melting & Reshaping:** Converted wide-format monthly time series data into a normalized long format using `pd.melt()` with distinct identifiers (`RegionID`, `SizeRank`, `RegionName`, `RegionType`, `StateName`).
2. **Data Cleaning & Standardisation:** 
   * Parsed raw date strings into standard datetime objects.
   * Handled missing value entries and normalized national-level state indicators (`USA`).
   * Filtered out null pricing rows and sorted chronologically by region.
3. **Advanced Feature Engineering:**
   * **Growth Metrics:** Computed Month-over-Month (MoM) and Year-over-Year (YoY) percentage appreciation rates.
   * **Peak-to-Trough Analysis:** Calculated running all-time highs (`Running_Peak`), percentage drawdowns (`Drawdown_Pct`), and binary peak status flags (`Is_At_Peak`).
   * **Geographic Mapping:** Mapped state abbreviations to official US Census Regions (*Northeast, Midwest, South, West*) to analyse regional macro trends.


📊 Key Interactive Visualisations Built
* **Peak-to-Trough Trajectories:** Dual-panel synchronised subplots tracking home value timelines alongside historical drawdown percentages.
* **Recovery Velocity:** Statistical box plots illustrating monthly rebound growth rates during post-peak market recoveries.
* **Dynamic Dropdown Dashboards:** Interactive Plotly graph objects featuring custom dropdown menus allowing users to toggle through individual Metropolitan Statistical Areas (MSAs) and states seamlessly.
* **Regional Aggregations:** Comparative trendlines analysing macroeconomic housing performance across major US Census regions.


🚀 Getting Started & Usage
