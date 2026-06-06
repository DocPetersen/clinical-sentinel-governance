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