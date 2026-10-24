# 03 — Accounts Payable (AP)

## 1. Objective
Understand how a company records supplier invoices and manages amounts owed to suppliers in SAP S/4HANA Cloud Public Edition Finance.

## 2. Business Scenario
ABC India Pvt. Ltd. purchases goods worth ₹10,000 from a supplier on credit.

## 3. Accounting Entry

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Purchases Expense | 10,000 | |
| Supplier (Accounts Payable) | | 10,000 |
| **Total** | **10,000** | **10,000** |

## 4. Accounting Explanation
- **Purchases Expense — Debit:** The purchase is recorded as an expense in this simplified example.
- **Supplier — Credit:** The company owes ₹10,000 to the supplier, increasing its liability.
- **Accounting Rule:** Total debits must equal total credits.

## 5. Business Process
1. Receive goods or services from a supplier.
2. Receive the supplier invoice.
3. Verify the invoice details.
4. Record the supplier invoice in the accounting system.
5. Pay the supplier according to the agreed payment terms.

## 6. SAP Learning Notes
Accounts Payable is part of Financial Accounting (FI). In SAP, supplier invoices create accounting impacts in the relevant expense or asset account and the supplier reconciliation account.

The exact posting process depends on the business scenario and the SAP apps available.

## 7. Project Status
This is a self-created learning scenario. The accounting entry has not yet been posted in SAP.
## 8. Supplier Payment Scenario

### Business Scenario
ABC India Pvt. Ltd. pays the outstanding supplier amount of ₹10,000 through its bank.

### Accounting Entry

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Supplier (Accounts Payable) | 10,000 | |
| Bank | | 10,000 |
| **Total** | **10,000** | **10,000** |

### Accounting Explanation
- Supplier — Debit: The outstanding liability decreases.
- Bank — Credit: The company's bank asset decreases.
- Business Impact: The supplier balance is cleared, and the bank balance decreases by ₹10,000.

## 9. SAP Processing Steps and Technical References

### A. Create and Post a Supplier Invoice

**Fiori App:** Create Supplier Invoice  
**App ID:** F0859  
**Purpose:** Record a supplier invoice in SAP.

**Navigation and Processing:**
1. Log in to the SAP Fiori launchpad.
2. Search for "Create Supplier Invoice".
3. Open the app.
4. Enter the company code.
5. Enter the supplier invoice date and posting date.
6. Enter the supplier invoice reference and gross invoice amount.
7. Enter the supplier details and relevant G/L account items.
8. Check the invoice details and required fields.
9. Select Post, if available and all validations pass.
10. Record the generated accounting document number.

**Expected Accounting Impact:**
- Debit: Relevant expense or asset account.
- Credit: Supplier reconciliation account.

### B. Technical Reference — T-Codes and App IDs

| Transaction / App ID | Purpose |
|---|---|
| F0859 | Create and manage supplier invoices |
| MIRO | Advanced supplier invoice processing |
| MIR7 | Park or hold an advanced supplier invoice |
| F0718 | Post General Journal Entries; for supported G/L postings, not supplier invoice posting |

Note: These are technical references. Availability depends on the SAP product, release, authorizations, and app configuration. Classic SAP GUI transaction codes may not work in every Public Cloud trial.

### C. Verification

After posting, open the relevant supplier invoice list or document display app and verify:
- Supplier account
- Invoice amount
- Posting date
- Accounting document number
- Debit and credit balances

### D. Learning Status

The processing steps are documented for learning purposes. Actual SAP posting and document verification must be performed in the available SAP trial before being marked complete.
