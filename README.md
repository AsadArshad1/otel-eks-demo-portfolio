# OpenTelemetry Demo – Local & EKS Deployment (Portfolio)

This repo documents deployment of the official OpenTelemetry microservices demo:
- Local: Docker Compose + Observability (Prometheus, Grafana, Jaeger)
- Cloud: AWS EKS with Terraform + Helm/Kubernetes manifests
- Tracing/metrics/logs via OpenTelemetry

## Repo layout
- `upstream/opentelemetry-demo` – official demo (git submodule)
- `infra/terraform` – IaC for EKS
- `k8s/` – manifests / Helm charts
- `.github/workflows/` – CI/CD
- `docs/` – diagrams, screenshots, runbook

## Milestones
- [ ] Local: docker-compose + screenshots
- [ ] EKS: terraform + manifests + public demo
- [ ] CI/CD: GitHub Actions for build & deploy
- [ ] Observability: Grafana/Jaeger dashboards published

## Local Deployment (Docker Compose)

The demo runs locally with Docker Compose:

bash
"""cd upstream/opentelemetry-demo
   docker compose up --build"""

Frontend: http://localhost:8080

Grafana: http://localhost:3000

Jaeger: http://localhost:16686

### SCREENSHOTS
- `docs/` – diagrams, screenshots, runbook

## Containerization of Microservices
- Built Docker images for `ad`, `recommendation`, and `product-catalog`
- Tagged and pushed them to Docker Hub:
  - ad → dockerhub.io/asadarshad19/ad:v1
  - recommendation → dockerhub.io/asadarshad19/recommendation:v1
  - product-catalog → dockerhub.io/asadarshad19/product-catalog:v1



