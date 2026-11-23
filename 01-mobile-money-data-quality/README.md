# Mobile Money Transaction Data Quality Analysis

## 1. Project Overview

This project examines the quality and reliability of a sample mobile money transaction dataset using Python and Pandas.

The objective is to demonstrate how a data analyst identifies inconsistencies, cleans transaction records, validates financial data, and extracts meaningful business insights.

### How to Run the Project

1. Download or clone this repository.
2. Open `mobile_money_data_quality.ipynb` in Google Colab.
3. Download `sample_transactions.csv` from `data/raw/`.
4. Run the notebook using **Runtime → Run all**.
5. When prompted, upload the downloaded `sample_transactions.csv` file.
6. Allow the notebook to execute all analysis and visualizations.

### Requirements

- Python
- pandas
- Matplotlib
- Google Colab or Jupyter Notebook

### Project Structure

```text
01-mobile-money-data-quality/
├── README.md
├── notebooks/
│   ├── mobile_money_data_quality.ipynb
│   └── mobile_money_data_quality_old.ipynb
├── data/
│   ├── raw/
│   │   └── sample_transactions.csv
│   └── processed/
│       └── cleaned_transactions.csv
└── reports/
    └── data_quality_report.md

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

### Key Findings

- 16 original records were reduced to 15 after removing an exact duplicate.
- 1 missing transaction amount and 1 zero-value transaction were identified.
- 10 valid successful transactions were analysed.
- Total successful transaction value: GH₵4,120.
- Average successful transaction value: GH₵412.
- Bank Transfer recorded the highest total transaction value at GH₵1,700.

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

### Analytical Limitations

- The dataset is synthetic and contains only 16 original records.
- The findings demonstrate an analytical workflow but do not represent actual customer behavior.
- A larger real-world dataset would be needed to establish reliable business trends.

## 10. Project Status

Data inspection, cleaning, data quality assessment, transaction validation, and channel performance analysis have been completed.

Three visualisations were created to examine successful transaction value, average transaction value, and transaction volume across payment channels.

Business insights and practical recommendations were developed based on the analysis.

The project demonstrates a structured approach to data quality assessment, financial data validation, exploratory data analysis, visualisation, and business intelligence.
