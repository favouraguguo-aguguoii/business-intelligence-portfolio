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

## 6. Transaction Performance Analysis

Following data cleaning and validation, successful transactions with positive monetary amounts were selected for financial analysis.

A total of 10 valid successful transactions were identified, representing a combined transaction value of GH₵4,120.

### Performance by Payment Channel

| Payment Channel | Transaction Count | Total Value (GH₵) | Average Value (GH₵) |
|---|---:|---:|---:|
| Bank Transfer | 2 | 1,700 | 850 |
| Card | 4 | 1,520 | 380 |
| Mobile Money | 4 | 900 | 225 |
| **Overall** | **10** | **4,120** | **412** |

The analysis shows differences in transaction volume and monetary value across the three payment channels.

## 7. Key Business Insights

1. **Bank Transfer recorded the highest total transaction value.** It generated GH₵1,700 from only two successful transactions, giving it the highest average transaction value of GH₵850.

2. **Card and Mobile Money recorded the highest transaction volumes.** Each channel had four valid successful transactions.

3. **Card generated more transaction value than Mobile Money.** Despite having the same transaction count, Card generated GH₵1,520 compared with Mobile Money's GH₵900.

4. **Mobile Money recorded the lowest average transaction value.** Its average was GH₵225, compared with GH₵380 for Card and GH₵850 for Bank Transfer.

## 8. Business Recommendations

1. Investigate why Mobile Money has a lower average transaction value than Card, despite both channels recording the same number of valid successful transactions.

2. Examine whether Bank Transfer attracts higher-value transactions or customers, given its higher average transaction value.

3. Monitor both transaction volume and total transaction value when evaluating payment channel performance.

4. Maintain data validation controls to ensure missing amounts, zero-value transactions, and duplicate records are investigated before financial reporting.

## 9. Data Quality Recommendations

1. Investigate successful transactions with missing amounts.
2. Verify zero-value transactions against transaction records.
3. Apply duplicate checks before reporting.
4. Standardise transaction status labels.
5. Establish data validation rules before financial analysis.

## 10. Limitations

The dataset is synthetic and contains only 16 original records.

The findings demonstrate data quality assessment techniques and should not be interpreted as evidence of actual mobile money industry performance.

## 11. Conclusion

The exercise demonstrates the importance of validating transaction data before conducting financial analysis.

Reliable business intelligence depends not only on analytical tools but also on the quality and integrity of the underlying data.
