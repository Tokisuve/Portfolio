🚀 Space Missions Data Analysis & Visualization
📌 Project Overview
This project explores a comprehensive historical dataset of space missions ranging from the dawn of the space age in 1957 up to 2022. Using Python, Pandas, and Plotly, the analysis uncovers key historical trends, including launch success rates by organization, global spending distributions, and rocket reliability metrics.   
+ 1
🛠️ Tech Stack & Libraries

Language: Python
Data Manipulation & Cleaning: Pandas, NumPy
Data Visualisation: Plotly Express, Matplotlib

🧹 Data Processing & Feature Engineering
Data Type Conversions: Standardized and parsed raw string dates and launch times into proper datetime and numeric formats.
Missing Value Management: Handled missing pricing records and filled data gaps to ensure clean aggregations.

Feature Extraction:
Extracted structural geolocation components (Launchpad, State/Region, and Country) from messy text strings using custom string splitting and mapping logic.
Created a custom Decade feature to track historical trends across different eras of space exploration.

📊 Key Insights & Visualisations
Top Successful Launches (Historical):
Analyzed cumulative historical launches and success rates across major space programs and private entities (such as RVSN USSR, CASC, and Arianespace).   
Visualised via interactive Plotly pie charts to compare operational volume and reliability.

Global Spending Analysis (Country Spenders):
Aggregated estimated mission costs by country of origin to highlight historical financial contributions and investments in space infrastructure.
Visualized via bar charts showcasing top-tier global contributors (led by the USA and Russia).   

Rocket Reliability & Failure Rates:
Filtered out experimental anomalies by applying launch thresholds to evaluate failure rates across different rocket series (identifying models with higher historical risk profiles).
