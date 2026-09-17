# Financial Transaction Risk & Anomaly Analytics Lakehouse

## 1. Business Problem

Financial institutions need to identify unusual transaction
patterns, understand changes in account behaviour and evaluate
risk indicators while controlling false positives.

This project demonstrates a cloud lakehouse architecture for
transaction-risk and anomaly analytics.

## 2. Business Questions

- Which transaction patterns are unusual?
- Which accounts demonstrate abnormal behaviour over time?
- What proportion of transactions are flagged as potentially
  risky?
- How well do unsupervised anomalies overlap with known
  benchmark fraud labels?
- How do rules, Isolation Forest and XGBoost compare?

## 3. Core Data Sources

### PaySim

Synthetic historical transaction data replayed through
Event Hubs to simulate transaction-event arrival.

### Frankfurter

Daily foreign-exchange rates used as enrichment data.

## 4. Streaming Approach

Historical PaySim transactions are replayed at an accelerated
cadence.

This simulates event arrival for architectural demonstration
and does not represent a live banking transaction stream.

## 5. ML Approach

The project evaluates:

- rule-based detection
- Isolation Forest
- XGBoost classification

The known PaySim fraud label is used as a benchmark for
evaluation.

## 6. Limitations

PaySim is synthetic benchmark data and does not represent
actual bank customers or production banking transactions.

The resulting models are therefore demonstrated as
analytical techniques rather than production fraud-detection
systems.
