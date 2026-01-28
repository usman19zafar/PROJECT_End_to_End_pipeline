# Project 2 – End-to-End CSV Data Pipeline (Raw → Bronze → Silver → Gold)

## Overview
This project demonstrates an end-to-end data engineering pipeline that ingests raw CSV data, applies structured transformations, and produces curated datasets using a **Bronze, Silver, and Gold** layered architecture.

The pipeline is designed and executed using **Azure Data Factory**, with transformations implemented via notebooks. A successful pipeline execution is included as evidence.

---

## Architecture
**Flow:**
Raw CSV → Bronze → Silver → Gold

Each layer has a clear responsibility:
- **Raw**: Original source CSV files
- **Bronze**: Ingested data with basic structure and schema handling
- **Silver**: Cleaned and transformed data
- **Gold**: Final curated dataset ready for consumption and validation

---
```code
## Repository Structure
Project_End_to_End_pipeline/
│
├── README.md
│
├── data/
│   ├── raw/                # Original source CSV files
│   ├── bronze/             # Ingested data (raw → structured)
│   ├── silver/             # Cleaned and transformed data
│   └── gold/               # Final curated dataset
│
├── notebooks/
│   ├── 01_raw_to_bronze.ipynb
│   ├── 02_bronze_to_silver.ipynb
│   └── 03_silver_to_gold.ipynb
│
├── screenshots/
│   └── pipeline_success_run.png   # Successful pipeline execution proof
│
└── p_ingest_project2.json          # Exported pipeline definition (ADF)
```
---

## Tools & Technologies
- Azure Data Factory
- Azure Blob Storage
- Python
- Jupyter Notebooks
- JSON-based pipeline definitions
- Power BI

---

## How to Use
1. Review the pipeline logic in the notebooks folder.
2. Inspect the exported pipeline JSON for orchestration details.
3. Refer to the screenshot for confirmation of a successful pipeline run.
4. Sample data is provided to illustrate each processing stage.

---

## Key Learning Outcomes
- Designing layered data architectures (Bronze/Silver/Gold)
- Building reproducible ingestion and transformation pipelines
- Separating orchestration from transformation logic
- Producing clean, validated datasets ready for analytics

---

## Status
✅ Completed  
This project is part of a larger sequence of end-to-end data engineering projects.
