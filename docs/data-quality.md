# Data Quality

## 1. Transaction Validation

Checks include:

- required fields
- valid transaction type
- non-negative transaction amount
- valid transaction sequence
- valid fraud labels
- duplicate detection
- account identifier completeness

## 2. Financial Consistency

Balance-related fields will be checked for logical
relationships where appropriate.

## 3. FX Validation

Checks include:

- valid currency codes
- valid dates
- non-null exchange rates
- duplicate date/currency combinations
- expected historical coverage

## 4. ML Data Quality

Before model training:

- verify target distribution
- check class imbalance
- prevent future information leakage
- preserve chronological ordering
- validate train/test separation

## 5. Testing

CI tests use small fixtures and do not require live Azure
resources.
