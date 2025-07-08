---
layout: page
title: Projects
---

These are real-world infrastructure and automation engineering projects I’ve led and delivered at Avalara:

---

### 🛡️ Vulnerability Management at Scale

- Designed multi-layered dashboards in **Wiz** and **Tenable**, tracking vulnerabilities by **CVSSv2/v3**, remediation SLA, source (OS vs App), and fix lifecycle.
- Reduced vulnerability counts by over **80%** across environments, while defining operational exceptions for app-specific risks.
- Built SLA-centric dashboards (Critical: 30d, High: 60d, Medium: 90d), integrated with asset tags and scan metadata to drive prioritization.
- Provided technical enablement to remediation teams on dashboard use, automating data flows and actionable insights for real-time remediation.
- Maintained dashboards as IaC; visualizations were used in security audit reviews and internal compliance reporting.

---

### 🤖 Infrastructure Automation via Ansible + CI/CD

- Developed modular **Ansible playbooks** for:
  - .NET Core/Hosting Bundle deployments
  - SSMS and driver upgrade pipelines (ODBC/OLE DB)
  - CrowdStrike agent validation (pre/post resource capture)
  - Vulnerability mitigations (speculative execution, cfn-bootstrap cleanup)
  - Tenable Agent upgrades and service validation
- All workflows are pushed via GitLab → AAP → dynamic test inventories in AWS dev environments.
- Metrics streamed to **Grafana** via **Zabbix**, with health checks automated for service/process validation.
- Playbooks are reusable, version-controlled, and integrate with role-based inventory access across environments.
- **ChatGPT in VSCode** is used extensively to troubleshoot playbook logic, optimize loops, parse API data, and design complex conditionals.

---

### 🧠 Autonomous Post-Update Validation (Ansible + Slack + SSM)

- Engineered an **automated health verification system** that:
  - Runs system-wide diagnostics (CPU, memory, service status, agent health)
  - Triggers via Ansible schedule after scheduled maintenance events
  - Summarizes host-level results, uploads formatted CSV and message to Slack
- Ensures clean handoff post-maintenance and helps detect regression scenarios early

---

### 🌐 Automated Provisioning + Decommissioning (ServiceNow, Terraform, AAP)

- Built fully automated server provisioning pipeline:
  - **ServiceNow Catalog → GitLab CI → Terraform Infra Deploy → AAP Bootstrap**
  - Supports EC2 and Azure VMs, using reusable modules for OS, region, env-specific logic
- Decommissioning pipeline automates:
  - NetBox removal, DNS cleanup, AD unbinding, SSM deregistration, EBS tag removal
- Modular architecture enables multi-region, multi-account deployment and teardown
- Cost tags and infra metadata are appended for all compute resources by default

---

### ☁️ Lambda-Based System Lifecycle Orchestration (PowerOps)

- Designed **event-driven Lambda architecture** to auto-power on and off test systems:
  - Uses **EventBridge + Python Lambda** to detect 2nd Tuesday (Patch Tuesday)
  - Systems auto-start, monitored, and shut down exactly 3 days later
  - Sends Slack Webhook alerts to stakeholders on both power-on and off events
- Entire stack deployed via **Terraform**, with reusability across accounts
- This project introduced measurable **cost savings** by removing idle workloads in non-prod

---

### 🔒 IAM and Security Group Automation (for Okta + Infra Access)

- Created Ansible-based workflows to:
  - Provision SGs tied to Okta app roles and infra-access use cases
  - Define auto-tagging rules and enforce via Git-based IaC
  - Use domain-specific inventories to scope changes securely

---

### 🧩 Cost and Compliance Automation Across Multi-Cloud

- Defined tagging policies across **Azure subscriptions** and AWS accounts
- Used **Terraform modules** to enforce compliance at scale
- Maintained **custom patching baselines** and **tag-driven patch groups** in AWS Systems Manager
- Leveraged Tableau and cloud-native tools for cost analytics and optimization triggers

---

### 🔁 UDE Migration for Dynamics 365 F&O

- Lead migration of dev environments from LCS to **Power Platform Admin Center (UDE)**
- Provisioned Azure VMs, configured metadata sync with Visual Studio
- Automated UDE registration, developer access, and metadata refresh pipeline using GitLab, Terraform, and VS tooling

---

### 🧱 Engineering Best Practices

- Every solution follows **infrastructure-as-code** using **modular, reusable Terraform** that works across multiple cloud accounts.
- All workflows are integrated with **GitLab CI/CD**, include **AI-assisted logic validation**, and are built to be **self-healing and observable**.
- Systems are designed for scale, cost visibility, and environment parity between dev, test, and prod.