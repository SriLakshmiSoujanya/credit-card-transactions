# 📋 SharePoint List Schema – Credit Card Transactions

This list is used by Power Automate flows to:

- Trigger email alerts when transactions exceed a threshold.
- Send a monthly usage summary to each user.

---

## 🔗 List Name:
**CreditCardTransactions**

---

## 📊 Columns Used:

| Column Name        | Data Type     | Description                                  |
|--------------------|---------------|----------------------------------------------|
| UserID             | Single line   | Unique ID to identify the user               |
| Gender             | Choice        | M / F                                        |
| City               | Single line   | City of the user                             |
| CardType           | Choice        | Gold / Platinum / Signature / Silver         |
| ExpenditureType    | Choice        | Bills, Travel, Food, etc.                    |
| TransactionAmount  | Number        | Amount spent in INR                          |
| TransactionDate    | Date & Time   | Date of the transaction                      |
| Email              | Single line   | Email address of the user                    |

---

## 🖼️ Screenshot of SharePoint List

Credit_Card_Sharepointlist.png

---

## 🔗 How It's Used in Flows

- **Flow 1 (HighTransactionAlert)**: Sends email alert if amount > ₹Threshold.
- **Flow 2 (MonthlyCreditCardReport)**: Sends summary email to users at month end.
