# 🎬 Netflix Data Analytics | End-to-End Data Engineering with dbt & Snowflake
## 📌 Introduction

This project showcases a modern data engineering workflow using dbt (data build tool) and Snowflake to analyze the MovieLens dataset.
The pipeline transforms raw movie, rating, and tagging data into structured fact and dimension models, enabling robust analytics and business insights.

## 🏗️ Architecture

<img src="Data Pipeline Architecture.jpg">

## Key Layers

1. **Raw Layer** – Ingests raw CSV files into Amazon S3, then loads into Snowflake.  
2. **Staging Layer** – Data cleaning, standardization, and schema alignment.  
3. **Serving Layer** – Final star schema models for analytics & BI tools (Power BI, Tableau, Looker Studio).
   
## 🛠 Tech Stack

- **Cloud Data Warehouse**: Snowflake  
- **Transformation Framework**: dbt  
- **Version Control**: Git & GitHub  
- **Visualization**: Power BI, Tableau, Looker Studio  

## 📂 Dataset

Source: [MovieLens Dataset](https://grouplens.org/datasets/movielens/)

**Raw Tables**:  
- `raw_movies` – Movies metadata  
- `raw_ratings` – User ratings  
- `raw_tags` – User tags  
- `raw_genome_scores` – Tag relevance scores  

## ✨ Features

- **Raw → Staging Transformation**: Data cleaning, schema standardization.  
- **Star Schema Modeling**: Fact & Dimension tables for analytics.  
- **Data Quality Assurance**:  
  - Built-in dbt tests: `not_null`, `unique`  
  - Custom macro: `no_nulls_in_columns()`  
- **Relevance Filtering**: Keep scores with relevance > 0.  
- **Version Control & Collaboration**: Fully managed via Git & GitHub.  

## 🚀 Future Enhancements

- Automate dbt runs with **GitHub Actions (CI/CD)**.  
- Expand BI dashboards in **Power BI / Tableau / Looker Studio**.  
- Integrate **Airflow or Prefect** for orchestration.  
- Extend pipeline to **real-time streaming (Kafka → Snowflake)**.  

## 🎯 Key Learnings

- Building **scalable ELT pipelines** with dbt & Snowflake.  
- Designing **dimensional models** (Fact/Dimension).  
- Implementing **data quality tests & macros**.  
- Leveraging **GitHub for collaboration & version control**.
  
# 👤 Author

**Nguyen Dinh Hoang Tuan**  
📧 ndhtuan02@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/tuan-nguyen-02353b378) | [GitHub](https://github.com/Devhtuan)
