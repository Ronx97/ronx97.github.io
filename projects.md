---
layout: page
title: Projects
---

Here are a few automation and infrastructure projects I’ve led at Avalara:

### 🛡️ Vulnerability Remediation Dashboards
- Built real-time dashboards in Wiz and Tenable for SLA-based vulnerability tracking.
- Categorized vulnerabilities by severity (Critical/High/Medium) and type (OS vs App).
- Enabled reporting on remediated vs open issues across all environments.

### 🤖 Ansible Automation for Security Tools
- Developed workflows to test and validate CrowdStrike sensor updates.
- Integrated with Zabbix + Grafana for pre- and post-update metrics (CPU, memory).
- Triggered and monitored via Ansible Automation Platform synced from GitLab.

### 🌐 Server Provisioning and Deprovisioning Automation
- Built Terraform-based server deployment logic integrated with ServiceNow.
- Orchestrated full infra lifecycle with human approval checkpoints via Ansible.

### ☁️ Patch Compliance via AWS SSM & Azure Policies
- Created custom patch baselines and tag-driven patch groups in AWS SSM.
- Defined Azure policies to enforce tagging and automate compliance.
- Standardized patching across Windows, Amazon Linux, and hybrid nodes.

### 🔁 UDE Migration for Dynamics 365 F&O
- Led UDE setup in PPAC for F&O dev environments.
- Provisioned Azure dev VMs and configured Visual Studio sync for metadata.
- Automated supporting infrastructure deployment via Terraform and Azure.

All projects followed infra-as-code practices using Terraform, Git, Ansible, and GitLab CI/CD.