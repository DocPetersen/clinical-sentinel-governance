# 🏥 Clinical Sentinel
### *Automating Data Integrity & HIPAA Compliance in the Cloud*

---

## 🔍 The Problem
In clinical data environments, **data corruption** and **privacy leaks** are critical risks. Traditional manual audits are slow, prone to human error, and fail to provide real-time assurance that patient data remains accurate and secure during transmission.

## 💡 The Solution
**Clinical Sentinel** is an end-to-end automated governance framework. It bridges the gap between raw clinical log ingestion and boardroom-ready compliance reporting by enforcing **data integrity at the source** and **security at the destination.**



## 🛠 Tech Stack & Workflow
* **Pipeline Engine**: Python (`pandas`, `snowflake-connector`)
* **Warehouse**: Snowflake (Cloud Data Platform)
* **Governance Logic**: SQL (Audit Trails, RBAC, Compliance Views)
* **Security**: MD5 Hash Verification & Least-Privilege Access Control

## 📈 Impact
* **Zero-Trust Integrity**: Every record is verified via MD5 checksums upon ingestion.
* **Compliance Automation**: Real-time identification of non-compliant records (e.g., missing HIPAA-mandated signatures).
* **Operational Security**: Strict Role-Based Access Control (RBAC) ensures sensitive PII is only accessible to authorized personnel.

## 📂 Project Navigation
| Component | Purpose |
| :--- | :--- |
| `clinical_pipeline_demo.py` | The automated ingestion engine. |
| `02_data_quality_audit.sql` | The automated integrity "watchdog." |
| `04_security_governance.sql` | The security perimeter enforcement. |

---
*Built to demonstrate scalable, secure, and auditable Data Engineering practices.*
