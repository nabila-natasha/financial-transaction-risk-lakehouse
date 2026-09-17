# Data Model

## 1. Modeling Approach

The analytical model separates transaction-risk facts from
reference/enrichment data.

## 2. Core Fact

### FACT_TRANSACTION

Grain:

One PaySim transaction.

Key attributes include:

- transaction sequence/time
- transaction type
- amount
- origin account
- destination account
- balance attributes
- fraud benchmark label

## 3. Dimensions

Potential dimensions include:

- DIM_DATE
- DIM_TRANSACTION_TYPE
- DIM_ACCOUNT

## 4. Enrichment

Foreign-exchange data is maintained separately at its
appropriate date/currency grain and joined to transaction
analytics only where the business meaning is valid.

## 5. Modeling Principle

The model avoids creating relationships merely because two
datasets contain similarly named fields.

Relationships must reflect the actual grain and business
meaning of the data.
