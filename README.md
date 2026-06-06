<<<<<<< HEAD
Clinical Sentinel: Data Governance & Integrity System
Overview
The Clinical Sentinel project provides an automated, secure framework for managing clinical service logs. By integrating Snowflake's data storage capabilities with Python-based ETL processes, this system ensures data integrity, maintains strict HIPAA compliance, and provides actionable governance reporting.

Project Structure
The repository is organized to ensure modularity and clear separation of concerns:

01_schema_setup.sql: Defines the foundational database infrastructure and table schemas for clinical logs.

02_data_quality_audit.sql: Contains automated SQL logic to perform data quality checks and identify anomalies.

03_compliance_reporting.sql: Implements views and queries for monitoring compliance scores and organizational reporting.

04_security_governance.sql: Manages Role-Based Access Control (RBAC) to enforce security and the principle of least privilege.

clinical_pipeline_demo.py: Production-level Python script for automated data ingestion and integrity verification.

clinical_pipeline_demo.ipynb: An interactive notebook demonstrating the pipeline’s workflow.

audit_export_2026_06_05.csv: Sample audit data export used for verification.

requirements.txt: Lists all necessary Python dependencies for the pipeline environment.

Key Features
Automated Data Ingestion: Employs snowflake-connector-python to ingest and validate clinical records.

Integrity Verification: Uses MD5 checksums (pd.util.hash_pandas_object) to confirm data consistency during transfer.

Governance & Security: Features robust SQL auditing and security scripts to ensure data privacy in alignment with healthcare standards.

Usage
Environment Setup: Ensure your environment includes the dependencies listed in requirements.txt.

Infrastructure: Execute the .sql scripts in the order defined (01 through 04) to set up the database environment.

Pipeline Execution: Run clinical_pipeline_demo.py to initiate the ETL process and perform integrity checks.
=======
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
>>>>>>> 1e6a1f7 (Update README with project documentation.)
