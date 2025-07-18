# MLOps Checklist: Model Deployment

This checklist helps you deploy models in a way that’s automated, testable, and production-ready — using modern CI/CD and infrastructure practices.

---

## CI/CD for Model Deployment

- [ ] Automate model build, test, and deployment pipelines (using GitHub Actions, Jenkins, GitLab CI, etc.)
- [ ] Containerize models using Docker (with slim images)
- [ ] Use versioned API endpoints for serving models
- [ ] Automate rollback on failure or low performance
- [ ] Trigger deployments on model registry updates or version tags

---

## Infrastructure Setup

- [ ] Choose deployment mode: batch, real-time (REST/gRPC), or streaming
- [ ] Use scalable serving platforms (KServe, Seldon, TorchServe, SageMaker, Vertex AI)
- [ ] Enable auto-scaling and resource limits
- [ ] Implement health checks and readiness probes
- [ ] Secure model endpoints with tokens, OAuth, or IP filtering

---

## Pre-Deployment Testing

- [ ] Unit test model wrappers and inference logic
- [ ] Validate deployment containers with smoke tests
- [ ] Test inputs/outputs against expected shape, type, range
- [ ] Validate latency and throughput under load (using Locust or JMeter)

---

## Post-Deployment Hooks

- [ ] Log prediction requests and responses
- [ ] Set up alerting for failed or high-latency responses
- [ ] Store prediction metadata for traceability
- [ ] Route traffic between versions using canary or blue-green deployment

---

## Observability

- [ ] Use monitoring tools (Prometheus, Grafana, OpenTelemetry)
- [ ] Monitor model latency, memory, and CPU
- [ ] Set thresholds for anomaly detection in model behavior

---

## From Dev to Prod With Confidence

Want to streamline model deployment for scale, speed, and compliance?

Explore Azilen's [MLOps Services](https://www.azilen.com/mlops-services/)

---

## 📁 Folder & File Structure (Recommended)

checklists/
├── data-prep.md
├── model-training.md
├── model-deployment.md ✅ You are here
├── monitoring.md
