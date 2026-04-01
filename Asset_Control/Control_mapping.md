| Risk ID | Risk Description | Control Recommendation | Control Type | ISO 27001 | NIST 800-53 | CIS Controls |
|--------|------------------|------------------------|--------------|-----------|-------------|--------------|
| R-001 | Public RDP exposure (Port 3389 open to internet) | Restrict RDP access via NSG to trusted IPs; implement VPN for secure access | Preventive | A.9.4 (System Access Control) | AC-17 (Remote Access) | 12.3 (Secure Remote Access) |
| R-002 | No MFA on admin account | Enforce Multi-Factor Authentication (MFA); create separate privileged accounts | Preventive | A.9.2 (User Access Management) | IA-2 (Identification & Authentication) | 6.3 (Access Control Management) |
| R-003 | Default OS configuration | Apply CIS hardening benchmarks; disable unnecessary services; enforce patching | Corrective | A.12.6 (Technical Vulnerability Mgmt) | CM-6 (Configuration Settings) | 5 (Secure Configuration) |
| R-004 | No centralized logging / SIEM | Enable centralized logging; configure alerting; integrate SIEM (e.g., Sentinel) | Detective | A.12.4 (Logging & Monitoring) | AU-2 (Audit Events) | 8 (Audit Log Management) |
| R-005 | Excessive privileges / unrestricted admin access | Implement RBAC; enforce least privilege; monitor admin activity | Preventive | A.6.1 (Information Security Roles) | AC-6 (Least Privilege) | 6 (Access Control Management) |
