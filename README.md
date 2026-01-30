# CRM Data Cleaning & Validation

## Overview
This project demonstrates how I clean, validate, and prepare CRM lead data for downstream sales and operations use.

## Problem
Incoming CRM data often contains:
- Missing required fields
- Duplicate leads
- Invalid values (email, phone)

## Data
- Source: Simulated CRM export
- Format: CSV
- Records: 5,000+
- Note: This dataset is a simulated CRM export created for portfolio demonstration purposes. Data quality issues were intentionally introduced to reflect real-world operational scenarios.

## Approach
- Defined data quality rules
- Used SQL to identify duplicates and invalid records
- Standardized fields for reporting readiness
- Used SQL-based validation checks to assess data completeness, format correctness, and duplication risk prior to CRM ingestion.
- Enforced controlled lead_source values to ensure consistent attribution and reporting accuracy

## Output
- Cleaned dataset
- SQL queries for validation
- Documented data quality rules
- Generated a cleaned CRM dataset by enforcing required-field rules, validating email formats, standardizing text fields, and removing duplicate records.
- Reduced raw dataset from 5,000 records to 3762 validated, ingestion-ready leads.

## Tools Used
- SQL
- Excel / Google Sheets

## Data Quality Impact

| Metric                        | Before Cleaning | After Cleaning |
|-------------------------------|-----------------|----------------|
| Total lead records            |      5,000      |      3762      |
| Leads with valid email        |      4,598      |      3762      |
| Leads with company populated  |      5,000      |      3762      |
| Leads with valid lead source  |      5,000      |      3762      |
| Duplicate emails              |      18         |        0       |
| Leads with valid phone number |      4,104      |      3762      |

### Summary
By enforcing data quality rules and removing invalid or duplicate records, the dataset was reduced from 5,000 raw leads to 3762 ingestion-ready records. This process eliminated 18 duplicate entries and ensured 100% compliance with required field and lead source standards, improving downstream CRM reliability and reporting accuracy.
