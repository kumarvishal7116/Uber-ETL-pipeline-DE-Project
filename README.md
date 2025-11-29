🚗 Uber ETL Pipeline – Data Engineering Project

This project demonstrates an end-to-end **ETL (Extract → Transform → Load)** data engineering pipeline using Python.  
It processes raw Uber trip data, cleans and transforms it, and prepares analytics-ready outputs supported by SQL-based analysis.

The project includes modular ETL scripts, notebooks for exploration, and SQL queries for downstream reporting — ideal for learning, portfolio building, and interview preparation.

---


📘Project Architecture

Raw Data (CSV)
│
▼
[Extract Stage] → ingest raw Uber dataset
│
▼
[Transform Stage] → data cleaning, feature engineering, validation
│
▼
[Load Stage] → save cleaned data (CSV/parquet/DB)
│
▼
Analytics → SQL queries, insights, dashboards


📁 **Repository Structure**

├── data/
│ └── uber_data.csv # sample raw dataset
│
├── mage-files/
│ ├── extract.py # extract Uber raw data
│ ├── transform.py # clean & transform data
│ └── load.py # load processed data
│
├── Uber Data Pipeline (Fixed Version).ipynb # detailed notebook walkthrough
├── Uber Data Pipeline (Video Version).ipynb # notebook used for demonstrations
│
├── analytics_query.sql # SQL queries for analytics
├── commands.txt # helpful commands & notes
└── README.md


---

## 🛠️ **Technologies Used**

- **Python** – core ETL scripting  
- **Pandas** – data cleaning & transformation  
- **Jupyter Notebooks** – data exploration & validation  
- **SQL** – analytics queries  
- **Mage-style modular scripts** – clean extract/transform/load structure  
- Optional: PostgreSQL / SQLite / Parquet for storage  

---

## ⚙️ **Setup & Installation**

### **1️⃣ Clone the Repository**
```bash
git clone https://github.com/kumarvishal7116/Uber-ETL-pipeline-DE-Project.git
cd Uber-ETL-pipeline-DE-Project


2️⃣ Create Virtual Environment
python -m venv venv

Windows
venv\Scripts\activate

macOS/Linux
source venv/bin/activate


3️⃣ Install Dependencies
pip install -r requirements.txt



pip install pandas jupyter


▶️ How to Run the Pipeline
Run Complete ETL Pipeline

python mage-files/extract.py
python mage-files/transform.py
python mage-files/load.py

Run Individual Stages
python mage-files/extract.py

Transform
python mage-files/transform.py

Load
python mage-files/load.py


📊 Notebooks for EDA & Validation

You can explore cleaning steps, statistics, and visualizations through:

Uber Data Pipeline (Fixed Version).ipynb

Uber Data Pipeline (Video Version).ipynb

Launch notebook:
jupyter notebook "Uber Data Pipeline (Fixed Version).ipynb"


🧠 Analytics Using SQL
The analytics_query.sql file contains SQL queries to run on the cleaned dataset.

Sample insights include:
Total trips by hour/day
Average fare, trip distance, duration
Trips by location clusters
Peak demand analysis
Run in SQLite / Postgres / BigQuery as needed.


⭐ Key Features

Fully modular Extract → Transform → Load pipeline
Clean & readable Python ETL scripts
Realistic Uber-style dataset
Jupyter notebooks for explanation & EDA
SQL queries for analytics & reporting
Beginner-friendly and ideal for portfolio showcasing

🚀 Future Improvements
Dockerize the pipeline
Add Airflow orchestration
Add logging & exception handling
Convert outputs to parquet format
Build Power BI / Tableau dashboard
Add automated data validation (Great Expectations / Pandera)


