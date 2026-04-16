# State Drug Utilization Data 2025

Source: https://data.medicaid.gov/dataset/158a1baa-5506-400a-8ec3-97756f0b0536#data-table



## Description of Project

We will use State Drug Utilization Data provided by the Centers for Medicare & Medicaid 
Services. This dataset contains detailed information on outpatient drug utilization, prescription 
counts, and reimbursement amounts reported by state Medicaid programs. The data supports 
relational modeling by separating entities such as states, drugs identified by National Drug Code 
(NDC), and prescription utilization records across time periods. These entities enable multi-table 
schema design with primary and foreign key relationships.

The dataset contains messy attributes that require cleaning and transformation, including 
inconsistent drug naming conventions, National Drug Code formatting variations, suppressed or 
missing values, and currency-based reimbursement fields. The dataset also contains large-scale 
records across states and time periods, exceeding the minimum size requirement and justifying 
distributed Spark processing and complex joins.

## Personally Identifiable Information

There is no personally identifiable information in our data.

## Access Control

Bronze:	Data Engineers focused on creating reliable data ingestion from original source

Silver:	Data Scientists/Analysts for performing analysis in order to answer business-related questions

Gold:	Politician/Bureaucrats/Decision Makers for decision making 

## How to Run

1) Download CSV file from https://data.medicaid.gov/dataset/158a1baa-5506-400a-8ec3-97756f0b0536#data-table
2) Save the file to your Google Drive (not in a folder). The file name should be the same as it was when you downloaded it "StateDrugUtilizationData-2025.csv"
3) Open Jupyter Notebook "Phase4_CIS_660_Group_Project"
4) Hit "Run All"

## Authors

Sri Rakumari Mendu: Database & Schema Lead
Responsible for ERD design, PostgreSQL schema creation with primary and foreign key 
constraints, bulk data imports, and SQL analytics.

Vinay Kanth Challa: Processing & Spark Lead
Responsible for PySpark data cleaning logic, distributed transformations, data standardization, 
and Spark SQL implementation.

Robert Kratz-Hahn: Pipeline & Governance Lead
Responsible for medallion data architecture, data dictionary documentation, PII/security 
considerations, and final presentation flow.

## License

Data source: Medicaid State Drug Utilization Data available through the 
Centers for Medicare & Medicaid Services public data resources. The dataset is publicly 
available for research and analysis.

