---
layout: page
title: Projects
---

<link rel="stylesheet" href="/assets/css/custom.css">

<div class="project-page">

# **Technical Projects & Automation Frameworks**

Each section below represents a major pillar of my work across multi-cloud automation, AI-driven orchestration, security engineering, compliance, identity governance, and enterprise lifecycle automation.  
All content is grouped by architectural domain, with card-style sections for clean presentation.

---

<!-- 1. Agentic AI Automation -->
<div class="card-section">

<h2>🚀 1. Agentic AI Automation & Distributed Knowledge Intelligence (DKI)</h2>

<p>
I build enterprise-grade agentic automation systems across AWS, Azure, and internal environments using <strong>n8n</strong>, 
<strong>Tines</strong>, and <strong>Cursor</strong>, capable of multi-step reasoning, cross-cloud orchestration, 
and deep operational insight. These pipelines combine event-driven serverless triggers, identity-aware controls, 
and Ansible-based execution layers to fully automate large-scale operational tasks with auditability.
</p>

<h3>AI-Driven Identity & Access Governance</h3>
<p>
I developed a complete User Access Review (UAR/UAC) automation framework that audits and validates access across 
Active Directory, Azure AD, DFS shares, finance systems, and engineering tooling.  
The workflow retrieves permission structures, evaluates access patterns, writes evidence into <strong>S3</strong> and 
<strong>Azure Blob Storage</strong>, routes decisions via Slack-based approvals, and updates access states through 
n8n + AAP integration.  
This system also handles automated <strong>security group and service account creation</strong> across clouds using IaC-defined 
roles and platform APIs.
</p>

<h3>Agentic Reasoning Pipelines (n8n + Cursor + Lovable)</h3>
<p>
I built a multi-layered reasoning engine where n8n orchestrates workflows while Cursor and Lovable perform 
contextual decision logic. This includes:
</p>

<ul>
  <li>Detecting RBAC drift and IaC drift across multiple subscriptions</li>
  <li>Identifying missing security agents, unhealthy services, or configuration anomalies</li>
  <li>Analyzing logs, comparing baselines, and deciding remediation steps</li>
  <li>Issuing validated operations through AAP job templates, SSM commands, or Azure Runbook triggers</li>
  <li>Publishing detailed Slack reports with logs, before/after evaluations, and validation evidence</li>
</ul>

<h3>Google Apps Integration & Credential Automation</h3>
<p>
I engineered a multi-cloud workflow for <strong>Google OAuth2 credential governance</strong> using custom-developed apps 
with granular scopes for Docs, Sheets, and Drive APIs.  
These credentials feed into distributed automation pipelines for:
</p>

<ul>
  <li>Generating compliance spreadsheets automatically</li>
  <li>Writing cost, security, and access analytics into Sheets</li>
  <li>Producing leadership-ready documents generated fully through n8n workflows</li>
</ul>

<p>
All workflows operate through secure credential rotation, HTTP-triggered dispatching, and Slack webhook–based notifications.
</p>

</div>

---

<!-- 2. Multi-Cloud Serverless Automation -->
<div class="card-section">

<h2>☁️ 2. Multi-Cloud Serverless Automation & Integration Layer (AWS • Azure • GCP)</h2>

<p>
I design automation systems built on serverless components that orchestrate cloud infrastructure, application lifecycles, 
governance policies, and compliance pipelines across AWS, Azure, and Google Cloud.  
These frameworks combine Lambda, EventBridge, Azure Automation Runbooks, Azure Functions, GCP service accounts, OAuth, 
and Terraform IaC modules into unified execution workflows.
</p>

<h3>AWS Lambda + EventBridge Automation Framework</h3>
<p>
I built a distributed AWS automation platform that performs:
</p>

<ul>
  <li>Scheduled EC2 start/stop for cost optimization across environments</li>
  <li>Automated snapshot creation, retention enforcement, and lifecycle cleanup</li>
  <li>Patch readiness and validation checks triggered post-maintenance windows</li>
  <li>Dynamic tagging enforcement and metadata governance</li>
  <li>Security posture scans integrated with SSM, CloudWatch, and Slack alerts</li>
</ul>

<p>
All logic is event-driven, highly modular, and easily extended with IaC (Terraform).
</p>

<h3>Azure Automation Runbooks & Functions Integration</h3>
<p>
I implemented automation workflows that control the operational lifecycle of Azure VMs, UDE developer machines, 
identity governance tasks, credential rotation, and security posture checks.  
These pipelines interact with Azure Monitor, Defender for Cloud, Runbooks, and EventHub to provide 
cross-environment operational oversight.
</p>

<h3>Multi-Cloud Credential, Service Account & OAuth Integration</h3>
<p>
I architected a central credential automation engine that manages:
</p>

<ul>
  <li>Azure AD app registrations with defined RBAC scopes</li>
  <li>Google Cloud OAuth apps for Docs, Sheets, Drive</li>
  <li>AWS IAM roles and cross-account execution policies</li>
  <li>GCP service accounts used by automation workflows</li>
  <li>Trigger pipelines for n8n via HTTP-based triggers or internal APIs</li>
</ul>

<p>
These credentials drive compliance, monitoring, automation, and analytics across the organization.
</p>

</div>

---

<!-- 3. Security, Compliance, Vulnerability -->
<div class="card-section">

<h2>🔐 3. Multi-Cloud Security, Compliance & Vulnerability Engineering</h2>

<p>
I build and maintain enterprise-wide security automation systems using crowd-based agents, 
tenant-wide governance policies, and multi-cloud compliance pipelines. These systems unify AWS, Azure, and GCP 
security posture into centralized dashboards and automated remediation playbooks.
</p>

<h3>Security Agent Deployment & Validation Automation</h3>
<p>
I implemented a zero-touch deployment and validation engine for <strong>CrowdStrike Falcon</strong> and 
<strong>Tenable</strong> across 500+ Windows and Linux servers.  
It validates agent health daily, detects anomalies, correlates results with cloud resource metadata, and triggers 
remediation workflows using SSM, AAP, or Runbooks.
</p>

<h3>Azure Tenant Root Governance (Policy-as-Code + CI/CD)</h3>
<p>
I manage Azure tenant governance with Terraform-driven policy enforcement pipelines that ensure:
</p>

<ul>
  <li>Consistent RBAC hierarchy inheritance</li>
  <li>Subscription-wide baseline policies</li>
  <li>Continuous compliance checks via CI/CD</li>
  <li>Automated tagging standards with corrective actions</li>
</ul>

<h3>Azure Defender for Cloud → EventHub Continuous Export</h3>
<p>
I engineered a complete continuous-export pipeline for security alerts, vulnerability data, configuration deviations, 
and compliance recommendations. This data feeds:
</p>

<ul>
  <li>SIEM platforms</li>
  <li>Grafana dashboards for vulnerability trends</li>
  <li>Internal Slack channels for engineering insights</li>
</ul>

<h3>Cost, Security & Usage Dashboards</h3>
<p>
I built cross-platform dashboards using <strong>Grafana</strong>, <strong>AWS Cost Explorer</strong>, 
<strong>Azure Cost Management</strong>, <strong>Wiz</strong>, <strong>Tenable</strong>, and <strong>Tableau</strong> 
to visualize:
</p>

<ul>
  <li>Vulnerability exposure & patch compliance</li>
  <li>Cost forecasting per environment</li>
  <li>Security posture drifts & anomalies</li>
  <li>AI usage trends & budget consumption</li>
</ul>

</div>

---

<!-- 4. Multi-Cloud Patch Orchestration -->
<div class="card-section">

<h2>🩺 4. Multi-Cloud Patch Orchestration & Lifecycle Automation</h2>

<p>
I automate enterprise patching across 500+ servers using AWS SSM, Azure Update Manager, and Ansible AAP.

These systems ensure reliable patching, complete validation, and full auditability with evidence stored centrally.
</p>

<h3>Patch Execution Framework</h3>
<p>
The automation framework includes:
</p>

<ul>
  <li>Baseline assignment & version validation</li>
  <li>Pre-patch health checks (CPU, memory, services, DNS, AD reachability)</li>
  <li>Event log parsing and anomaly detection</li>
  <li>Post-patch verification & service revalidation</li>
  <li>Snapshot lifecycles for safe rollback</li>
</ul>

<h3>Slack-Based Reporting Layer</h3>
<p>
A unified Slack reporting engine sends:
</p>

<ul>
  <li>Host-level validation summaries</li>
  <li>CSV reports of patch outcomes</li>
  <li>Vulnerability remediation suggestions</li>
  <li>Patch compliance scoring</li>
</ul>

</div>

---

<!-- 5. Infrastructure & IaC Engineering -->
<div class="card-section">

<h2>🏗 5. Infrastructure & IaC Engineering</h2>

<p>
I architect large-scale, modular Terraform libraries that standardize cloud deployments across AWS and Azure.

These modules support identity, networking, compute, governance, monitoring, storage, and developer workflows.
</p>

<h3>Terraform Architectural Modules</h3>
<p>
The module library includes patterns for:
</p>

<ul>
  <li>VPC/VNet foundations and subnets</li>
  <li>RBAC/IAM modeling</li>
  <li>Azure Policy & AWS Config integrations</li>
  <li>Developer VM provisioning (UDE integration)</li>
  <li>Global tagging strategies & metadata governance</li>
</ul>

<h3>CI/CD-Driven Infrastructure Governance</h3>
<p>
Policies, tagging rules, and compliance rulesets are validated through GitLab CI/CD pipelines
that enforce drift detection, corrective actions, and audit logging.
</p>

</div>

---

<!-- 6. AI Governance -->
<div class="card-section">

<h2>🤖 6. AI Governance, Usage Intelligence & Licensing Automation</h2>

<p>
I am responsible for the governance and lifecycle operations of enterprise AI tools including Cursor, Lovable, and ChatGPT.

My automations ensure secure onboarding/offboarding, cost controls, usage transparency, and compliance.
</p>

<h3>SCIM Automation & Usage Governance</h3>
<p>
I implemented SCIM-based automation that handles user provisioning, deactivation, and role enforcement.

Usage metrics are collected across platforms, processed into Sheets/Tableau, and summarized for leadership through Slack.
</p>

<h3>Budget Enforcement & Anomaly Detection</h3>
<p>
Automation workflows monitor:
</p>

<ul>
  <li>Daily and monthly usage trends</li>
  <li>Budget thresholds</li>
  <li>Unusual activity spikes</li>
  <li>Team-wise consumption patterns</li>
</ul>

<p>
Alerts are dispatched to Slack channels with direct links to corrective workflows.
</p>

</div>

---

<!-- 7. Dynamics UDE -->
<div class="card-section">

<h2>🧩 7. Dynamics 365 Lifecycle Engineering (LCS → UDE)</h2>

<p>
I engineered Avalara's transition from Microsoft LCS environments to Unified Development Environments (UDE)
using Power Platform Admin Center (PPAC).  
This involved automation of backend infrastructure, developer VM orchestration, metadata retrieval, 
and workspace initialization.
</p>

<h3>UDE Provisioning Framework</h3>
<p>
Automation handles:
</p>

<ul>
  <li>Environment creation in PPAC</li>
  <li>Developer VM provisioning via Azure automations</li>
  <li>Download & sync of F&O metadata</li>
  <li>Workspace bootstrapping</li>
  <li>Daily lifecycle operations driven by Runbooks</li>
</ul>

</div>

</div>
