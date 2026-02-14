# Devops-practice-lab

This repository is a hands-on, chapter‑based guide to building and deploying cloud-native applications
using Terraform, Kubernetes, Flux, and related tools. Each numbered folder represents a self‑contained
"chapter" focused on a particular area of the development‑to‑operations lifecycle.

---

## Chapters Overview

1. **Terraform** (`1-terraform/`)
   - Learn the fundamentals of Terraform by solving a networking problem with AWS Lambda.
   - Focuses on private networking, VPCs and internet access from isolated functions.

2. **Kubernetes Cluster** (`2-kubernetes-cluster/`)
   - Create and manage an Amazon EKS (or local Kind/Minikube) cluster with Terraform.
   - Install Flux v2 in the cluster to bootstrap the continuous-deployment flow.

3. **Continuous Deployment** (`3-continuous-deployment/`)
   - Use FluxCD and Helm to continuously deliver workloads into the cluster.
   - Build Docker images, publish them to a registry, and deploy with Helm charts.
   - Exercise includes NATS messaging, producer/consumer services, and Benthos.

4. **Telemetry** (`4-telemetry/`)
   - Add observability via metrics, logs and tracing (OpenTelemetry, Prometheus, Grafana, Jaeger).
   - Instrument services and visualize metrics/traces in dashboards.

5. **Secrets** (`5-secrets/`)
   - Manage sensitive data for applications using Vault (or sealed‑secrets) instead of plaintext.
   - Integrate secrets into Kubernetes workloads securely.

6. **Continuous Integration** (`6-continuous-integration/`)
   - Configure GitHub Actions pipelines to validate infrastructure on each push.
   - Run Terraform/Helm tests and publish charts based on tags.

7. **Service Mesh** (`7-service-mesh/`)
   - (TBD) Explore service mesh concepts, policies and tooling (e.g. Cilium, Istio) in Kubernetes.

---

## Getting Started

1. Clone this repository and browse the chapter directories.
2. Follow the README in each chapter for exercises, suggested roadmaps, and references.
3. You can work sequentially through the chapters or focus on particular areas of interest.
4. Many chapters rely on an AWS account; configure your CLI credentials before running Terraform.
5. Use `kubectl` and `k9s` to inspect clusters; `terraform` to provision resources; and `flux` to manage deployments.

> 💡 The structure is intentionally minimal to encourage experimentation. Feel free to adapt,
> extend or repurpose the examples for your own learning path.

---

## Resources

- `cr.yaml` contains repository metadata used by automated tooling.
- Each chapter has its own `README.md` with detailed instructions and references.

---

Happy learning! 🚀
