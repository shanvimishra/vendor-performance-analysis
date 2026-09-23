# Vendor Performance Analysis

An end-to-end data analytics project analyzing vendor sales, purchasing,
profitability, inventory turnover, pricing, and procurement efficiency.

## Project Overview

This project uses transactional vendor data to identify patterns in:

- Vendor sales and purchasing performance
- Gross profit and profit margins
- Inventory turnover
- Vendor concentration and dependency
- Bulk-purchasing price efficiency
- Unsold inventory and capital tied up in stock
- Relationships between sales, purchases, profitability, and inventory

The workflow combines data ingestion, SQL aggregation, Python-based analysis,
statistical testing, and a Power BI dashboard.

## Tech Stack

- **Python**
- **Pandas / NumPy**
- **SQL / SQLite**
- **Matplotlib / Seaborn**
- **SciPy**
- **Jupyter Notebook**
- **Power BI**
- **Git / GitHub**

## Project Structure

```text
vendor-performance-analysis/
│
├── data/
│   └── vendor_sales_summary.csv
│
├── notebooks/
│   ├── exploratory-data-analysis.ipynb
│   └── vendor-performance-analysis.ipynb
│
├── scripts/
│   ├── ingestion_db.py
│   └── get_vendor_summary.py
│
├── dashboard/
│   └── vendor_performance.pbix
│
├── report/
│   └── Vendor_Performance_Report.pdf
│
├── requirements.txt
├── .gitignore
└── README.md
```

## Workflow

```text
Raw Transaction Data
        ↓
SQLite Database
        ↓
SQL Aggregation
        ↓
Data Cleaning & Feature Engineering
        ↓
Vendor Performance Dataset
        ↓
Exploratory Data Analysis
        ↓
Statistical Analysis
        ↓
Power BI Dashboard
        ↓
Business Insights
```

## Analysis Areas

### Vendor Performance
Analysis of vendor-level sales, purchases, gross profit, and margins to
understand differences in commercial performance.

### Inventory Efficiency
Measures such as inventory turnover and unsold inventory are used to
identify potential inventory inefficiencies and capital tied up in stock.

### Purchasing & Pricing
The project examines purchasing quantities and unit costs to understand
whether higher-volume purchasing is associated with lower procurement costs.

### Vendor Concentration
Vendor contribution is analyzed to identify concentration in purchasing
and potential dependency on a smaller group of suppliers.

### Statistical Analysis
The notebooks include correlation analysis, confidence intervals, and
hypothesis testing to evaluate relationships and differences in the data.

## Example Business Questions

- Which vendors generate the highest sales and gross profit?
- Which vendors contribute the largest share of purchases?
- How much capital is tied up in unsold inventory?
- Does purchasing in larger quantities reduce unit costs?
- Which vendors show weaker inventory turnover?
- What relationships exist between sales, purchases, and profitability?

## Running the Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/vendor-performance-analysis.git
cd vendor-performance-analysis
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

Activate it on Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the data pipeline

The ingestion script can be used to load source data into the local SQLite
database, after which the vendor summary script performs the SQL-based
aggregation.

```bash
python scripts/ingestion_db.py
python scripts/get_vendor_summary.py
```

The generated local database is intentionally excluded from Git through
`.gitignore`.

### 5. Explore the notebooks

Open the notebooks under `notebooks/` using Jupyter:

```bash
jupyter notebook
```

### 6. Power BI

Open:

```text
dashboard/vendor_performance.pbix
```

in Power BI Desktop to explore the dashboard.

## Key Findings

The accompanying analysis/report investigates findings including vendor
concentration, unsold inventory, purchasing efficiency, profitability, and
relationships between operational metrics.

For exact figures and methodology, see the notebooks and the
`Vendor_Performance_Report.pdf` included in the repository.

## Portfolio Note

This repository is organized as a portfolio-ready version of the supplied
project materials. If the original analysis was based on a course, tutorial,
template, or third-party project, the repository owner should retain the
appropriate attribution and clearly document any original modifications.

## License

No open-source license is declared for the supplied project materials.
Add a license only if you have the right to redistribute the included
code, data, report, and dashboard.
