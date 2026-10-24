# 04 — Accounts Receivable (AR)

## 1. Objective
Understand how a company records customer invoices and manages money owed by customers in SAP S/4HANA Cloud Public Edition Finance.

## 2. Business Scenario
ABC India Pvt. Ltd. sells goods worth ₹20,000 to a customer on credit.

## 3. Accounting Entry — Customer Invoice

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Customer (Accounts Receivable) | 20,000 | |
| Sales Revenue | | 20,000 |
| **Total** | **20,000** | **20,000** |

## 4. Accounting Explanation
- **Customer — Debit:** The customer owes the company ₹20,000. Accounts Receivable is an asset, and an increase in an asset is recorded as a debit.
- **Sales Revenue — Credit:** Revenue increases when the company makes a sale.
- **Accounting Rule:** Total debits must equal total credits.

## 5. Business Process
1. Receive a customer order.
2. Deliver goods or services.
3. Create the customer invoice.
4. Post the invoice in the accounting system.
5. Receive payment from the customer.
6. Clear the outstanding customer balance.

## 6. SAP Processing — Customer Invoice

**Possible Fiori app:** Create Outgoing Invoices  
**Purpose:** Create a customer invoice, where supported by the available SAP configuration.

**Processing steps:**
1. Open the SAP Fiori launchpad.
2. Search for the relevant customer invoice app.
3. Enter the company code, customer, invoice date, and posting date.
4. Enter the amount and relevant revenue account details.
5. Check the invoice data.
6. Post the invoice if the app supports posting and all validations pass.
7. Record the accounting document number.

**Important:** The exact app and steps depend on your SAP Public Cloud trial and configuration. We will verify them in your system before marking this process as practised.

## 7. Technical References — T-Codes and Apps

| Reference | Purpose |
|---|---|
| Create Outgoing Invoices | Possible Fiori app for customer invoicing |
| FB70 | Enter customer invoice in classic SAP GUI |
| F-28 | Post incoming customer payment in classic SAP GUI |
| FBL5N | Display customer line items in classic SAP GUI |

Classic SAP GUI transaction codes may not be available in SAP S/4HANA Cloud Public Edition.

## 8. Accounting Entry — Customer Payment

**Business Scenario:** The customer pays the outstanding ₹20,000 through the company's bank.

| Account | Debit (₹) | Credit (₹) |
|---|---:|---:|
| Bank | 20,000 | |
| Customer (Accounts Receivable) | | 20,000 |
| **Total** | **20,000** | **20,000** |

**Explanation:**
- **Bank — Debit:** The company's bank balance increases.
- **Customer — Credit:** The customer's outstanding liability to the company decreases.

## 9. Verification and Testing
After posting in SAP, verify:
- Customer account
- Invoice amount
- Posting date
- Accounting document number
- Open customer balance
- Payment and clearing status

