# MLOps Checklist: Data Preparation

This checklist helps you prepare your data pipelines for robust and repeatable machine learning workflows in production environments.

---

## Data Ingestion

- [ ] Identify and list all data sources (internal, external, streaming)
- [ ] Establish secure access and authentication (API keys, IAM roles)
- [ ] Set up automated data extraction (ETL/ELT tools, Airflow, etc.)
- [ ] Validate schema and data types during ingestion
- [ ] Track data ingestion success/failure logs

---

## Data Cleaning & Validation

- [ ] Handle missing values using defined imputation strategies
- [ ] Detect and remove duplicates or corrupt records
- [ ] Normalize formats (e.g., date/time, strings, categories)
- [ ] Set up basic data validation rules and error thresholds

---

## Feature Engineering

- [ ] Define feature extraction logic (static and real-time)
- [ ] Version control feature definitions (with Git or Feature Store)
- [ ] Test features for leakage and correlation
- [ ] Store features in a central, queryable location (Feature Store)

---

## Metadata & Lineage

- [ ] Tag data with source, version, and timestamp
- [ ] Track transformations (who changed what and when)
- [ ] Store metadata for future audits and explainability

---

## Folder & File Structure (Recommended)

checklists/
├── data-prep.md ✅ You are here
├── model-training.md
├── model-deployment.md
├── monitoring.md

---

## Need Help With Data Readiness?

Explore how Azilen helps organizations streamline their data pipelines and enable MLOps success.  
→ [MLOps Services](https://www.azilen.com/mlops-services/)
