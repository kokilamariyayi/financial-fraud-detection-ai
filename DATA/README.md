## Dataset Overview

This dataset contains financial transaction records used for detecting fraudulent
activities in mobile money platforms. The dataset consists of approximately
6.3 million transaction records and is widely used for fraud detection research
and machine learning experimentation.

Some transactions in the dataset were already flagged as fraudulent by existing
rule-based systems, making it suitable for analyzing the limitations of traditional
fraud detection approaches and improving them using machine learning.

> Note: The dataset is not included in this repository due to its large size
(≈ 493 MB). Only the dataset description and source link are provided.

---

## Transaction Types

- **CASH-IN**  
  Process of increasing the account balance by depositing cash through a merchant.

- **CASH-OUT**  
  Withdrawal of cash from a merchant, decreasing the account balance.

- **DEBIT**  
  Transfer of money from the mobile money service to a bank account.

- **PAYMENT**  
  Payment for goods or services, decreasing the sender’s balance and increasing
  the receiver’s balance.

- **TRANSFER**  
  Transfer of money between two users within the mobile money platform.

---

## Dataset Characteristics

- Highly imbalanced dataset (fraud cases are very rare)
- Tabular financial transaction data
- Binary classification problem
- Suitable for real-world fraud detection modeling

---

## Columns Description

| Column Name        | Description |
|--------------------|-------------|
| step               | Time step of the transaction |
| type               | Type of transaction |
| amount             | Transaction amount |
| nameOrig           | Source account identifier |
| oldbalanceOrg      | Sender balance before transaction |
| newbalanceOrig     | Sender balance after transaction |
| nameDest           | Destination account identifier |
| oldbalanceDest     | Receiver balance before transaction |
| newbalanceDest     | Receiver balance after transaction |
| isFraud            | Target label (1 = Fraud, 0 = Not Fraud) |

---

## Target Variable

- **isFraud**
  - `1` → Fraudulent transaction  
  - `0` → Legitimate transaction

---

## License

MIT License

---

## Dataset Source

The dataset is publicly available and can be accessed from:
[https://www.kaggle.com/datasets/ntnu-testimon/paysim1](https://www.kaggle.com/datasets/amanalisiddiqui/fraud-detection-dataset)

---

## Usage

This dataset is primarily used for:
- Learning and experimentation
- Research in financial fraud detection
- Building and evaluating machine learning models
