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

