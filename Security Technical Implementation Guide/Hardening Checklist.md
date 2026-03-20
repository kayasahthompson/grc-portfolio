# STIG Hardening Checklist: Aether Edge Cloud Assets
**Framework:** DISA STIG (Defense Information Systems Agency)  
**Target:** Red Hat Enterprise Linux (RHEL 8) / AWS Cloud  
**Objective:** To ensure all Aether Edge assets meet Department of Defense (DoD) security standards for government contracting readiness.

---

## 1. Top 5 High-Severity (CAT I) Findings & Fixes
As part of the hardening process for the Aether Edge financial database, the following STIG requirements were addressed:

| STIG ID | Vulnerability Title | Severity | Fix / Mitigation Applied |
| :--- | :--- | :--- | :--- |
| **V-230233** | Root Login via SSH | **CAT I** | Disabled PermitRootLogin in `/etc/ssh/sshd_config`. |
| **V-230221** | Unencrypted Telnet | **CAT I** | Uninstalled `telnet-server`; enforced SSH (v2) for all remote admin. |
| **V-230326** | Password Complexity | **CAT II** | Configured `pam_pwquality` to require min 15 chars & special chars. |
| **V-230381** | Audit Log Overflow | **CAT II** | Set `max_log_file_action` to `rotate` to prevent system shutdown. |
| **V-230237** | Banner/Legal Notice | **CAT III** | Configured `/etc/issue` with the mandatory DoD "Privacy Act" warning. |

## 2. Methodology: "The STIG Viewer"
I utilized the **DISA STIG Viewer** to cross-reference our **RS-1003 (Cloud Misconfiguration)** risk against the RHEL 8 STIG baseline. This ensures that our cloud infrastructure isn't just "secure," but is "Audit Ready" for federal oversight.

## 3. Continuous Monitoring
To maintain compliance, I recommend the use of **OpenSCAP** for automated weekly scans to detect "configuration drift" away from these STIG requirements.

---
*Note: This project demonstrates my ability to apply DISA security standards to enterprise systems in a cleared environment.*
