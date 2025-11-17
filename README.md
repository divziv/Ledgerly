# Ledgerly


📄 Dataset Description

This dataset contains detailed transactional records used for analytics, classification, and machine-learning tasks.
Below is a description of all columns included in the dataset:

🧾 Columns

1. timestamp
   The exact date and time when the transaction occurred (ISO format).
2. customer_id
   Unique identifier assigned to the customer who performed the transaction.
3. customer_country
   Country where the customer’s account or profile is registered.
4. merchant_country
   Country where the merchant or service provider is located.
5. merchant_mcc
   Merchant Category Code (MCC) representing the merchant’s business type.
6. merchant
   Name of the merchant, store, vendor, or service provider for the transaction.
7. category
   Top-level financial category (e.g., Lifestyle Spending, Income, Investments) assigned to the transaction.
8. subcategory
   More granular classification detailing the specific nature of the transaction (e.g., Fast food, Stock purchase).
9. amount
   The monetary value of the transaction.
10. currency
    Currency in which the transaction amount is denominated (e.g., INR, USD).
11. payment_method
    Payment instrument used (e.g., UPI, Card, Netbanking, Wallet, PayPal).
12. channel
    Mode or environment through which the transaction was initiated (e.g., ONLINE, POS, ATM, MOBILE_APP).
13. terminal_id
Identifier of the terminal or POS machine where the transaction was processed (empty if not applicable).
14. card_last4
    Last four digits of the payment card used (shown only for card transactions).
15. is_recurring
    Binary flag indicating whether the transaction is part of a recurring series (1 = yes, 0 = no).
16. is_subscription
    Binary flag showing whether the transaction corresponds to a subscription service (1 = yes, 0 = no).
17. is_international
    Binary flag showing whether the transaction is cross-border (customer_country ≠ merchant_country).
18. description
    Realistic and sometimes noisy text describing the transaction (may include spelling errors, casing changes, symbols).
19. txn_ref
    Unique transaction reference number generated for the transaction.
20. label
    Ground-truth subcategory label used for training machine learning models.
21. payment_classification_type
    Top-level category grouping used for model training, reporting, or analytics (same as “category”).