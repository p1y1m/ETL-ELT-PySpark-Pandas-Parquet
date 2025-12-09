# Author: Pedro Yanez Melendez

# End-to-End ETL / ELT Data Pipeline in Google Colab (pandas + PySpark + Parquet)

This project showcases a modern **data engineering** workflow implemented 100% in **Google Colab**, combining **ETL** and **ELT** patterns with **pandas**, **PySpark**, and **Parquet** in a cloud-ready, analytics-oriented pipeline.

## Project Overview

- **Extract (E)**  
  - Use **pandas** to download a public CSV dataset from the web.  
  - Persist the raw data locally inside Colab for reproducibility.

- **Transform (T) with pandas – ETL style**  
  - Clean missing values, filter invalid records, and engineer new features (e.g. `tip_pct`, `high_tip_flag`).  
  - Normalize categorical fields and enforce basic data-quality rules.  
  - Save the **cleaned dataset** as a CSV to a `processed/` folder.

- **Load (L) and Transform (T) with PySpark – ELT style**  
  - Use **PySpark** to load the cleaned data into a **Spark DataFrame**.  
  - Run distributed transformations and aggregations (group by day, time, average tip %, high-tip rate).  
  - Materialize an **analytics table** optimized for reporting and dashboards.

- **Persist (Parquet + CSV)**  
  - Save the analytics table in **Parquet** format (columnar, big-data friendly, ready for tools like **AWS Athena/Lakehouse/Spark**).  
  - Export a CSV version for quick inspection, BI tools, or sharing.

## Tech Stack and Keywords

- **pandas**: fast in-memory data wrangling and feature engineering.
- **PySpark**: scalable **distributed computing** for heavier transformations and aggregations.
- **Parquet**: modern **columnar storage** format used in **data lakes** and **lakehouse** architectures.
- **Google Colab**: fully managed notebook environment (no local installation required).
- Patterns: **ETL**, **ELT**, data-quality checks, analytics-ready data model.

This project demonstrates practical skills in **data pipelines**, **big data analytics**, and **cloud-ready formats**, using tools and concepts that are highly relevant in today’s data engineering ecosystem.
