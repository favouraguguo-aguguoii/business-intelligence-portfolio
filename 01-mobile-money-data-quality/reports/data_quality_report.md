# Mobile Money Transaction Data Quality Report

## 1. Executive Summary

This project assesses the quality of a synthetic mobile money transaction dataset containing 16 original records.

The assessment identified an exact duplicate record, a missing transaction amount, a zero transaction amount, and inconsistent transaction status formatting.

After removing the exact duplicate, 15 records remained for further analysis.

## 2. Data Quality Assessment

| Assessment | Finding |
|---|---:|
| Original records | 16 |
| Records after duplicate removal | 15 |
| Remaining duplicate transaction IDs | 0 |
| Missing transaction amounts | 1 |
| Zero transaction amounts | 1 |

## 3. Transaction Status Distribution

Following standardisation, the transaction statuses were:

| Status | Records |
|---|---:|
| Successful | 12 |
| Failed | 2 |
| Pending | 1 |
| **Total** | **15** |

## 4. Exceptions Requiring Investigation

### Missing transaction amount

One transaction had a successful status but no recorded amount.

This record should be investigated before being included in financial reporting.

### Zero transaction amount

One successful transaction had an amount of GH₵0.

Although its status was marked successful, its financial value requires verification.

### Duplicate records

One exact duplicate was identified and removed, preventing the same transaction record from being counted twice.

## 5. Business Implications

Poor transaction data quality can affect:

- Financial reporting accuracy.
- Transaction reconciliation.
- Revenue and transaction-value calculations.
- Management decision-making.
- Operational monitoring.

A successful transaction status should not automatically be interpreted as proof of a valid monetary transaction.

## 6. Recommendations

1. Investigate successful transactions with missing amounts.
2. Verify zero-value transactions against transaction records.
3. Apply duplicate checks before reporting.
4. Standardise transaction status labels.
5. Establish data validation rules before financial analysis.

## 7. Limitations

The dataset is synthetic and contains only 16 original records.

The findings demonstrate data quality assessment techniques and should not be interpreted as evidence of actual mobile money industry performance.

## 8. Conclusion

The exercise demonstrates the importance of validating transaction data before conducting financial analysis.

Reliable business intelligence depends not only on analytical tools but also on the quality and integrity of the underlying data.
