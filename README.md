<div align="center">

<!-- ANIMATED HERO BANNER -->
<img src="./assets/banner.svg" alt="Sarvesh Kumar Mishra - Senior DevSecOps Engineer &amp; Cloud Architect" width="100%" />

<br/>

# Sarvesh Kumar Mishra
### **Senior DevSecOps Engineer &bull; Enterprise Cloud Architect &bull; Technical Lead**
**16+ Years Total IT Experience | 7+ Years Specialized in DevSecOps & Multi-Cloud Architecture**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Sarvesh_Kumar_Mishra-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sarveshkumarmishra)
[![Email](https://img.shields.io/badge/Email-Contact_Sarvesh-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sarvesh.mishra.devsecops@gmail.com)
[![Location](https://img.shields.io/badge/Location-Open_for_Global_&_Remote-2ea44f?style=for-the-badge&logo=google-maps&logoColor=white)](#-get-in-touch--lets-collaborate)
[![Status](https://img.shields.io/badge/Status-Open_for_Lead_/_Architect_Roles-8A2BE2?style=for-the-badge&logo=target&logoColor=white)](#-executive-profile--career-narrative)

<p align="center">
  <b>Architecting Resilient Multi-Cloud Foundations &bull; Shifting Security Left &bull; Driving 100+ Workload Enterprise Migrations &bull; Scaling FinOps & Governance</b>
</p>

---

</div>

## 📌 Executive Profile & Career Narrative

I am a **Senior DevSecOps Engineer and Cloud Architect** with **16+ years of total IT industry experience**, including **7+ years dedicated to enterprise-scale DevSecOps, cloud migration, and Infrastructure as Code (IaC)**. 

Throughout my career, I have operated at the intersection of **business strategy, systems architecture, and engineering leadership**. I specialize in designing and delivering enterprise Azure and AWS landing zones, orchestrating zero-downtime migrations (100+ multi-tier workloads), hardening defense-in-depth security postures (CIS/ISO27001), and implementing automated DevSecOps pipelines that shift security left without throttling developer velocity.

```
                           [ How to Look Unique? ]
                                      │
                                [ Portfolio ]
                                      │
                     ┌────────────────┴────────────────┐
                     │                                 │
                [ Freshers ]                    [ Experienced ]
                                                       │
                                      ┌────────────────┴────────────────┐
                                      │ 1. Resume (Impact & metrics)    │
                                      │ 2. LinkedIn (Thought leader)    │
                                      │ 3. Job Portals (Keywords)       │
                                      │ 4. GitHub (Production IaC/Pipelines)
                                      │ 5. Technical Blog & ADRs        │
                                      └─────────────────────────────────┘
```

> **The Senior Mindset:** Senior engineers and architects do not merely configure tools; we answer fundamental questions: *"What is the business? What is the functional domain? What is the impact on ROI, reliability, and security?"* My approach aligns infrastructure blueprints with organizational revenue, risk management, and governance.

---

## ⚡ High-Impact Executive Metrics

| Metric | Business & Engineering Value Delivered | Primary Technologies / Domains |
|:---|:---|:---|
| **16+ Years** | Proven track record spanning enterprise IT infrastructure, systems engineering, and cloud transformation | Enterprise Architecture & Leadership |
| **7+ Years** | Hands-on DevSecOps, automated CI/CD governance, and multi-cloud security hardening | Azure DevOps, GitHub Actions, Jenkins, Checkov, Trivy |
| **100+ Workloads** | Seamless end-to-end datacenter-to-Azure migration executed with **zero unexpected downtime** | Azure Migrate, CAF, Hub-and-Spoke, ASR |
| **28%+ OPEX Saved** | Continuous FinOps cost governance via rightsizing, automated scheduling, and log tuning | Infracost, Azure Cost Mgmt, Reserved Instances |
| **100% Guardrails** | Automated drift detection and CIS Level 2 benchmark policy enforcement across management groups | Terraform, Azure Policy, Defender for Cloud |
| **99.99% Uptime** | High-availability compute architectures with multi-region disaster recovery (RTO &lt; 1h / RPO &lt; 15m) | VMSS, Azure Site Recovery, ZRS/GRS |

---

## 🏛️ The 10 Scalability & Quality Pillars

Every enterprise solution and landing zone I architect is anchored in these ten non-negotiable architectural pillars:

```
┌────────────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                    10 Scalability & Quality Pillars                                    │
│                                                                                                        │
│   1. Scalable       2. Robust        3. Secure        4. Reliable        5. Portable                   │
│   6. Governed       7. High Avail    8. Cost-Optim    9. Backed Up      10. Compliant & Monitored      │
└────────────────────────────────────────────────────────────────────────────────────────────────────────┘
```

```mermaid
flowchart TD
    subgraph CorePillars ["🏛️ Enterprise Architecture & Governance Pillars"]
        P1["1. Scalable & Robust<br/>(VMSS, Auto-scaling, Multi-AZ)"]
        P2["2. Secure & Compliant<br/>(CIS L2, Zero-Trust, Entra ID PIM)"]
        P3["3. Reliable & Portable<br/>(IaC Terraform, Containers, Multi-Cloud)"]
        P4["4. FinOps & Cost-Optimized<br/>(28%+ Savings, Rightsizing, RIs)"]
        P5["5. Backed Up & Observable<br/>(ASR, RTO < 1h, RPO < 15m, AMA DCR)"]
    end
```

---

## 🌐 Enterprise Hub-and-Spoke Reference Architecture

This production-grade Hub-and-Spoke network topology ensures secure cross-premises connectivity, centralized traffic inspection, and strict network segmentation for enterprise multi-tier workloads.

```mermaid
flowchart TD
    subgraph OnPrem ["🏢 On-Premises Enterprise Datacenter"]
        DC["Core Datacenter Infrastructure / Legacy Systems"]
    end

    subgraph HubVNet ["🛡️ Azure HUB VNet (Central Connectivity & Security)"]
        GW["GatewaySubnet<br/>(ExpressRoute / S2S VPN Gateway)"]
        FW["Azure Firewall Premium / NVA<br/>(TLS Inspection & Central Egress)"]
        DNS["Azure Private DNS Zones<br/>(Centralized PaaS Resolution)"]
    end

    subgraph SpokeApp ["📦 Spoke 1: Production Application VNet"]
        AppTier["App Tier Subnet<br/>(VMSS / AKS Workloads)"]
        DBTier["Database Tier Subnet<br/>(Private Endpoints)"]
        NSG1["Network Security Groups & ASGs"]
    end

    subgraph SpokeShared ["⚙️ Spoke 2: Shared Services & DevSecOps VNet"]
        Runners["Self-Hosted CI/CD Runners<br/>(Azure DevOps / Jenkins)"]
        Bastion["Azure Bastion Host"]
        SecTools["Vulnerability & Monitoring Agents"]
    end

    DC <-->|"ExpressRoute / S2S VPN"| GW
    GW --> FW
    FW <-->|"VNet Peering & UDR 0.0.0.0/0 Route"| SpokeApp
    FW <-->|"VNet Peering & UDR 0.0.0.0/0 Route"| SpokeShared
    DBTier -.->|"Private Endpoint Resolution"| DNS
```

### Key Networking Architectural Decisions:
* **IP Address Management (IPAM) & CIDR:** Rigorous pre-migration assessment of on-prem IP pools to ensure zero overlapping CIDR ranges across Azure VNets.
* **Forced Centralized Traffic Inspection:** User Defined Routes (UDRs) forcing `0.0.0.0/0` and all spoke-to-spoke traffic through the Azure Firewall / Network Virtual Appliance (NVA).
* **Controlled Ingress & Egress:** Inbound traffic routed through Azure Application Gateway / Azure Front Door with Web Application Firewall (WAF); outbound traffic secured via TLS inspection.
* **Zero Public PaaS Exposure:** All PaaS services (Key Vault, Storage Accounts, SQL Databases) communicate exclusively over Private Endpoints with centralized Private DNS zone resolution linked to the Hub.

---

## 🔒 Multi-Layered Defense-in-Depth Security Framework

Security is not an afterthought; it is integrated across every tier of the enterprise ecosystem:

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                              Multi-Layered Defense-in-Depth                            │
├────────────────────────────────────────────────────────────────────────────────────────┤
│  1. Identity Level   │ Entra ID • PIM (JIT Approvals) • Conditional Access • MFA       │
│  2. Network Level    │ Hub-and-Spoke • NSG / ASG Micro-segmentation • Azure Firewall   │
│  3. Governance Level │ Azure Policy (CIS Benchmark) • Defender for Cloud Secure Score  │
│  4. Compute & Data   │ Defender for Servers • CMK Disk Encryption • Automated Patching │
└────────────────────────────────────────────────────────────────────────────────────────┘
```

| Security Layer | Implemented Enterprise Controls & Technology Stack |
|:---|:---|
| **Identity & Access** | **Microsoft Entra ID**, Conditional Access Policies, Mandatory MFA, **Privileged Identity Management (PIM)** with just-in-time time-bound access, Managed Identities (eliminating hardcoded credentials). |
| **Network Perimeter** | Hub-and-Spoke isolation, NSGs/ASGs micro-segmentation, **Azure Firewall Premium** with IDPS & TLS inspection, DDoS Protection Standard, Private Endpoints for PaaS. |
| **Governance & Policy** | **Azure Policy & Initiatives** (CIS Azure Benchmark v2.0, Microsoft Cloud Security Benchmark), automated audit/deny triggers, compliance reporting dashboards. |
| **Compute & Workload** | **Microsoft Defender for Servers**, automated OS patch baselines, disk encryption with **Customer Managed Keys (CMK)**, immutable Azure Storage containers. |
| **Secrets & Keys** | **Azure Key Vault** with Azure RBAC authentication, automated certificate rotation, envelope encryption. |

---

## 🚀 DevSecOps Shift-Left CI/CD & IaC Governance Pipeline

Every infrastructure change is governed by an automated, trunk-based pipeline that verifies syntax, audits security vulnerabilities, estimates cloud costs, and prevents configuration drift.

```mermaid
flowchart LR
    A["💻 Git Commit<br/>(Trunk-Based)"] --> B["🔍 Pre-Commit Lint<br/>(tflint & terraform fmt)"]
    B --> C["🛡️ Shift-Left Security<br/>(Checkov, Trivy, Gitleaks)"]
    C --> D["💰 FinOps Cost Audit<br/>(Infracost Delta)"]
    D --> E["📋 Terraform Plan<br/>(Remote State Lock)"]
    E --> F["👥 Peer Review Gate<br/>(CODEOWNERS: 2+ Reviewers)"]
    F --> G["🚀 Terraform Apply<br/>(Azure Blob Lease Locked)"]
    G --> H["📊 Observability<br/>(Drift Detection & Telemetry)"]
```

### DevSecOps Quality & Branching Safeguards:
* **Trunk-Based Development:** Short-lived feature branches (`feature/*`, `fix/*`) merged frequently to reduce merge debt.
* **Mandatory Branch Protection:** Direct push and branch deletion strictly disabled on `main` and production branches.
* **Peer Reviews:** Mandatory Pull Request approvals from at least **two senior reviewers** governed by `CODEOWNERS`.
* **Shift-Left Security Scanners:** Automated gates blocking PRs if high/critical CVEs are detected by Checkov, Trivy, or tfsec.
* **Secrets Sanitization:** Pre-commit hooks and pipeline stages running **Gitleaks** to prevent secret leakage.
* **Automated Drift Detection:** Scheduled nightly pipelines running `terraform plan -detailed-exitcode` to detect and alert on unauthorized manual portal changes immediately.

---

## 🗺️ 100+ Workload Enterprise Cloud Migration Strategy

A proven, systematic blueprint for migrating mission-critical enterprise workloads from on-premises datacenters to Azure with **zero unexpected business disruption**.

```mermaid
flowchart LR
    S1["1. Discovery<br/>• Inventory & Dependency Map<br/>• Azure Migrate Appliances"] --> S2["2. Assessment<br/>• Readiness & Sizing<br/>• TCO & ROI Projections<br/>• Wave Planning"]
    S2 --> S3["3. Landing Zone<br/>• CAF Architecture<br/>• Hub-and-Spoke Network<br/>• Identity & Governance"]
    S3 --> S4["4. Cutover Execution<br/>• DB Replication Sync<br/>• DNS TTL Reduction<br/>• Maintenance Window"]
    S4 --> S5["5. Hypercare<br/>• 24x7 War Room Support<br/>• Performance Baseline<br/>• FinOps Rightsizing"]
```

### Comprehensive Migration Playbook:
1. **Discovery & Assessment:** Deployed Azure Migrate lightweight appliances to catalog 100+ multi-tier workloads, analyze process-level network dependencies, and calculate compute/storage TCO.
2. **Landing Zone Readiness (Microsoft CAF):** Established structured Management Group hierarchies, subscription boundaries (Dev, UAT, Prod), and automated network landing zones prior to workload movement.
3. **Execution & Cutover:** Asynchronous data replication, pre-cutover DNS TTL lowering to 300s, automated cutover scripts, and immediate smoke/sanity test suites.
4. **Hypercare & Optimization:** Dedicated 2-4 week war room support, real-time application performance monitoring via Azure Monitor, and post-migration FinOps rightsizing.

---

## 💰 FinOps: Cloud Financial Management & Optimization

Cloud architecture is incomplete without cost governance. By treating cost as a primary architectural constraint, I consistently reduce cloud waste while preserving performance:

```
┌────────────────────────────────────────────────────────────────────────────────────────────────┐
│                                   FinOps Optimization Framework                                 │
├────────────────────────────────────────────────────────────────────────────────────────────────┤
│  1. Waste Elimination │ Automated cleanup of unattached disks, orphan public IPs & snapshots  │
│  2. Dynamic Sizing    │ Compute rightsizing based on 30-day P95 utilization telemetry          │
│  3. Commitment Savings│ Strategic 1-Yr & 3-Yr Reserved Instances (RI) & Azure Savings Plans    │
│  4. Workload Scheduling│ Automated start/stop runbooks for non-production environments         │
│  5. Log Ingestion Cut │ Azure Monitor Data Collection Rules (DCR) filtering noisy diagnostics  │
└────────────────────────────────────────────────────────────────────────────────────────────────┘
```

* **Eliminating Idle Resources:** Scheduled Azure Automation runbooks and Logic Apps identifying unattached disks, obsolete snapshots, and unused public IP addresses.
* **Predictable Cost Modeling:** CI/CD pipeline integration with **Infracost** delivering real-time monthly cost diffs on pull requests before infrastructure is provisioned.
* **Log Ingestion Tuning:** Configured Data Collection Rules (DCR) in the Azure Monitor Agent (AMA) to filter out high-volume, low-value security events, slashing Log Analytics ingestion costs by over 30%.

---

## 📡 Observability, SRE & Disaster Recovery Baselines

Ensuring 99.99% system availability through proactive observability, structured incident routing, and resilient disaster recovery mechanisms:

| Dimension | Strategy & Implementation Architecture |
|:---|:---|
| **Centralized Observability** | Single-pane telemetry via Azure Monitor and centralized **Log Analytics Workspaces** segmented by enterprise landing zone. |
| **Agent Architecture** | High-performance **Azure Monitor Agent (AMA)** configured with fine-grained Data Collection Rules (DCR). |
| **Intelligent Alert Routing** | Action Groups dynamically dispatching critical alerts to Microsoft Teams, Slack, and **PagerDuty** with automated escalation matrices. |
| **Disaster Recovery (DR)** | Primary-to-secondary region replication orchestrated via **Azure Site Recovery (ASR)** guaranteeing **RTO &lt; 1 hour** and **RPO &lt; 15 minutes**. |
| **Storage Redundancy** | Tiered storage strategies leveraging Locally Redundant (LRS), Zone-Redundant (ZRS), and Geo-Redundant Storage (GRS) based on data criticality. |

---

## 👥 Technical Leadership & Delivery Governance

Operating at the Lead/Architect level requires balancing hands-on deep-dive technical engineering with executive stakeholder management:

```
+------------+       +---------------+       +---------+       +----------------------+       +----------------+
|   Sales    | ----> |   Pre-Sales   | ----> |   TAM   | ----> | Enterprise Architect | ----> | Technical Lead |
| Commercial |       | Techno-       |       | Tech    |       | Infra + Application  |       | Infra / App    |
| Focus      |       | Functional    |       | Account |       | Strategy & Design    |       | Execution      |
|            |       | Proposals     |       | Manager |       |                      |       |                |
+------------+       +---------------+       +---------+       +----------------------+       +----------------+
```

* **Pre-Sales & Solutioning:** Authoring techno-functional proposals, responding to enterprise RFPs/RFIs, creating technical estimation models, and delivering architecture POCs.
* **Vendor & Partner Governance:** Managing Statement of Work (SOW) definitions, objective **Technical Evaluation Matrices**, SLA enforcement, and deliverable sign-offs.
* **Governance Frameworks:** Formulating Standard Operating Procedures (SOPs), conducting blameless incident retrospectives, and enforcing RACI matrices across cross-functional squads.
* **Engineering Mentorship:** Running structured Knowledge Transfer (KT) sessions, upskilling junior and mid-level engineers in DevSecOps practices, and chairing Architecture Review Boards (ARBs).

---

## 🛠️ Comprehensive Technical Skill Spectrum

<div align="center">

### Cloud Platforms & Enterprise Infrastructure
![Microsoft Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Amazon AWS](https://img.shields.io/badge/Amazon_AWS-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Hybrid Cloud](https://img.shields.io/badge/Hybrid_Cloud-ExpressRoute_/_VPN-00599C?style=for-the-badge&logo=azure-networking&logoColor=white)
![Landing Zones](https://img.shields.io/badge/Enterprise_Landing_Zones-CAF-008AD7?style=for-the-badge&logo=azure-devops&logoColor=white)

### Infrastructure as Code & Configuration
![Terraform](https://img.shields.io/badge/Terraform-844FBA?style=for-the-badge&logo=terraform&logoColor=white)
![Azure Bicep](https://img.shields.io/badge/Azure_Bicep-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=for-the-badge&logo=ansible&logoColor=white)
![ARM Templates](https://img.shields.io/badge/ARM_Templates-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)

### CI/CD, DevSecOps & Shift-Left Security
![Azure DevOps](https://img.shields.io/badge/Azure_DevOps_Pipelines-0078D7?style=for-the-badge&logo=azure-devops&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=for-the-badge&logo=jenkins&logoColor=white)
![Checkov](https://img.shields.io/badge/Checkov-2C3437?style=for-the-badge&logo=bridgecrew&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-0052CC?style=for-the-badge&logo=aquasec&logoColor=white)
![GitLeaks](https://img.shields.io/badge/Gitleaks-Red-B81D24?style=for-the-badge&logo=security&logoColor=white)
![Infracost](https://img.shields.io/badge/Infracost-00D084?style=for-the-badge&logo=infracost&logoColor=black)

### Containers & Orchestration
![Kubernetes](https://img.shields.io/badge/Kubernetes_(AKS/EKS)-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Helm](https://img.shields.io/badge/Helm_Charts-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![Container Registry](https://img.shields.io/badge/ACR_/_ECR-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)

### Identity, Security & Governance
![Microsoft Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID_(AAD)-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Azure PIM](https://img.shields.io/badge/Azure_PIM-JIT_Access-00599C?style=for-the-badge&logo=azure-devops&logoColor=white)
![Microsoft Defender](https://img.shields.io/badge/Defender_for_Cloud-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Azure Policy](https://img.shields.io/badge/Azure_Policy-CIS_Compliance-008AD7?style=for-the-badge&logo=azure-devops&logoColor=white)
![HashiCorp Vault](https://img.shields.io/badge/HashiCorp_Vault-000000?style=for-the-badge&logo=vault&logoColor=white)

### Observability, SRE & Scripting
![Azure Monitor](https://img.shields.io/badge/Azure_Monitor_/_AMA-0078D4?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Log Analytics](https://img.shields.io/badge/Log_Analytics_(KQL)-00599C?style=for-the-badge&logo=microsoft-azure&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Bash](https://img.shields.io/badge/Bash_Shell-4EAA25?style=for-the-badge&logo=gnu-bash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

</div>

---

## 📂 Featured Enterprise Architecture Blueprints

Explore select architectural frameworks, IaC boilerplates, and automated pipeline templates:

<table>
  <tr>
    <td width="50%">
      <h3>🏛️ <a href="https://github.com/Sarvesh0401/azure-enterprise-landing-zone">azure-enterprise-landing-zone</a></h3>
      <p>Production-grade Terraform module creating a Microsoft CAF-compliant Hub-and-Spoke topology with Azure Firewall Premium, Private DNS zones, and automated subnet micro-segmentation.</p>
      <code>Terraform</code> &bull; <code>Azure</code> &bull; <code>Hub-and-Spoke</code> &bull; <code>Zero-Trust</code>
    </td>
    <td width="50%">
      <h3>🛡️ <a href="https://github.com/Sarvesh0401/devsecops-pipeline-accelerator">devsecops-pipeline-accelerator</a></h3>
      <p>Modular Azure DevOps and GitHub Actions YAML pipeline templates embedding shift-left security (Checkov, Trivy, Gitleaks) and FinOps cost estimation (Infracost) before apply gates.</p>
      <code>CI/CD</code> &bull; <code>Checkov</code> &bull; <code>Trivy</code> &bull; <code>Infracost</code>
    </td>
  </tr>
  <tr>
    <td width="50%">
      <h3>💰 <a href="https://github.com/Sarvesh0401/azure-finops-governance-toolkit">azure-finops-governance-toolkit</a></h3>
      <p>Automated PowerShell and Azure CLI runbooks to detect unattached disks, prune stale snapshots, rightsize compute clusters, and generate cost-anomaly alerts.</p>
      <code>FinOps</code> &bull; <code>Automation</code> &bull; <code>Cost Optimization</code> &bull; <code>PowerShell</code>
    </td>
    <td width="50%">
      <h3>☸️ <a href="https://github.com/Sarvesh0401/hardened-aks-baseline">hardened-aks-baseline</a></h3>
      <p>Secure Azure Kubernetes Service (AKS) cluster deployment featuring Private Clusters, Azure CNI, Pod Identity / Workload Identity, Calico network policies, and Key Vault CSI driver.</p>
      <code>Kubernetes</code> &bull; <code>AKS</code> &bull; <code>Helm</code> &bull; <code>Micro-segmentation</code>
    </td>
  </tr>
</table>

---

## 📊 GitHub Analytics & Engineering Pulse

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Sarvesh0401&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0b0f19&title_color=38bdf8&icon_color=00f2fe&text_color=94a3b8" alt="Sarvesh's GitHub Stats" height="165" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sarvesh0401&layout=compact&theme=tokyonight&hide_border=true&bg_color=0b0f19&title_color=38bdf8&text_color=94a3b8" alt="Top Languages" height="165" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Sarvesh0401&theme=tokyonight&hide_border=true&background=0b0f19&ring=38bdf8&fire=00f2fe&currStreakLabel=38bdf8" alt="Streak Stats" width="49%" />

</div>

---

## 🤝 Get in Touch & Let's Collaborate

Whether you are seeking a **Senior / Lead DevSecOps Engineer**, an **Enterprise Cloud Architect** to guide high-stakes cloud migrations, or technical advisory on establishing secure, cost-governed cloud platforms:

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sarveshkumarmishra)
[![Email](https://img.shields.io/badge/Email-sarvesh.mishra.devsecops@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:sarvesh.mishra.devsecops@gmail.com)
[![GitHub](https://img.shields.io/badge/GitHub-Follow_@Sarvesh0401-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Sarvesh0401)

<br/>

```
"Infrastructure is code. Security is continuous. Scalability is non-negotiable."
```

**Designed & Architected with 🛡️ by Sarvesh Kumar Mishra**

</div>
