# Capstone
📊 Credit Card & Loan Application Data Engineering Capstone
Overview
This capstone project showcases a complete end-to-end data engineering pipeline, combining ETL development, API integration, data warehousing, front-end interface programming, and data analysis/visualization using industry-standard tools:

Python (Pandas, Requests, Matplotlib)

Apache Spark (Core & SQL)

MySQL

PySpark

CLI-based UI

The project demonstrates how raw credit card and loan application data can be transformed, stored, accessed, and visualized for business decision-making.

🛠️ Technologies Used
Area	Tools/Tech
Language	Python 3, SQL
ETL Framework	PySpark, Pandas
Database	MySQL
API Integration	Python Requests
Visualization	Matplotlib, Seaborn
Interface	Console-based UI (Python CLI)
Version Control	Git, GitHub\

creditcard_capstone/
│
├── data/                        # Contains raw JSON data and screenshots of graphs
│
├── scripts/
│   ├── etl_creditcard.py       # PySpark pipeline for credit card data
│   ├── etl_loan_api.py         # API integration and ETL for loan data
│   ├── cli.py                  # Console front-end interface
│   ├── visualizations.py       # All graph creation logic
│   └── database_setup.sql      # SQL scripts to create required tables
│
├── README.md                   # Project documentation (this file)
├── requirements.txt            # Python dependencies
└── .gitignore                  # Ignores sensitive info, __pycache__, etc.

🔄 Workflow Summary
1. ETL Pipeline for Credit Card Data
Extracted data from 3 JSON files: CDW_SAPP_CUSTOMER, CDW_SAPP_BRANCH, and CDW_SAPP_CREDITCARD.

Transformed data using PySpark according to a business mapping document.

Loaded the clean data into a MySQL database: creditcard_capstone.

2. CLI Application
Developed a console-based UI to:

Search transactions by ZIP code, month, and year.

View and edit customer details.

Generate monthly statements.

View customer transactions between two dates.

Fully functional .py script demonstrating data access from MySQL.

3. Loan Application API Integration
Accessed loan application data from:

https://raw.githubusercontent.com/platformps/LoanDataset/main/loan_data.json

Verified HTTP status codes.

Loaded processed loan data into MySQL table CDW_SAPP_LOAN_APPLICATION.

4. Visualizations & Insights
From Credit Card Dataset:
📌 Most common transaction type (bar chart)

📌 Top 10 states by number of customers (horizontal bar chart)

📌 Top 10 customers by total transaction value (bar chart)

From Loan Dataset:
📌 Approval rate for self-employed applicants (pie chart)

📌 Custom analysis: Discovered loan approval patterns based on income level and area (bar and scatter plots)

All visualizations include clean labels, legends, titles, and are saved as high-resolution .png images.

📷 Screenshots
Screenshots of graphs and key program outputs are located in the data/screenshots/ folder and were included per submission guidelines.

🚀 How to Run
Prerequisites
Python 3.8+

MySQL Server

Apache Spark

All Python libraries in requirements.txt

Steps
Clone the repository

Create the database using database_setup.sql

Run etl_creditcard.py and etl_loan_api.py to populate the DB

Launch the console app:

bash
Copy
Edit
python cli.py
Run visualizations:

bash
Copy
Edit
python visualizations.py
📈 Key Skills Demonstrated
Building scalable ETL pipelines using PySpark and SQL

Handling structured/unstructured data from various sources (API, JSON)

Designing CLI interfaces for data retrieval and interaction

Creating insights-driven visualizations for stakeholders

Managing codebase using GitHub branches and .gitignore

✅ Deliverables
✔ Cleaned and loaded relational database

✔ Functional front-end program

✔ Five+ visualizations with actionable insights

✔ Loan API integration and ingestion

✔ GitHub repository with documented code and README

✔ Screenshots of all graphs for reference

🤝 Acknowledgments
This capstone project was completed as part of CAP 350 - Data Engineering at Per Scholas. Special thanks to the instructional team and support staff.