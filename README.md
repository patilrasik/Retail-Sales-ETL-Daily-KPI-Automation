Retail Sales ETL & Daily KPI Automation 
This project automates the complete data pipeline for monitoring daily retail sales performance. Using Python, pandas, and MySQL, the pipeline cleans raw transaction data, standardizes fields, computes revenue & profit, and generates daily KPIs such as total revenue, total orders, previous day revenue, and day-over-day percentage change.
A sales alert engine is built into the pipeline to automatically detect significant drops or spikes in revenue based on a configurable threshold (e.g., 15%). Each run exports cleaned datasets and KPI summaries as CSV files and stores KPI results in MySQL for long-term reporting.
A Power BI dashboard is created on top of the processed output to visualize revenue trends, daily changes, alerts, and operational insights, enabling faster decision-making and real-time monitoring.

🔧 Tech Stack
Python (pandas, datetime, mysql-connector)
MySQL (KPI storage and reporting)
CSV/Excel (raw data ingestion & output files)
Power BI (dashboard & visualizations)
JSON (configuration settings)

🚀 Key Features
Automated ETL pipeline for retail sales data
Cleans data, parses dates, normalizes columns
Computes daily KPIs: revenue, orders, profit, % change
Detects sales drops/spikes with alert logic
Exports processed data as CSV files
Stores KPIs in MySQL for reporting
Power BI dashboard for trend & alert visualization

📁 Project Structure
project/
│
├── retail_etl.py           # main ETL pipeline script
├── config.json             # file paths + MySQL settings + thresholds
├── data/
│   ├── raw/                # input CSV/Excel files
│   └── processed/          # cleaned output files + KPI CSVs
└── README.md               # project documentation

📊 Dashboard Insights
The Power BI dashboard includes:
Daily revenue trend
Revenue % change
Alerts for drop/spike
Total orders trend
Profit insights

📝 How to Run
Update config.json with correct file paths and MySQL credentials
Run the ETL script:
python retail_etl.py
