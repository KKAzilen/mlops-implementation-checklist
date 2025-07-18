# MLOps Checklist: Model Training & Versioning

Use this checklist to ensure your training workflows are reproducible, auditable, and ready for continuous improvement in production.

---

## Environment Setup

- [ ] Use virtual environments (`venv`, `conda`, or Docker)
- [ ] Track dependencies using `requirements.txt`, `poetry.lock`, or `environment.yml`
- [ ] Define and manage compute environment (CPU, GPU, memory limits)
- [ ] Use consistent versions of Python, libraries, and CUDA/ML stack

---

## Reproducibility

- [ ] Set random seeds across libraries (`numpy`, `tensorflow`, `torch`)
- [ ] Parameterize your training script (via config files or CLI)
- [ ] Store and version configs (YAML, JSON) alongside code
- [ ] Ensure consistent data splits (train/val/test) across runs

---

## Model Training Process

- [ ] Use experiment tracking tools (MLflow, Weights & Biases, Neptune)
- [ ] Log metrics (accuracy, loss, AUC) per run
- [ ] Log hyperparameters and model artifacts
- [ ] Store model training logs centrally (CloudWatch, ELK, etc.)

---

## Versioning & Storage

- [ ] Version models with meaningful tags (`model_v1.2`, `v2.0-beta`)
- [ ] Store trained models in a central registry or blob storage
- [ ] Include metadata: dataset version, date, accuracy, author
- [ ] Automate post-training evaluation and comparison

---

## Testing Before Deployment

- [ ] Run inference tests with sample inputs
- [ ] Validate output consistency and edge case behavior
- [ ] Compare model to baseline or previous versions
- [ ] Include basic unit tests in training pipeline

---

## Production Tip

Model training should be treated as **code + data + config** — all version-controlled and traceable.

For full lifecycle support, check out → [MLOps Services](https://www.azilen.com/mlops-services/)

---

## 📁 Folder & File Structure (Recommended)

| File | Description |
|------|-------------|
| [`data-preparation.md`](data-preparation.md) | Data pipeline and feature store readiness |
| [`model-training-and-versioning.md`](model-training-and-versioning.md) ✅ You are here | Training reproducibility, versioning |
| [`model-deployment.md`](model-deployment.md) | CI/CD, infra-as-code, containerization |
| [`model-monitoring-and-feedback-loops.md`](model-monitoring-and-feedback-loops.md) | Drift detection, performance monitoring |
