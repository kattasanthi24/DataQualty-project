# Data Quality Control

## Project Description: Data Quality Control Initiative at ABC Enterprises
This initiative aims to establish a secure and efficient data analytics framework that ensures high-quality, reliable, and compliant data for decision-making. By leveraging AWS tools, the project focuses on enriching, protecting, governing, and observing data to meet enterprise standards.

---

## Project Title:
Building a Comprehensive Data Governance and Analytics Platform

---

## Objective:
To design and implement a robust data pipeline that:  
1. Consolidates and standardizes data from diverse sources.  
2. Safeguards sensitive information with encryption and access controls.  
3. Automates data processing while ensuring compliance with data governance policies.  

---

## Background:
Inconsistent and fragmented datasets pose significant challenges to organizations. This project addresses these challenges by creating a centralized data management system. AWS services are used to standardize workflows, enhance security, and maintain data integrity while preparing datasets for advanced analytics.

---

## Scope:
1. **Data Enrichment**: Normalize and structure data using AWS Data Catalog and crawlers.  
2. **Data Protection**: Implement encryption, versioning, and replication for secure data storage.  
3. **Data Governance**: Define policies for data quality, consistency, and compliance.  
4. **Data Observability**: Monitor metrics, detect anomalies, and manage resources effectively.  

---

## Methodology:

### Data Enrichment
- **Consolidation and Structuring**: Sampled clickstream data was exported to the `cur-bucket` in JSON format, ensuring uniformity across sources.  
- **AWS Data Catalog**: Configured crawlers to scan and organize data into a centralized repository, enabling seamless querying and analysis.

![image](https://github.com/user-attachments/assets/16687739-352d-4549-bedd-e6202961a23c)

### Data Protection
- **Encryption with AWS KMS**: Configured symmetric keys to protect data at rest.  
- **Bucket Encryption**: Enabled default encryption on S3 buckets, ensuring automatic protection for new data.  
- **Versioning and Replication**: Enabled versioning for all buckets and established backup buckets with replication rules to prevent data loss.
### KMS-keys
![image](https://github.com/user-attachments/assets/02e502e0-c7eb-426f-9e4e-e8986348aa2f)

![Encrypted Buckets](https://github.com/user-attachments/assets/6c45a077-877c-4a47-bfda-9a5af26da15e)

### Data Governance
- **Sensitive Data Handling**: Identified and masked Personally Identifiable Information (PII) to ensure compliance.  
- **ETL Pipeline Design**: Developed a pipeline using AWS Glue for efficient data transformation and aggregation. Conditional routers were employed to route data into organized folders for downstream processing.

![ETL](https://github.com/user-attachments/assets/6bb15398-0f66-445c-865a-a5591daf8637)

###  Data Observability
- **CloudWatch Dashboards**: Designed to track key metrics such as storage usage, resource performance, and cost estimations. This visualization aids in maintaining optimal resource management and financial planning.

![Cloud Watch Dashbard](https://github.com/user-attachments/assets/913a7db5-de55-4278-a1ce-daf40d5e9f01)

---

## Deliverables:
1. **Consolidated Data**: Organized and cataloged datasets ready for analysis.  
2. **Secure Storage**: Encrypted, versioned, and replicated S3 buckets.  
3. **Automated Pipeline**: ETL pipeline for efficient and repeatable data processing.  
4. **Governance Framework**: Policies ensuring compliance and data quality.  
5. **Monitoring Dashboard**: CloudWatch-based visualizations for performance tracking.

---

## Timeline:
1. **Week 1-2**: Data collection, enrichment, and cataloging.  
2. **Week 3-4**: Implementation of encryption, versioning, and replication.  
3. **Week 5-6**: Development of governance policies and ETL pipeline.  
4. **Week 7**: Creation of observability dashboards and final testing.  

---

