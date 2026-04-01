# ☁️ Cloud Security Risk Assessment (GRC Simulation – Microsoft Azure)

## 📌 Overview

This project presents a structured **Governance, Risk, and Compliance (GRC) assessment** of a cloud-hosted virtual machine in Microsoft Azure. The objective was to identify security risks, evaluate their potential impact, and recommend controls aligned with industry-standard frameworks.

The assessment simulates a real-world enterprise scenario where misconfigurations in cloud environments can introduce significant security and compliance risks.

---

## 🎯 Objectives

* Perform a cloud-based risk assessment using GRC principles
* Identify and classify assets, threats, and vulnerabilities
* Quantify risks using a structured scoring model
* Map security controls to recognized compliance frameworks
* Provide actionable remediation and governance recommendations

---

## 🏗️ Environment & Scope

* **Cloud Platform:** Microsoft Azure
* **Resource Type:** Virtual Machine (Windows Server 2022)
* **Access Method:** Remote Desktop Protocol (RDP)
* **Exposure:** Public IP enabled

### Scope Limitations

* Single virtual machine assessment
* No additional cloud services (e.g., storage, IAM, SIEM) included
* Non-exploitative (GRC-focused assessment only)

---

## 🔍 Methodology

The assessment followed a structured GRC lifecycle:

1. **Asset Identification**
   Identified critical components including compute, identity, network access, and logs.

2. **Threat Modeling**
   Evaluated realistic threat scenarios such as brute-force attacks, privilege abuse, and unauthorized configuration changes.

3. **Vulnerability Analysis**
   Identified weaknesses including public RDP exposure, lack of MFA, default OS configurations, and absence of centralized monitoring.

4. **Risk Assessment & Scoring**
   Applied a quantitative model:

   * Likelihood (1–5)
   * Impact (1–5)
   * Risk Score = Likelihood × Impact

5. **Control Mapping**
   Mapped risks to industry frameworks including:

   * ISO 27001
   * NIST 800-53
   * CIS Controls

6. **Mitigation Planning**
   Developed security and governance recommendations to reduce risk exposure.

---

## 📊 Key Findings

| Risk Area                 | Description                                              | Risk Level |
| ------------------------- | -------------------------------------------------------- | ---------- |
| Public RDP Exposure       | Open port (3389) accessible from the internet            | Critical   |
| Lack of MFA               | Single admin account without multi-factor authentication | Critical   |
| Default OS Configuration  | No system hardening or baseline enforcement              | High       |
| No Centralized Monitoring | Absence of SIEM/log aggregation                          | Medium     |
| Excessive Privileges      | Unrestricted administrative access                       | Medium     |

---

## 🛡️ Control Recommendations

### Access Control

* Restrict RDP access to trusted IP ranges
* Implement Multi-Factor Authentication (MFA)
* Enforce least privilege using role-based access control (RBAC)

### System Hardening

* Apply CIS benchmarks
* Disable unnecessary services and ports
* Automate patch management

### Monitoring & Detection

* Enable centralized logging (SIEM integration)
* Configure alerting for suspicious activities
* Retain logs for compliance requirements

### Governance & Compliance

* Define and enforce access control policies
* Monitor administrative activities
* Align configurations with ISO 27001 and NIST standards

---

## 📈 Risk Scoring Model

| Metric     | Scale                            |
| ---------- | -------------------------------- |
| Likelihood | 1 (Rare) – 5 (Almost Certain)    |
| Impact     | 1 (Insignificant) – 5 (Critical) |
| Risk Score | Likelihood × Impact (1–25)       |

---

## 🧠 Business Impact

If left unaddressed, the identified risks could result in:

* Unauthorized access to cloud resources
* Potential data breaches
* Regulatory non-compliance
* Reputational damage and operational disruption

---

## 🧰 Tools & Technologies

* Microsoft Azure
* Windows Server 2022
* Azure Network Security Groups (NSG)
* Event Viewer (Logging)

---

## 📁 Repository Structure

```
cloud-grc-risk-assessment-azure/
│
├── README.md
├── report/
│   └── Cloud_Security_Risk_Assessment.pdf
├── diagrams/
├── risk-register/
├── controls/
└── evidence/
```

---

## 🚀 Key Skills Demonstrated

* GRC Risk Assessment Methodology
* Cloud Security (Azure)
* Threat & Vulnerability Analysis
* Risk Quantification
* Control Mapping (ISO 27001, NIST, CIS)
* Security Governance & Compliance

---

## 🔑 Key Takeaways

* Cloud misconfigurations are a major source of security risk
* Strong identity and access management is critical
* Monitoring and logging are essential for detection and response
* Aligning technical controls with compliance frameworks improves security posture

---

## 📌 Future Improvements

* Expand scope to include Azure Active Directory (IAM)
* Integrate Microsoft Defender for Cloud
* Implement SIEM (e.g., Microsoft Sentinel)
* Add automated compliance assessments

---

## 👤 Author

**Abubakar Yusuf**
GRC / SOC Analyst

---

## ⭐ Project Value

This project demonstrates the ability to bridge **technical cloud security issues with governance, risk, and compliance requirements**, a critical capability for modern cybersecurity roles.
