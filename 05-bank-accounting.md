# 05 — Bank Accounting and Bank Reconciliation

## 1. Objective
Understand how a company records bank transactions and reconciles its accounting records with the bank statement.

## 2. Business Scenario
ABC India Pvt. Ltd. has the following transactions:
- Receives ₹20,000 from a customer into its bank account.
- Pays ₹10,000 to a supplier through its bank account.

## 3. Accounting Entry — Customer Receipt

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Bank | 20,000 | |
| Customer (Accounts Receivable) | | 20,000 |
| **Total** | **20,000** | **20,000** |

**Explanation:** Bank is debited because the company's bank balance increases. The customer account is credited because the outstanding receivable decreases.

## 4. Accounting Entry — Supplier Payment

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Supplier (Accounts Payable) | 10,000 | |
| Bank | | 10,000 |
| **Total** | **10,000** | **10,000** |

**Explanation:** The supplier account is debited because the liability decreases. Bank is credited because the company's bank balance decreases.

## 5. What Is Bank Reconciliation?
Bank reconciliation compares the company's bank account records with the bank statement to identify differences.

Examples of differences include:
- Bank charges not yet recorded in the books.
- Deposits not yet reflected on the bank statement.
- Payments issued but not yet processed by the bank.
- Errors or duplicate transactions that need investigation.

## 6. Simple Bank Reconciliation Example

| Particulars | Amount (₹) |
|---|---:|
| Balance as per company bank ledger | 50,000 |
| Less: Bank charges not yet recorded | 500 |
| Adjusted balance | 49,500 |

**Accounting entry for bank charges:**

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Bank Charges Expense | 500 | |
| Bank | | 500 |
| **Total** | **500** | **500** |

This example assumes the bank has already deducted the charges, but the company has not yet recorded them.

## 7. SAP Processing and Technical References

### Possible Fiori Apps
- **Manage Bank Statements:** Review and manage imported bank statements, where available.
- **Reprocess Bank Statement Items:** Investigate and resolve bank statement items that require additional processing, where available.
- **Manage Bank Accounts:** View or maintain bank account master data, subject to authorization.

The exact app names and availability depend on your SAP S/4HANA Cloud Public Edition release and configuration.

### Classic SAP GUI T-Codes
| T-Code | Purpose |
|---|---|
| FF_5 | Import electronic bank statements in supported classic SAP GUI systems |
| FEBAN | Process electronic bank statement items in supported classic SAP GUI systems |
| FBL3N | Display G/L account line items in classic SAP GUI |

These are technical references, not a guarantee that the codes are available in your Public Cloud trial.

## 8. Practical Testing Checklist
When the relevant SAP apps are available:
1. Identify the bank G/L account.
2. Review the recorded bank transactions.
3. Review or import the bank statement if supported.
4. Compare statement items with accounting records.
5. Investigate unmatched items.
6. Record any required adjustments.
7. Confirm the remaining differences are explained.

