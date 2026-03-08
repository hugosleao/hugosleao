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

I build **Internal Developer Platforms** that eliminate the friction between writing code and running it in production.

My focus is on **control plane architecture** — systems where a developer requests a service, and the platform automatically provisions the repository, CI/CD pipeline, infrastructure and observability. No tickets. No manual steps. No AWS console access.

Currently evolving from **DevOps operations** into **Platform Engineering and Cloud Architecture**, applying architectural patterns from industry leaders like Spotify, Netflix and Mercado Livre to real production-grade labs.

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

## 🚀 Featured Project

<div align="center">

### [platform-engineering-reference](https://github.com/hugosleao/platform-engineering-reference)

![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat-square&logo=argo&logoColor=white)
![Backstage](https://img.shields.io/badge/Backstage-9BF0E1?style=flat-square&logo=backstage&logoColor=black)

</div>

> Production-grade **Internal Developer Platform** on Kubernetes.
> Same architecture principles used by **Spotify · Netflix · Mercado Livre · Uber**.

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

**What makes it different:** a Kubernetes **Operator** (Go + controller-runtime) continuously reconciles state — if a resource is deleted, it's recreated automatically. No manual intervention.

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

## 📚 Learning Journey

| Book | Author | What it influences |
|:---|:---|:---|
| **Platform Engineering on Kubernetes** | Mauricio Salatino | IDP architecture, Crossplane, ArgoCD |
| **Kubernetes Patterns** | Ibryam & Huß | Operator pattern, CRDs, reconcile loops |
| **Cloud Native DevOps with Kubernetes** | Arundel & Domingus | GitOps, observability, security |
| **API Design Patterns** | JJ Geewax | Control plane APIs, resource lifecycle |
| **Crafting Engineering Strategy** | Will Larson | Platform as product, engineering strategy |
| **Team Topologies** | Skelton & Pais | Platform team model, cognitive load, fast flow |

---

## 📊 Stats

<div align="center">

<img height="160" src="https://github-readme-stats.vercel.app/api?username=hugosleao&show_icons=true&theme=dark&hide_border=true&count_private=true&bg_color=0d1117&title_color=00ADD8&icon_color=00ADD8" />
<img height="160" src="https://github-readme-stats.vercel.app/api/top-langs/?username=hugosleao&layout=compact&theme=dark&hide_border=true&bg_color=0d1117&title_color=00ADD8&langs_count=6" />

</div>

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com?user=hugosleao&theme=dark&hide_border=true&background=0d1117&ring=00ADD8&fire=00ADD8&currStreakLabel=00ADD8)

</div>

---

<div align="center">

*Building platforms where developers focus on code — the platform handles everything else.*

</div>
