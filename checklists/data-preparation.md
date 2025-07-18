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

## Need Help With Data Readiness?

Explore how Azilen helps organizations streamline their data pipelines and enable MLOps success. 
Check out our → [MLOps Services](https://www.azilen.com/mlops-services/)

---

## Folder & File Structure (Recommended)

| File | Description |
|------|-------------|
| [`data-prep.md`](data-preparation.md) ✅ You are here | Data pipeline and feature store readiness |
| [`model-training-and-versioning.md`](model-training-and-versioning.md) | Training reproducibility, versioning |
| [`model-deployment.md`](model-deployment.md) | CI/CD, infra-as-code, containerization |
| [`model-monitoring-and-feedback-loops.md`](model-monitoring-and-feedback-loops.md) | Drift detection, performance monitoring |
