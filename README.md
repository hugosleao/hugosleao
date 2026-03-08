<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=28&pause=1000&color=00ADD8&center=true&vCenter=true&width=700&lines=Hugo+Le%C3%A3o;Senior+DevOps+Engineer;Platform+Engineering+%7C+Cloud+Architecture;Building+Internal+Developer+Platforms" alt="Typing SVG" />

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/hugosleao)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/hugosleao)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:hugosleao.dev@gmail.com)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@hugosleao)

![Profile Views](https://komarev.com/ghpvc/?username=hugosleao&color=00ADD8&style=flat-square)

</div>

---

## About

My background is in DevOps and cloud automation, and today my focus is on **Platform Engineering and Cloud Architecture** — building and evolving cloud-native platforms that enable teams to ship software faster with reliable infrastructure, automation and strong engineering practices.

Inspired by how companies like **Spotify, Netflix and Mercado Livre** design Internal Developer Platforms — where a developer requests a service and the platform automatically provisions the repository, CI/CD, infrastructure and observability. No tickets. No manual steps. No AWS console access.

```
DevOps  ──────────────────────────────────────────────────▶  Platform Engineering
         Infrastructure    GitOps      Control Planes
         Automation        Systems     & IDPs
```

---

## 🏗️ Current Focus

| Area | What I'm working on |
|:---|:---|
| **Platform Engineering** | Internal Developer Platforms with developer self-service |
| **Control Plane Architecture** | Go Operators using `controller-runtime` + Kubernetes CRDs |
| **Cloud Architecture (AWS)** | EKS, Crossplane, VPC, IAM, Secrets Manager, OIDC |
| **GitOps** | ArgoCD ApplicationSets, multi-environment GitFlow |
| **Developer Experience** | Backstage portals, Golden Path templates, service scaffolding |
| **Infrastructure Abstraction** | Crossplane XRDs and Compositions for RDS, S3, SQS |

---

## ✅ Platform Capabilities

```
✔  Self-service service provisioning  — developer fills form, platform delivers
✔  GitOps continuous delivery         — Git is the only source of truth
✔  Infrastructure abstraction         — Crossplane Compositions for RDS · S3 · SQS
✔  Policy as code                     — Kyverno enforces standards at admission
✔  Developer portal                   — Backstage catalog, templates, scorecards
✔  Control plane architecture         — Go Operators with reconciliation loops
✔  Zero static credentials            — GitHub Actions OIDC + AWS STS
✔  Automated TLS                      — cert-manager + Let's Encrypt + Route53
```

---

## 🔬 Platform Engineering Lab

This GitHub profile documents my ongoing work designing and experimenting with **Internal Developer Platforms, Kubernetes control planes and cloud-native platform architectures**.

---

## 🚀 Featured Project

<div align="center">

### [platform-engineering-reference](https://github.com/hugosleao/platform-engineering-reference)

Reference architecture for building **Internal Developer Platforms on Kubernetes** — Backstage, ArgoCD, Crossplane and AWS.

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Backstage](https://img.shields.io/badge/Backstage-9BF0E1?style=flat-square&logo=backstage&logoColor=black)

</div>

> Production-grade **Internal Developer Platform** on Kubernetes.
> Same architecture principles used by **Spotify · Netflix · Mercado Livre · Uber**.

**Internal Developer Platform Architecture**

```mermaid
graph TD
    DEV(["👤 Developer<br/>fills form in Backstage"])
    BS["🖥️ Backstage<br/>Developer Portal · IDP"]
    API["⚙️ Platform API<br/>Go Operator · Reconcile Loop"]
    GH["📦 GitHub<br/>repo · CI/CD · branch protection"]
    GR["📂 gitops-repo<br/>ArgoCD Apps · Crossplane Claims"]
    ARGO["🔄 ArgoCD<br/>GitOps Engine · auto-sync"]
    POL["🛡️ Policy Layer<br/>Kyverno · admission control"]
    OBS["📊 Observability<br/>Prometheus · Grafana · audit log"]
    EKS["☸️ EKS Cluster<br/>Workloads · Crossplane"]
    AWS["☁️ AWS Infrastructure<br/>RDS · S3 · SQS · ECR"]

    DEV --> BS
    BS --> API
    API --> GH
    API --> GR
    GR --> ARGO
    ARGO --> POL
    POL --> EKS
    EKS --> AWS
    EKS --> OBS

    style DEV fill:#1f2937,stroke:#00ADD8,color:#fff
    style BS  fill:#1f2937,stroke:#9BF0E1,color:#fff
    style API fill:#1f2937,stroke:#00ADD8,color:#fff
    style GH  fill:#1f2937,stroke:#6e7681,color:#fff
    style GR  fill:#1f2937,stroke:#6e7681,color:#fff
    style ARGO fill:#1f2937,stroke:#EF7B4D,color:#fff
    style POL fill:#1f2937,stroke:#c084fc,color:#fff
    style OBS fill:#1f2937,stroke:#F46800,color:#fff
    style EKS fill:#1f2937,stroke:#326CE5,color:#fff
    style AWS fill:#1f2937,stroke:#FF9900,color:#fff
```

**What makes it different:** a Kubernetes **Operator** (Go + controller-runtime) continuously reconciles state — if a resource is deleted, it's recreated automatically. No manual intervention.

```
Developer fills a form in Backstage
  │
  ├──▶ Platform API (Go Operator) reconciles desired state
  │         │
  │         ├──▶ GitHub: repo + branch protection + CI/CD
  │         ├──▶ ArgoCD: Applications (dev / hml / prd)
  │         └──▶ Crossplane: RDS · S3 · SQS on AWS
  │
  └──▶ Developer gets a running service in minutes
```

---

## 🛠️ Tech Stack

<div align="center">

**Platform Engineering**

![Backstage](https://img.shields.io/badge/Backstage-9BF0E1?style=flat-square&logo=backstage&logoColor=black)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Crossplane](https://img.shields.io/badge/Crossplane-EF7B4D?style=flat-square&logoColor=white)
![Kyverno](https://img.shields.io/badge/Kyverno-326CE5?style=flat-square&logo=kubernetes&logoColor=white)

**Cloud & Infrastructure**

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![EKS](https://img.shields.io/badge/EKS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)

**Development**

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**Observability**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

</div>

---

## 📐 Engineering Approach

I study and build using three layers — ensuring knowledge stays valid even when tools evolve:

```
CONCEPT                   PATTERN                      IMPLEMENTATION
──────────────────────    ──────────────────────────   ────────────────────────
Continuous Delivery    →  GitOps                    →  ArgoCD
Operator Pattern       →  Controller + Reconcile    →  Platform API (Go)
Infrastructure IaC     →  Control Plane API         →  Crossplane
Policy as Code         →  Admission Control         →  Kyverno
Self-service           →  Developer Portal          →  Backstage
```

> Technology is secondary. **Architectural thinking is primary.**

---

## 🧭 Architecture Interests

```
• Internal Developer Platforms (IDP)
• Control Plane Architecture
• Cloud Native Systems Design
• Developer Experience Engineering
• Platform APIs and Infrastructure Abstraction
• GitOps and Continuous Delivery Systems
• Kubernetes Operators and CRD-driven workflows
• Policy as Code and Platform Governance
```

---

## 📚 Learning Journey

| Book | Author | What it influences |
|:---|:---|:---|
| **Platform Engineering on Kubernetes** | Mauricio Salatino | IDP architecture, Crossplane, ArgoCD |
| **Kubernetes Patterns** | Ibryam & Huß | Operator pattern, CRDs, reconcile loops |
| **Cloud Native DevOps with Kubernetes** | Arundel & Domingus | GitOps, observability, security |
| **API Design Patterns** | JJ Geewax | Control plane APIs, resource lifecycle |
| **Crafting Engineering Strategy** | Will Larson | Platform as product, engineering strategy |
| **Team Topologies** | Skelton & Pais | Platform team model, cognitive load, fast flow |
| **AWS SAA-C03** | Amazon | Cloud architecture, services, networking *(in progress)* |

---

<div align="center">

*Building platforms where developers focus on code — the platform handles everything else.*

</div>
