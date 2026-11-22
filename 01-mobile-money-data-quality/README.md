# Mobile Money Transaction Data Quality Analysis

## 1. Project Overview

This project examines the quality and reliability of a sample mobile money transaction dataset using Python and Pandas.

The objective is to demonstrate how a data analyst identifies inconsistencies, cleans transaction records, validates financial data, and extracts meaningful business insights.

## 2. Business Problem

Transaction datasets may contain duplicate records, missing values, inconsistent labels, and invalid transaction amounts.

If these issues are not identified and addressed, they can affect transaction reporting, financial summaries, and business decisions.

This project applies a structured data quality assessment to identify and handle these issues.

## 3. Project Objectives

- Inspect the transaction dataset.
- Identify and remove exact duplicate records.
- Standardise transaction status labels.
- Identify missing and zero transaction amounts.
- Define valid successful transactions.
- Analyse transaction performance across payment channels.
- Present findings and practical recommendations.

## 4. Tools and Technologies

- Python
- Pandas
- Google Colab
- GitHub

## 5. Dataset Description

The project uses a small, synthetic mobile money transaction dataset created for learning and demonstration purposes.

The dataset contains transaction identifiers, dates, payment channels, transaction amounts, statuses, and agent locations.

It does not contain actual customer or financial institution records.

## 6. Data Quality Findings

Initial records: 16

Records after removing exact duplicates: 15

Remaining duplicate transaction IDs: 0

Missing transaction amounts: 1

Zero transaction amounts: 1

Transaction statuses after standardisation:

- Successful: 12
- Failed: 2
- Pending: 1

## 7. Analysis Approach

The analysis follows a structured workflow:

1. Data inspection
2. Duplicate identification and removal
3. Status standardisation
4. Numeric data validation
5. Missing and zero-value assessment
6. Identification of valid successful transactions
7. Transaction analysis by payment channel

## 8. Key Business Considerations

A successful transaction status does not automatically mean that its monetary value is valid.

Transactions with missing or zero amounts require investigation before they are included in financial reporting.

This distinction is important when calculating transaction volumes and monetary performance.

## 9. Limitations

The dataset is synthetic and contains only 16 original records.

Consequently, the findings demonstrate analytical methods rather than actual mobile money market performance.

## 10. Project Status

Data inspection, cleaning, data quality assessment, transaction validation, and channel performance analysis have been completed.

Three visualisations were created to examine successful transaction value, average transaction value, and transaction volume across payment channels.

Business insights and practical recommendations were developed based on the analysis.

The project demonstrates a structured approach to data quality assessment, financial data validation, exploratory data analysis, visualisation, and business intelligence.
