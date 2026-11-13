# 8-K filings of the first 30 SEC ticker entries since 2025-07-01 — item tallies, three pulls, 40 filings read

Summary: For the first 30 registrants in SEC company_tickers.json (fixed in pull 1), every Form 8-K and 8-K/A filed from 2025-07-01 was pulled three times at least 24 hours apart (466, 467 and 469 rows), tallied by item code, and the 40 most recent qualifying pull-1 filings by acceptanceDateTime were read item by item from their EDGAR documents.

## Registrants

registrants_raw: 30
registrants kept: 30
duplicates dropped: 0

The first 30 entries (keys "0" to "29") of www.sec.gov/files/company_tickers.json, in file order, fixed in pull 1. A repeated CIK keeps its first entry; no CIK repeated, so all 30 remain.

| # | Ticker | Company (as company_tickers.json gives the title) | CIK |
|---|---|---|---|
| 0 | AAPL | Apple Inc. | 0000320193 |
| 1 | NVDA | NVIDIA CORP | 0001045810 |
| 2 | MSFT | MICROSOFT CORP | 0000789019 |
| 3 | GOOGL | Alphabet Inc. | 0001652044 |
| 4 | AMZN | AMAZON COM INC | 0001018724 |
| 5 | META | Meta Platforms, Inc. | 0001326801 |
| 6 | AVGO | Broadcom Inc. | 0001730168 |
| 7 | TSLA | Tesla, Inc. | 0001318605 |
| 8 | LLY | ELI LILLY & Co | 0000059478 |
| 9 | BRK-B | BERKSHIRE HATHAWAY INC | 0001067983 |
| 10 | WMT | Walmart Inc. | 0000104169 |
| 11 | SKHY | SK hynix Inc. | 0002120882 |
| 12 | JPM | JPMORGAN CHASE & CO | 0000019617 |
| 13 | AMD | ADVANCED MICRO DEVICES INC | 0000002488 |
| 14 | MU | MICRON TECHNOLOGY INC | 0000723125 |
| 15 | V | VISA INC. | 0001403161 |
| 16 | JNJ | JOHNSON & JOHNSON | 0000200406 |
| 17 | XOM | ExxonMobil Holdings Corp | 0002115436 |
| 18 | ASML | ASML HOLDING NV | 0000937966 |
| 19 | MA | Mastercard Inc | 0001141391 |
| 20 | ABBV | AbbVie Inc. | 0001551152 |
| 21 | COST | COSTCO WHOLESALE CORP /NEW | 0000909832 |
| 22 | KO | COCA COLA CO | 0000021344 |
| 23 | PLTR | Palantir Technologies Inc. | 0001321655 |
| 24 | CVX | CHEVRON CORP | 0000093410 |
| 25 | PG | PROCTER & GAMBLE Co | 0000080424 |
| 26 | CSCO | CISCO SYSTEMS, INC. | 0000858877 |
| 27 | ORCL | ORACLE CORP | 0001341439 |
| 28 | MRK | Merck & Co., Inc. | 0000310158 |
| 29 | UNH | UNITEDHEALTH GROUP INC | 0000731766 |

## Pull 1 — 8k-30-filers-pull1.csv

row count: 466
CSV SHA-256: a488df1534dc386644dfa9c6f30dfda2473f7015b1de93cf13a6a3efbf063aba
Pull date (UTC): 2026-11-11

### Rows per registrant

| Company | CIK | Rows | Share of rows (%) |
|---|---|---|---|
| ADVANCED MICRO DEVICES INC | 0000002488 | 19 | 4.08 |
| AMAZON COM INC | 0001018724 | 18 | 3.86 |
| ASML HOLDING NV | 0000937966 | 0 | 0.00 |
| AbbVie Inc. | 0001551152 | 22 | 4.72 |
| Alphabet Inc. | 0001652044 | 22 | 4.72 |
| Apple Inc. | 0000320193 | 14 | 3.00 |
| BERKSHIRE HATHAWAY INC | 0001067983 | 12 | 2.58 |
| Broadcom Inc. | 0001730168 | 18 | 3.86 |
| CHEVRON CORP | 0000093410 | 22 | 4.72 |
| CISCO SYSTEMS, INC. | 0000858877 | 11 | 2.36 |
| COCA COLA CO | 0000021344 | 13 | 2.79 |
| COSTCO WHOLESALE CORP /NEW | 0000909832 | 15 | 3.22 |
| ELI LILLY & Co | 0000059478 | 10 | 2.15 |
| ExxonMobil Holdings Corp | 0002115436 | 6 | 1.29 |
| JOHNSON & JOHNSON | 0000200406 | 11 | 2.36 |
| JPMORGAN CHASE & CO | 0000019617 | 34 | 7.30 |
| MICRON TECHNOLOGY INC | 0000723125 | 14 | 3.00 |
| MICROSOFT CORP | 0000789019 | 15 | 3.22 |
| Mastercard Inc | 0001141391 | 13 | 2.79 |
| Merck & Co., Inc. | 0000310158 | 11 | 2.36 |
| Meta Platforms, Inc. | 0001326801 | 15 | 3.22 |
| NVIDIA CORP | 0001045810 | 16 | 3.43 |
| ORACLE CORP | 0001341439 | 17 | 3.65 |
| PROCTER & GAMBLE Co | 0000080424 | 29 | 6.22 |
| Palantir Technologies Inc. | 0001321655 | 7 | 1.50 |
| SK hynix Inc. | 0002120882 | 0 | 0.00 |
| Tesla, Inc. | 0001318605 | 17 | 3.65 |
| UNITEDHEALTH GROUP INC | 0000731766 | 22 | 4.72 |
| VISA INC. | 0001403161 | 23 | 4.94 |
| Walmart Inc. | 0000104169 | 20 | 4.29 |

### Rows per item code

A row counts once under each of its item codes; a row with no items is counted as "no items". Shares are percent of the pull's row count, so shares can sum to more than 100.00.

| Item code | Rows | Share of rows (%) |
|---|---|---|
| 9.01 | 341 | 73.18 |
| 2.02 | 170 | 36.48 |
| 8.01 | 125 | 26.82 |
| 5.02 | 102 | 21.89 |
| 7.01 | 74 | 15.88 |
| 5.07 | 29 | 6.22 |
| 5.03 | 20 | 4.29 |
| 1.01 | 17 | 3.65 |
| 2.03 | 6 | 1.29 |
| 3.02 | 4 | 0.86 |
| 3.03 | 4 | 0.86 |
| 1.02 | 3 | 0.64 |
| 2.05 | 2 | 0.43 |
| 2.01 | 1 | 0.21 |
| 3.01 | 1 | 0.21 |
| 5.08 | 1 | 0.21 |

### Item x registrant table — 10 most frequent item codes

Codes ranked by row count descending, ties broken by code ascending. Columns are registrants by ticker (CIKs in the Registrants table above). Cell = rows of that registrant carrying that code.

| Item code | AMD | AMZN | ABBV | GOOGL | AAPL | BRK-B | AVGO | CVX | CSCO | KO | COST | LLY | XOM | JNJ | JPM | MU | MSFT | MA | MRK | META | NVDA | ORCL | PG | PLTR | TSLA | UNH | V | WMT | Total |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 9.01 | 14 | 16 | 19 | 16 | 8 | 11 | 12 | 12 | 7 | 11 | 13 | 8 | 2 | 10 | 28 | 14 | 11 | 10 | 9 | 11 | 7 | 15 | 26 | 6 | 16 | 6 | 12 | 11 | 341 |
| 2.02 | 6 | 6 | 12 | 6 | 6 | 6 | 5 | 7 | 5 | 6 | 5 | 6 | 2 | 6 | 6 | 5 | 6 | 6 | 6 | 6 | 5 | 5 | 6 | 6 | 12 | 6 | 6 | 5 | 170 |
| 8.01 | 0 | 7 | 4 | 11 | 1 | 3 | 13 | 5 | 0 | 1 | 7 | 2 | 2 | 2 | 12 | 2 | 2 | 2 | 3 | 5 | 2 | 9 | 5 | 0 | 0 | 1 | 16 | 8 | 125 |
| 5.02 | 8 | 1 | 2 | 5 | 6 | 3 | 3 | 7 | 5 | 5 | 4 | 1 | 0 | 2 | 3 | 4 | 5 | 3 | 1 | 3 | 6 | 6 | 5 | 0 | 2 | 5 | 1 | 6 | 102 |
| 7.01 | 9 | 3 | 3 | 1 | 0 | 0 | 0 | 3 | 0 | 0 | 0 | 0 | 4 | 2 | 9 | 1 | 2 | 0 | 0 | 0 | 1 | 4 | 14 | 6 | 1 | 8 | 2 | 1 | 74 |
| 5.07 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 2 | 1 | 2 | 1 | 1 | 1 | 1 | 1 | 29 |
| 5.03 | 0 | 0 | 0 | 1 | 0 | 2 | 0 | 2 | 1 | 0 | 0 | 0 | 0 | 0 | 4 | 2 | 1 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 1 | 3 | 1 | 20 |
| 1.01 | 4 | 2 | 0 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 2 | 1 | 2 | 0 | 0 | 2 | 0 | 1 | 0 | 17 |
| 2.03 | 2 | 1 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 6 |
| 3.02 | 3 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 4 |

### Registrants with an 8-K/A

- Apple Inc.: 1
- BERKSHIRE HATHAWAY INC: 1
- CHEVRON CORP: 1
- ORACLE CORP: 1
- UNITEDHEALTH GROUP INC: 1
- Walmart Inc.: 2

## Pull 2 — 8k-30-filers-pull2.csv

row count: 467
CSV SHA-256: 52791f46eaab79f3613a6e6b8d571477175a6d9f4e840bc35b4f1a9ec1592c2b
Pull date (UTC): 2026-11-12

### Rows per registrant

| Company | CIK | Rows | Share of rows (%) |
|---|---|---|---|
| ADVANCED MICRO DEVICES INC | 0000002488 | 19 | 4.07 |
| AMAZON COM INC | 0001018724 | 18 | 3.85 |
| ASML HOLDING NV | 0000937966 | 0 | 0.00 |
| AbbVie Inc. | 0001551152 | 22 | 4.71 |
| Alphabet Inc. | 0001652044 | 22 | 4.71 |
| Apple Inc. | 0000320193 | 14 | 3.00 |
| BERKSHIRE HATHAWAY INC | 0001067983 | 12 | 2.57 |
| Broadcom Inc. | 0001730168 | 18 | 3.85 |
| CHEVRON CORP | 0000093410 | 22 | 4.71 |
| CISCO SYSTEMS, INC. | 0000858877 | 11 | 2.36 |
| COCA COLA CO | 0000021344 | 13 | 2.78 |
| COSTCO WHOLESALE CORP /NEW | 0000909832 | 15 | 3.21 |
| ELI LILLY & Co | 0000059478 | 10 | 2.14 |
| ExxonMobil Holdings Corp | 0002115436 | 6 | 1.28 |
| JOHNSON & JOHNSON | 0000200406 | 11 | 2.36 |
| JPMORGAN CHASE & CO | 0000019617 | 34 | 7.28 |
| MICRON TECHNOLOGY INC | 0000723125 | 14 | 3.00 |
| MICROSOFT CORP | 0000789019 | 15 | 3.21 |
| Mastercard Inc | 0001141391 | 13 | 2.78 |
| Merck & Co., Inc. | 0000310158 | 11 | 2.36 |
| Meta Platforms, Inc. | 0001326801 | 15 | 3.21 |
| NVIDIA CORP | 0001045810 | 17 | 3.64 |
| ORACLE CORP | 0001341439 | 17 | 3.64 |
| PROCTER & GAMBLE Co | 0000080424 | 29 | 6.21 |
| Palantir Technologies Inc. | 0001321655 | 7 | 1.50 |
| SK hynix Inc. | 0002120882 | 0 | 0.00 |
| Tesla, Inc. | 0001318605 | 17 | 3.64 |
| UNITEDHEALTH GROUP INC | 0000731766 | 22 | 4.71 |
| VISA INC. | 0001403161 | 23 | 4.93 |
| Walmart Inc. | 0000104169 | 20 | 4.28 |

### Rows per item code

A row counts once under each of its item codes; a row with no items is counted as "no items". Shares are percent of the pull's row count, so shares can sum to more than 100.00.

| Item code | Rows | Share of rows (%) |
|---|---|---|
| 9.01 | 342 | 73.23 |
| 2.02 | 170 | 36.40 |
| 8.01 | 125 | 26.77 |
| 5.02 | 103 | 22.06 |
| 7.01 | 74 | 15.85 |
| 5.07 | 29 | 6.21 |
| 5.03 | 20 | 4.28 |
| 1.01 | 17 | 3.64 |
| 2.03 | 6 | 1.28 |
| 3.02 | 4 | 0.86 |
| 3.03 | 4 | 0.86 |
| 1.02 | 3 | 0.64 |
| 2.05 | 2 | 0.43 |
| 2.01 | 1 | 0.21 |
| 3.01 | 1 | 0.21 |
| 5.08 | 1 | 0.21 |

### Item x registrant table — 10 most frequent item codes

Codes ranked by row count descending, ties broken by code ascending. Columns are registrants by ticker (CIKs in the Registrants table above). Cell = rows of that registrant carrying that code.

| Item code | AMD | AMZN | ABBV | GOOGL | AAPL | BRK-B | AVGO | CVX | CSCO | KO | COST | LLY | XOM | JNJ | JPM | MU | MSFT | MA | MRK | META | NVDA | ORCL | PG | PLTR | TSLA | UNH | V | WMT | Total |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 9.01 | 14 | 16 | 19 | 16 | 8 | 11 | 12 | 12 | 7 | 11 | 13 | 8 | 2 | 10 | 28 | 14 | 11 | 10 | 9 | 11 | 8 | 15 | 26 | 6 | 16 | 6 | 12 | 11 | 342 |
| 2.02 | 6 | 6 | 12 | 6 | 6 | 6 | 5 | 7 | 5 | 6 | 5 | 6 | 2 | 6 | 6 | 5 | 6 | 6 | 6 | 6 | 5 | 5 | 6 | 6 | 12 | 6 | 6 | 5 | 170 |
| 8.01 | 0 | 7 | 4 | 11 | 1 | 3 | 13 | 5 | 0 | 1 | 7 | 2 | 2 | 2 | 12 | 2 | 2 | 2 | 3 | 5 | 2 | 9 | 5 | 0 | 0 | 1 | 16 | 8 | 125 |
| 5.02 | 8 | 1 | 2 | 5 | 6 | 3 | 3 | 7 | 5 | 5 | 4 | 1 | 0 | 2 | 3 | 4 | 5 | 3 | 1 | 3 | 7 | 6 | 5 | 0 | 2 | 5 | 1 | 6 | 103 |
| 7.01 | 9 | 3 | 3 | 1 | 0 | 0 | 0 | 3 | 0 | 0 | 0 | 0 | 4 | 2 | 9 | 1 | 2 | 0 | 0 | 0 | 1 | 4 | 14 | 6 | 1 | 8 | 2 | 1 | 74 |
| 5.07 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 2 | 1 | 2 | 1 | 1 | 1 | 1 | 1 | 29 |
| 5.03 | 0 | 0 | 0 | 1 | 0 | 2 | 0 | 2 | 1 | 0 | 0 | 0 | 0 | 0 | 4 | 2 | 1 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 1 | 3 | 1 | 20 |
| 1.01 | 4 | 2 | 0 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 2 | 1 | 2 | 0 | 0 | 2 | 0 | 1 | 0 | 17 |
| 2.03 | 2 | 1 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 6 |
| 3.02 | 3 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 4 |

### Registrants with an 8-K/A

- Apple Inc.: 1
- BERKSHIRE HATHAWAY INC: 1
- CHEVRON CORP: 1
- ORACLE CORP: 1
- UNITEDHEALTH GROUP INC: 1
- Walmart Inc.: 2

## Pull 3 — 8k-30-filers-pull3.csv

row count: 469
CSV SHA-256: 8c9ce3ac56b81b1de5db61a80b763583b9dc94b8f02ab1eb977f771df3a1d3ca
Pull date (UTC): 2026-11-13

### Rows per registrant

| Company | CIK | Rows | Share of rows (%) |
|---|---|---|---|
| ADVANCED MICRO DEVICES INC | 0000002488 | 19 | 4.05 |
| AMAZON COM INC | 0001018724 | 18 | 3.84 |
| ASML HOLDING NV | 0000937966 | 0 | 0.00 |
| AbbVie Inc. | 0001551152 | 22 | 4.69 |
| Alphabet Inc. | 0001652044 | 22 | 4.69 |
| Apple Inc. | 0000320193 | 14 | 2.99 |
| BERKSHIRE HATHAWAY INC | 0001067983 | 12 | 2.56 |
| Broadcom Inc. | 0001730168 | 18 | 3.84 |
| CHEVRON CORP | 0000093410 | 22 | 4.69 |
| CISCO SYSTEMS, INC. | 0000858877 | 12 | 2.56 |
| COCA COLA CO | 0000021344 | 13 | 2.77 |
| COSTCO WHOLESALE CORP /NEW | 0000909832 | 15 | 3.20 |
| ELI LILLY & Co | 0000059478 | 10 | 2.13 |
| ExxonMobil Holdings Corp | 0002115436 | 6 | 1.28 |
| JOHNSON & JOHNSON | 0000200406 | 11 | 2.35 |
| JPMORGAN CHASE & CO | 0000019617 | 34 | 7.25 |
| MICRON TECHNOLOGY INC | 0000723125 | 14 | 2.99 |
| MICROSOFT CORP | 0000789019 | 15 | 3.20 |
| Mastercard Inc | 0001141391 | 13 | 2.77 |
| Merck & Co., Inc. | 0000310158 | 11 | 2.35 |
| Meta Platforms, Inc. | 0001326801 | 16 | 3.41 |
| NVIDIA CORP | 0001045810 | 17 | 3.62 |
| ORACLE CORP | 0001341439 | 17 | 3.62 |
| PROCTER & GAMBLE Co | 0000080424 | 29 | 6.18 |
| Palantir Technologies Inc. | 0001321655 | 7 | 1.49 |
| SK hynix Inc. | 0002120882 | 0 | 0.00 |
| Tesla, Inc. | 0001318605 | 17 | 3.62 |
| UNITEDHEALTH GROUP INC | 0000731766 | 22 | 4.69 |
| VISA INC. | 0001403161 | 23 | 4.90 |
| Walmart Inc. | 0000104169 | 20 | 4.26 |

### Rows per item code

A row counts once under each of its item codes; a row with no items is counted as "no items". Shares are percent of the pull's row count, so shares can sum to more than 100.00.

| Item code | Rows | Share of rows (%) |
|---|---|---|
| 9.01 | 344 | 73.35 |
| 2.02 | 171 | 36.46 |
| 8.01 | 126 | 26.87 |
| 5.02 | 103 | 21.96 |
| 7.01 | 74 | 15.78 |
| 5.07 | 29 | 6.18 |
| 5.03 | 20 | 4.26 |
| 1.01 | 17 | 3.62 |
| 2.03 | 6 | 1.28 |
| 3.02 | 4 | 0.85 |
| 3.03 | 4 | 0.85 |
| 1.02 | 3 | 0.64 |
| 2.05 | 2 | 0.43 |
| 2.01 | 1 | 0.21 |
| 3.01 | 1 | 0.21 |
| 5.08 | 1 | 0.21 |

### Item x registrant table — 10 most frequent item codes

Codes ranked by row count descending, ties broken by code ascending. Columns are registrants by ticker (CIKs in the Registrants table above). Cell = rows of that registrant carrying that code.

| Item code | AMD | AMZN | ABBV | GOOGL | AAPL | BRK-B | AVGO | CVX | CSCO | KO | COST | LLY | XOM | JNJ | JPM | MU | MSFT | MA | MRK | META | NVDA | ORCL | PG | PLTR | TSLA | UNH | V | WMT | Total |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 9.01 | 14 | 16 | 19 | 16 | 8 | 11 | 12 | 12 | 8 | 11 | 13 | 8 | 2 | 10 | 28 | 14 | 11 | 10 | 9 | 12 | 8 | 15 | 26 | 6 | 16 | 6 | 12 | 11 | 344 |
| 2.02 | 6 | 6 | 12 | 6 | 6 | 6 | 5 | 7 | 6 | 6 | 5 | 6 | 2 | 6 | 6 | 5 | 6 | 6 | 6 | 6 | 5 | 5 | 6 | 6 | 12 | 6 | 6 | 5 | 171 |
| 8.01 | 0 | 7 | 4 | 11 | 1 | 3 | 13 | 5 | 0 | 1 | 7 | 2 | 2 | 2 | 12 | 2 | 2 | 2 | 3 | 6 | 2 | 9 | 5 | 0 | 0 | 1 | 16 | 8 | 126 |
| 5.02 | 8 | 1 | 2 | 5 | 6 | 3 | 3 | 7 | 5 | 5 | 4 | 1 | 0 | 2 | 3 | 4 | 5 | 3 | 1 | 3 | 7 | 6 | 5 | 0 | 2 | 5 | 1 | 6 | 103 |
| 7.01 | 9 | 3 | 3 | 1 | 0 | 0 | 0 | 3 | 0 | 0 | 0 | 0 | 4 | 2 | 9 | 1 | 2 | 0 | 0 | 0 | 1 | 4 | 14 | 6 | 1 | 8 | 2 | 1 | 74 |
| 5.07 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 2 | 1 | 2 | 1 | 1 | 1 | 1 | 1 | 29 |
| 5.03 | 0 | 0 | 0 | 1 | 0 | 2 | 0 | 2 | 1 | 0 | 0 | 0 | 0 | 0 | 4 | 2 | 1 | 0 | 0 | 1 | 0 | 1 | 0 | 0 | 0 | 1 | 3 | 1 | 20 |
| 1.01 | 4 | 2 | 0 | 2 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 2 | 1 | 2 | 0 | 0 | 2 | 0 | 1 | 0 | 17 |
| 2.03 | 2 | 1 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 1 | 0 | 0 | 0 | 6 |
| 3.02 | 3 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 0 | 4 |

### Registrants with an 8-K/A

- Apple Inc.: 1
- BERKSHIRE HATHAWAY INC: 1
- CHEVRON CORP: 1
- ORACLE CORP: 1
- UNITEDHEALTH GROUP INC: 1
- Walmart Inc.: 2

## Review — 40 filings read (from pull 1)

qualifying_count: 161
review_count: 40

The 40 most recent pull-1 rows by acceptanceDateTime whose items include a code other than 2.02, 7.01, 8.01 and 9.01. Document path is the path of the document whose Type is the form, taken from the filing's index page. Per item, one line read from the sentence(s) under its heading: for 1.01 the counterparty and amount if stated, for 5.02 the role and effective date if stated, else the main fact.

| # | Company | CIK | Accession | Document path | Item | One line |
|---|---|---|---|---|---|---|
| 1 | COSTCO WHOLESALE CORP /NEW | 0000909832 | 0000909832-26-000134 | /Archives/edgar/data/909832/000090983226000134/cost-20261107.htm | 5.02 | On November 7, 2026, Helena B. Foulkes notified the Board of Directors (the “Board”) of Costco Wholesale Corporation (the “Company”) of her decision to resign from the Board and all committees of the Board of which she is a member, effective November 7, 2026. |
| 1 | COSTCO WHOLESALE CORP /NEW | 0000909832 | 0000909832-26-000134 | /Archives/edgar/data/909832/000090983226000134/cost-20261107.htm | 8.01 | On November 10, 2026, the Board of Directors declared a special cash dividend on the Company's common stock of $30 per share, payable December 4, 2026, to shareholders of record at the close of business on November 24, 2026. |
| 1 | COSTCO WHOLESALE CORP /NEW | 0000909832 | 0000909832-26-000134 | /Archives/edgar/data/909832/000090983226000134/cost-20261107.htm | 9.01 | (d) Exhibits. 99.1. Press release dated November 10, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). |
| 2 | UNITEDHEALTH GROUP INC | 0000731766 | 0000731766-26-000274 | /Archives/edgar/data/731766/000073176626000274/unh-20261103.htm | 5.02 | Madeline Bell as independent director On November 9, 2026, UnitedHealth Group Incorporated (the “Company”) issued a press release announcing the appointment of Madeline Bell to serve as an independent director of the Company, effective November 3, 2026. |
| 2 | UNITEDHEALTH GROUP INC | 0000731766 | 0000731766-26-000274 | /Archives/edgar/data/731766/000073176626000274/unh-20261103.htm | 9.01 | Exhibit Description 99.1 Press release dated November 9, 2026 104 Cover Page Interactive Data File (formatted as Inline XBRL). |
| 3 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-123389 | /Archives/edgar/data/723125/000110465926123389/tm2629062d1_8k.htm | 5.02 | On November 2, 2026, Linnie M. Haynesworth notified the Governance and Sustainability Committee of the Board of Directors (the “Board”) of Micron Technology, Inc. (the “Company”) that she would retire from the Board and, accordingly, Ms. Haynesworth will not be nominated for re-election at the Company’s fiscal 2026 annual shareholders meeting (the “Annual Meeting”). Ms. Haynesworth will continue to serve as a director through the end of her term at the Annual Meeting. |
| 3 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-123389 | /Archives/edgar/data/723125/000110465926123389/tm2629062d1_8k.htm | 9.01 | (d) Exhibits. Exhibit No. Description 99.1 Press Release issued on November 5, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 4 | MICROSOFT CORP | 0000789019 | 0001193125-26-448357 | /Archives/edgar/data/789019/000119312526448357/d177209d8k.htm | 5.02 | (b) On November 4, 2026, Emma N. Walmsley, a member of the Board of Directors of Microsoft Corporation (the “Company”) since 2019, informed the Company of her decision not to stand for re-election at the Company’s 2026 annual shareholder meeting (the “Annual Meeting”). Ms. Walmsley will continue to serve as a director until the Annual Meeting. Her decision not to stand for re-election is not as a result of any disagreement with management on any matter relating to the Company’s operations, policies, or practices. |
| 5 | AbbVie Inc. | 0001551152 | 0001104659-26-121322 | /Archives/edgar/data/1551152/000110465926121322/tm2628215d1_8k.htm | 5.02 | On October 28, 2026, Jennifer L. Davis, a Class II director of AbbVie Inc. (“AbbVie”), notified the Company’s Board of Directors (the “Board”), of her intent to resign from the Board, effective November 2, 2026, in light of her recent appointment as Chief Executive Officer at Align Technology, Inc. Her resignation as a director is not the result of any dispute or disagreement with AbbVie on any matter relating to the operations, policies or practices of AbbVie. |
| 6 | Meta Platforms, Inc. | 0001326801 | 0001193125-26-438017 | /Archives/edgar/data/1326801/000119312526438017/d183592d8k.htm | 1.01 | Mandatory Convertible Preferred Stock Offering On October 26, 2026, Meta Platforms, Inc. (the “Company”) entered into an underwriting agreement (the “Underwriting Agreement (Depositary Shares)”) with Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC as the representatives of the several underwriters named therein (the “Depositary Shares Underwriters”), pursuant to which the Company agreed to issue and sell 250,000,000 Series A depositary shares (the “Depositary Shares”), each representing a 1/20th interest in a share of 6.50% Series A Mandatory Convertible Preferred Stock, liquidation preference $1,000.00 per share, par value $0.000006 per share (the “Preferred Stock” and such offering, the “Depositary Shares Offering”). |
| 6 | Meta Platforms, Inc. | 0001326801 | 0001193125-26-438017 | /Archives/edgar/data/1326801/000119312526438017/d183592d8k.htm | 3.03 | On October 28, 2026, the Company filed the Certificates of Designations with the Secretary of State of the State of Delaware to establish the preferences, limitations, and relative rights of the Preferred Stock. |
| 6 | Meta Platforms, Inc. | 0001326801 | 0001193125-26-438017 | /Archives/edgar/data/1326801/000119312526438017/d183592d8k.htm | 5.03 | The information set forth under Item 3.03 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 5.03. Forward Looking Statements This Current Report on Form 8-K contains forward-looking statements within the meaning of the Private Securities Litigation Reform Act of 1995 (the “PSLRA”). |
| 6 | Meta Platforms, Inc. | 0001326801 | 0001193125-26-438017 | /Archives/edgar/data/1326801/000119312526438017/d183592d8k.htm | 9.01 | (d) Exhibits 1.1 Underwriting Agreement, dated as of October 26, 2026, by and among Meta Platforms, Inc. and Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as representatives of the several underwriters named therein, relating to the Depositary Shares. 1.2 Underwriting Agreement, dated as of October 26, 2026, by and among Meta Platforms, Inc., Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as representatives of the several underwriters named therein, Morgan Stanley Capital Services LLC and Goldman Sachs & Co. LLC, as forward purchasers, and Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as forward sellers, relating to the Class A Common Stock. 3.1 Original Certificate of Designations for the 6.50% Series A Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective October 28, 2026. 4.1 Form of Certificate for the 6.50% Series A Mandatory Convertible Preferred Stock (included as Exhibit A to Exhibit 3.1). 4.2 Deposit Agreement, dated as of October 29, 2026, by and among Meta Platforms, Inc., Computershare Trust Company, N.A., and Computershare Inc., acting jointly as bank depositary, and the holders from time to time of the Depositary Receipts described therein. 4.3 Form of Depositary Receipt for the Depositary Shares (included as Exhibit A to Exhibit 4.2). 5.1 Opinion of Davis Polk & Wardwell LLP relating to the Depositary Shares and the Preferred Stock. 5.2 Opinion of Davis Polk & Wardwell LLP relating to the Class A Common Stock. |
| 7 | Broadcom Inc. | 0001730168 | 0001193125-26-434271 | /Archives/edgar/data/1730168/000119312526434271/d148323d8k.htm | 2.03 | On October 26, 2026, Broadcom Inc. (the “Company”) arranged for financial partners to take on a portion of certain agreements to purchase AI racks based on custom AI accelerators designed by the Company and the related lease agreements with the Company’s customer that enable the deployment of compute capacity. |
| 8 | Meta Platforms, Inc. | 0001326801 | 0001628280-26-066700 | /Archives/edgar/data/1326801/000162828026066700/meta-20261019.htm | 1.01 | On October 19, 2026, the board of directors (the “Board”) of Meta Platforms, Inc. (the “Company” or “Meta”) approved and declared advisable, based on the unanimous recommendation of a special committee consisting of disinterested and independent directors established to review such transaction, and recommended to the Company’s shareholders, the amendment and restatement of the Company’s certificate of incorporation (as so amended and restated, the “Restated Charter”) to, among other things, adjust the Company’s capital structure by establishing a new class of non-voting Class C common stock, par value $0.000006 (the “Recapitalization”), which was subsequently approved by the requisite shareholders by written consent on October 20, 2026. |
| 8 | Meta Platforms, Inc. | 0001326801 | 0001628280-26-066700 | /Archives/edgar/data/1326801/000162828026066700/meta-20261019.htm | 2.02 | On October 21, 2026, the Company issued a press release and will hold a conference call regarding its financial results for the quarter ended September 30, 2026. |
| 8 | Meta Platforms, Inc. | 0001326801 | 0001628280-26-066700 | /Archives/edgar/data/1326801/000162828026066700/meta-20261019.htm | 8.01 | As described above, also on October 19, 2026, the Board declared the Stock Dividend, contingent upon the effectiveness of the Restated Charter, with the record date and payment date for the Stock Dividend to be established by the Board by subsequent action. |
| 8 | Meta Platforms, Inc. | 0001326801 | 0001628280-26-066700 | /Archives/edgar/data/1326801/000162828026066700/meta-20261019.htm | 9.01 | (d) Exhibits Exhibit Number Exhibit Title or Description 10.1 Founder Alignment Agreement, dated October 20, 2026, by and between Mark Zuckerberg and Meta Platforms, Inc. 99.1 Press release dated October 21, 2026 104 Cover Page Interactive Data File (the cover page XBRL tags are embedded within the inline XBRL document) |
| 9 | COSTCO WHOLESALE CORP /NEW | 0000909832 | 0000909832-26-000100 | /Archives/edgar/data/909832/000090983226000100/cost-20261013.htm | 5.02 | On October 13, 2026, the Compensation Committee of the Board of Directors approved the fiscal 2027 criteria for bonuses to executive officers, with the Nominating and Governance Committee of the Board also approving the environmental and social performance criteria. Executive officers other than the Chief Executive Officer are eligible to receive base bonuses of $400,000. The base amounts include $160,000 based on targets relating to sales and $160,000 based on targets relating to pre-tax income. |
| 9 | COSTCO WHOLESALE CORP /NEW | 0000909832 | 0000909832-26-000100 | /Archives/edgar/data/909832/000090983226000100/cost-20261013.htm | 9.01 | (d) Exhibits. 10.1. Fiscal 2027 Executive Bonus Plan. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). |
| 10 | PROCTER & GAMBLE Co | 0000080424 | 0000080424-26-000245 | /Archives/edgar/data/80424/000008042426000245/pg-20261016.htm | 5.07 | On October 13, 2026, the Company held its 2026 Annual Meeting of Shareholders. |
| 11 | AbbVie Inc. | 0001551152 | 0001104659-26-116227 | /Archives/edgar/data/1551152/000110465926116227/tm2627361d1_8k.htm | 5.02 | On October 14, 2026, AbbVie Inc. (“AbbVie”) expanded the size of its Board of Directors (the “Board”) from twelve directors to thirteen directors and appointed Dr. John M. Carethers as a Class II director. Dr. Carethers currently serves as the Vice Chancellor for Health Sciences at the University of California San Diego and was previously a director of Avantor, Inc. Dr. Carethers has been appointed to the Public Policy and Sustainability Committee of AbbVie. The Board affirmatively determined that Dr. Carethers is an “independent director” under each of the standards set forth in section 303A.02 of the New York Stock Exchange Listed Company Manual and AbbVie’s Governance Guidelines and Director Independence Guidelines. |
| 12 | Merck & Co., Inc. | 0000310158 | 0000310158-26-000237 | /Archives/edgar/data/310158/000031015826000237/mrk-20261009.htm | 5.02 | (d) Incorporated by reference is a press release issued by Merck & Co., Inc. (the “Company”) on October 13, 2026, attached as Exhibit 99.1, announcing the election of Paul J. Diaz to the Company’s Board of Directors (the “Board”), effective November 1, 2026. |
| 12 | Merck & Co., Inc. | 0000310158 | 0000310158-26-000237 | /Archives/edgar/data/310158/000031015826000237/mrk-20261009.htm | 9.01 | (d) Exhibits Exhibit 99.1 Press release issued October 13, 2026 Exhibit 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 13 | CISCO SYSTEMS, INC. | 0000858877 | 0000858877-26-000156 | /Archives/edgar/data/858877/000085887726000156/csco-20261007.htm | 5.02 | Director On October 7, 2026, the Board of Directors (“Board”) of Cisco Systems, Inc. (“Cisco”) appointed Girish D. Rishi, CEO of Cognite Holding B.V., as a member of the Board effective October 9, 2026. |
| 14 | CHEVRON CORP | 0000093410 | 0000093410-26-000188 | /Archives/edgar/data/93410/000009341026000188/cvx-20260930.htm | 5.02 | (b) On September 30, 2026, the Board of Directors (the “Board”) of Chevron Corporation (”Chevron”) approved certain officer elections. Mark A. Nelson, currently Chevron’s Vice Chairman and Executive Vice President of Oil, Products & Gas, will remain Vice Chairman with responsibility for Strategy and Business Development in addition to his corporate duties, and will no longer serve as Executive Vice President, Oil, Products & Gas, in each case, effective January 1, 2027. |
| 15 | Tesla, Inc. | 0001318605 | 0001628280-26-063820 | /Archives/edgar/data/1318605/000162828026063820/tsla-20260929.htm | 1.02 | Revolving Credit Facility As previously reported, Tesla is a party to that certain Credit Agreement, dated as of January 20, 2023 (as further amended from time to time, the “Existing Revolving Credit Agreement”), with Citi, as administrative agent and the lenders and other agents party thereto. |
| 15 | Tesla, Inc. | 0001318605 | 0001628280-26-063820 | /Archives/edgar/data/1318605/000162828026063820/tsla-20260929.htm | 2.03 | The information set forth in Item 1.01 above is incorporated herein by reference. |
| 15 | Tesla, Inc. | 0001318605 | 0001628280-26-063820 | /Archives/edgar/data/1318605/000162828026063820/tsla-20260929.htm | 1.01 | On September 29, 2026, Tesla, Inc. (“Tesla”) entered into the following credit agreements: •$20.0 billion senior unsecured three-year delayed draw term loan facility (the “Term Loan Facility”) pursuant to a Delayed Draw Term Loan Credit Agreement, dated as of September 29, 2026 (the “DDTL Credit Agreement”), by and among Tesla, as borrower, Citibank, N.A. (“Citi”), as administrative agent, and the lenders and other agents party thereto. •$8.0 billion senior unsecured five-year revolving facility (the “Five-Year Revolving Facility”) pursuant to a Five-Year Revolving Credit Agreement, dated as of September 29, 2026 (the “Five-Year Revolving Credit Agreement”), by and among Tesla, as borrower, Wells Fargo Bank, National Association (“WF Bank”), as administrative agent, and the lenders, issuing banks and other agents party thereto. •$2.0 billion senior unsecured 364-day revolving credit facility (the “364-Day Revolving Facility”) pursuant to a 364-Day Revolving Credit Agreement, dated as of September 29, 2026 (the “364-Day Revolving Credit Agreement”), by and among Tesla, as borrower, WF Bank, as administrative agent, and the lenders and other agents party thereto. |
| 15 | Tesla, Inc. | 0001318605 | 0001628280-26-063820 | /Archives/edgar/data/1318605/000162828026063820/tsla-20260929.htm | 9.01 | (d)Exhibits. Exhibit No. Description 104 Cover Page Interactive Data File (embedded within the Inline XBRL document). |
| 16 | ADVANCED MICRO DEVICES INC | 0000002488 | 0000002488-26-000182 | /Archives/edgar/data/2488/000000248826000182/amd-20260926.htm | 3.02 | On September 26, 2026, Advanced Micro Devices, Inc. (the “Company”) entered into an Agreement and Plan of Merger (the “Merger Agreement”) to acquire all of the equity interests in World Labs Technologies, Inc. (“World Labs”) (the “Acquisition”) for a total purchase price of approximately $8.2 billion to be paid in shares of the Company’s common stock, par value $0.01 per share (“Common Stock”), to stockholders of World Labs, subject to customary adjustments. |
| 17 | AMAZON COM INC | 0001018724 | 0001018724-26-000036 | /Archives/edgar/data/1018724/000101872426000036/amzn-20260908.htm | 5.02 | On September 8, 2026, the Board of Directors of Amazon.com, Inc. (the “Company”) elected Kevin R. Mandia as a director of the Company and also appointed him to the Audit Committee and Security Committee of the Board. Mr. Mandia has served as Chief Executive Officer of Armadin, Inc., a cybersecurity company he founded, since September 2025. Mr. Mandia has also served as General Partner of Ballistic Ventures, a venture capital firm he co-founded, since June 2024 and previously served as Strategic Partner from December 2021 to June 2024. |
| 18 | Apple Inc. | 0000320193 | 0001140361-26-035325 | /Archives/edgar/data/320193/000114036126035325/ef20081427_8ka.htm | 5.02 | Apple Inc. (“Apple”) previously announced its Chief Executive Officer transition plan in its Current Report on Form 8-K filed on April 20, 2026 (the “Original Form 8-K”). This Amendment to the Original Form 8-K (the “Form 8-K/A”) is being filed to disclose John Ternus’ new compensation arrangement in connection with his appointment to the role of CEO, and Tim Cook’s new compensation arrangement in connection with his appointment to the role of Executive Chair of Apple’s Board of Directors (the “Board”), in each case effective as of September 1, 2026 (the “Transition Date”). |
| 19 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-101067 | /Archives/edgar/data/723125/000110465926101067/tm2624017d1_8k.htm | 5.02 | On August 26, 2026, Micron Technology, Inc. ("Micron" or the “Company”) announced that Manish Bhatia, 54, the Company’s current Executive Vice President, Global Operations, has been appointed as President and Chief Operating Officer of the Company and that Dr. Scott DeBoer, 60, the Company’s current Executive Vice President, Chief Technology and Products Officer, has been appointed President and Chief Technology and Products Officer of the Company, effective immediately. |
| 19 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-101067 | /Archives/edgar/data/723125/000110465926101067/tm2624017d1_8k.htm | 9.01 | (d) Exhibits. Exhibit No. Description 99.1 Press Release dated August 26, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 20 | ADVANCED MICRO DEVICES INC | 0000002488 | 0000002488-26-000163 | /Archives/edgar/data/2488/000000248826000163/amd-20260817.htm | 5.02 | Director Retirement On August 17, 2026, Mr. Joe Householder provided Advanced Micro Devices, Inc. (the “Company”) with notice of his intention to retire from the Company’s Board of Directors (the “Board”) effective as of August 19, 2026. |
| 20 | ADVANCED MICRO DEVICES INC | 0000002488 | 0000002488-26-000163 | /Archives/edgar/data/2488/000000248826000163/amd-20260817.htm | 9.01 | (d) Exhibits Exhibit No. Description 99.1 Press Release dated August 19, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 21 | ADVANCED MICRO DEVICES INC | 0000002488 | 0001193125-26-354029 | /Archives/edgar/data/2488/000119312526354029/d142696d8k.htm | 2.03 | The information set forth under “Item 1.01. Entry into a Material Definitive Agreement” is incorporated herein by reference. |
| 21 | ADVANCED MICRO DEVICES INC | 0000002488 | 0001193125-26-354029 | /Archives/edgar/data/2488/000119312526354029/d142696d8k.htm | 1.01 | On August 17, 2026 (the “Closing Date”), Advanced Micro Devices, Inc. (the “Company”) closed its public offering (the “Offering”) of $4.75 billion aggregate principal amount of senior notes, consisting of $1.25 billion aggregate principal amount of its 4.600% Senior Notes due 2029 (the “2029 Notes”), $1.50 billion aggregate principal amount of its 5.000% Senior Notes due 2031 (the “2031 Notes”), $1.00 billion aggregate principal amount of its 5.250% Senior Notes due 2033 (the “2033 Notes”) and $1.00 billion aggregate principal amount of its 5.500% Senior Notes due 2036 (the “2036 Notes,” and together with the 2029 Notes, the 2031 Notes and the 2033 Notes, the “Notes”). |
| 21 | ADVANCED MICRO DEVICES INC | 0000002488 | 0001193125-26-354029 | /Archives/edgar/data/2488/000119312526354029/d142696d8k.htm | 9.01 | (d) Exhibits Exhibit Number Description 1.1 Underwriting Agreement, dated as of August 13, 2026, by and among Advanced Micro Devices, Inc. and Barclays Capital Inc., BofA Securities, Inc., Citigroup Global Markets Inc., J.P. Morgan Securities LLC, Morgan Stanley & Co. LLC and Wells Fargo Securities, LLC, as representatives of the several underwriters named therein 4.1 Third Supplemental Indenture, dated as of August 17, 2026, by and between the Company and U.S. Bank Trust Company, National Association, as trustee 4.2 Form of 2029 Note (included in Exhibit 4.1) 4.3 Form of 2031 Note (included in Exhibit 4.1) 4.4 Form of 2033 Note (included in Exhibit 4.1) 4.5 Form of 2036 Note (included in Exhibit 4.1) 5.1 Opinion of Latham & Watkins LLP |
| 22 | NVIDIA CORP | 0001045810 | 0001045810-26-000069 | /Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm | 1.01 | On August 17, 2026, NVIDIA Corporation (“NVIDIA”) announced a multi-year partnership with SB Energy Corp. (collectively with its affiliates, “SB Energy”) to advance the development of the PORTS Technology Campus, a large-scale AI data center campus in Pike County, Ohio (the “Portsmouth Site”). Through the partnership and the credit support described below, NVIDIA has secured land, power, and shell capacity at the Portsmouth Site to host NVIDIA AI compute infrastructure. An affiliate of OpenAI Group PBC (such affiliate, “OpenAI”) will be the tenant. |
| 22 | NVIDIA CORP | 0001045810 | 0001045810-26-000069 | /Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm | 2.03 | The information set forth in Item 1.01 above is hereby incorporated by reference into this Item 2.03. |
| 22 | NVIDIA CORP | 0001045810 | 0001045810-26-000069 | /Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm | 7.01 | On August 17, 2026, NVIDIA issued a press release announcing the partnership with SB Energy. |
| 22 | NVIDIA CORP | 0001045810 | 0001045810-26-000069 | /Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm | 9.01 | (d) Exhibits Exhibit Description 99.1 Press release, issued August 17, 2026 104 The cover page of this Current Report on Form 8-K, formatted in inline XBRL (included as Exhibit 101) |
| 23 | JOHNSON & JOHNSON | 0000200406 | 0000200406-26-000167 | /Archives/edgar/data/200406/000020040626000167/jnj-20260804.htm | 5.02 | On August 4, 2026, the Company announced that Jennifer Taubert will retire from her position as Executive Vice President, Worldwide Chairman, Innovative Medicine and member of the Executive Committee effective September 1, 2026. |
| 23 | JOHNSON & JOHNSON | 0000200406 | 0000200406-26-000167 | /Archives/edgar/data/200406/000020040626000167/jnj-20260804.htm | 9.01 | (d) Exhibits. Exhibit No. Description of Exhibit 99.1 Press Release dated August 4, 2026. |
| 24 | PROCTER & GAMBLE Co | 0000080424 | 0000080424-26-000094 | /Archives/edgar/data/80424/000008042426000094/pg-20260729.htm | 5.02 | On July 29, 2026, The Procter & Gamble Company (the "Company") announced that Jon R. Moeller, Executive Chairman of the Board, will retire from his position as Executive Chairman and as a member of the Board of Directors (“the Board”), effective July 31, 2026. |
| 24 | PROCTER & GAMBLE Co | 0000080424 | 0000080424-26-000094 | /Archives/edgar/data/80424/000008042426000094/pg-20260729.htm | 7.01 | The Company issued a news release on July 29, 2026, announcing Mr. Moeller’s retirement and Mr. Jejurikar’s appointment. |
| 24 | PROCTER & GAMBLE Co | 0000080424 | 0000080424-26-000094 | /Archives/edgar/data/80424/000008042426000094/pg-20260729.htm | 9.01 | Exhibit No. Description 99.1 Dividend News Release by The Procter & Gamble Company dated July 29, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 25 | JPMORGAN CHASE & CO | 0000019617 | 0000019617-26-000288 | /Archives/edgar/data/19617/000001961726000288/jpm-20260721.htm | 5.03 | The Board of Directors (the “Board”) of JPMorgan Chase & Co. (the “Corporation”) has adopted an amendment to Section 2.03 of the Corporation’s By-laws, effective July 21, 2026 (as so amended, the "By-laws"), to provide that a Lead Independent Director, if any, shall be appointed by the non-management directors. |
| 25 | JPMORGAN CHASE & CO | 0000019617 | 0000019617-26-000288 | /Archives/edgar/data/19617/000001961726000288/jpm-20260721.htm | 9.01 | (d) Exhibit Exhibit No. Description of Exhibit 3.2 By-laws of JPMorgan Chase & Co., as amended, effective July 21, 2026 101 Pursuant to Rule 406 of Regulation S-T, the cover page is formatted in Inline XBRL (Inline eXtensible Business Reporting Language). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document and included in Exhibit 101). |
| 26 | VISA INC. | 0001403161 | 0001403161-26-000096 | /Archives/edgar/data/1403161/000140316126000096/v-20260714.htm | 5.03 | The Board of Directors of Visa Inc. (the “Company”) amended the Company’s Amended and Restated Bylaws (as amended, the “Bylaws”), effective July 14, 2026. |
| 26 | VISA INC. | 0001403161 | 0001403161-26-000096 | /Archives/edgar/data/1403161/000140316126000096/v-20260714.htm | 9.01 | (d) Exhibits Exhibit Number Description 3.2 Amended and Restated Bylaws of Visa Inc. 104 Cover Page Interactive Data File (formatted as Inline XBRL) |
| 27 | NVIDIA CORP | 0001045810 | 0001045810-26-000060 | /Archives/edgar/data/1045810/000104581026000060/nvda-20260628.htm | 5.02 | (b) On June 28, 2026, Ajay K. Puri, Executive Vice President, Worldwide Field Operations of NVIDIA Corporation, or the Company, notified the Company of his intention to retire from his role effective upon the employment commencement date of his successor. |
| 28 | ADVANCED MICRO DEVICES INC | 0000002488 | 0000002488-26-000115 | /Archives/edgar/data/2488/000000248826000115/amd-20260626.htm | 5.02 | On June 26, 2026, the Board of Directors (the “Board”) of Advanced Micro Devices, Inc. (the “Company”) and the Compensation and Leadership Resources Committee of the Board (the “Committee”), as applicable, approved the following changes to the compensation of certain members of the Company’s executive team: Base Salary Increases Effective July 1, 2026, the annual base salaries for the below-listed members of the Company’s executive team will increase as follows: Name and Title Annual Base Salary as of June 30, 2026 Annual Base Salary Effective July 1, 2026 Lisa T. Su, Chair, President and Chief Executive Officer $1,323,000 $1,375,000 Jean Hu, Executive Vice President, Chief Financial Officer and Treasurer $800,000 $850,000 Mark Papermaster, Executive Vice President and Chief Technology Officer $870,000 $900,000 Darren Grasby, Executive Vice President, Chief Sales Officer and President EMEA $810,902 $843,866 Forrest Norrod, Executive Vice President and General Manager, Data Center Solutions $780,000 $800,000 _______________ (1) Amounts shown for Mr. Grasby were converted to U.S. dollars from £615,000 and £640,000, respectively, using an exchange rate of $1.31854 U.S. dollars per 1.00 British pound, which was the exchange rate reported by Bloomberg Financial as of June 26, 2026. |
| 29 | NVIDIA CORP | 0001045810 | 0001045810-26-000056 | /Archives/edgar/data/1045810/000104581026000056/nvda-20260624.htm | 5.07 | On June 24, 2026, at the 2026 Annual Meeting of Stockholders of NVIDIA Corporation, or the 2026 Annual Meeting, the following proposals were adopted or rejected by the margin indicated. |
| 30 | COCA COLA CO | 0000021344 | 0001552781-26-000366 | /Archives/edgar/data/21344/000155278126000366/e26287_ko-8k.htm | 5.02 | On June 25, 2026, The Coca-Cola Company (the “Company”) announced that Jennifer Mann, Executive Vice President and President, North America Operating Unit, will be departing the Company. Effective July 31, 2026, Ms. Mann will step down from her current positions. |
| 30 | COCA COLA CO | 0000021344 | 0001552781-26-000366 | /Archives/edgar/data/21344/000155278126000366/e26287_ko-8k.htm | 9.01 | EXHIBIT INDEX Exhibit No. Description Exhibit 10.1 Separation Agreement and Full and Complete Release and Agreement on Trade Secrets and Confidentiality between The Coca-Cola Company and Jennifer Mann, dated June 25, 2026. Exhibit 99.1 Press Release of The Coca-Cola Company, dated June 25, 2026. Exhibit 104 Cover Page Interactive Data File (the cover page XBRL tags are embedded within the iXBRL document). |
| 31 | JPMORGAN CHASE & CO | 0000019617 | 0000019617-26-000241 | /Archives/edgar/data/19617/000001961726000241/jpm-20260624.htm | 5.02 | On June 25, 2026, JPMorgan Chase & Co. ("JPMorganChase" or the “Firm”) announced that Doug Petno, 61, and Troy Rohrbaugh, 56, Co-CEOs of the Commercial & Investment Bank ("CIB"), have been elected Co-Presidents of the Firm, effective immediately.1 In addition to their new roles, Mr. Petno will become sole CEO of the CIB, and Mr. Rohrbaugh will become CEO of Consumer & Community Banking ("CCB"). |
| 31 | JPMORGAN CHASE & CO | 0000019617 | 0000019617-26-000241 | /Archives/edgar/data/19617/000001961726000241/jpm-20260624.htm | 9.01 | (d) Exhibit Exhibit No. Description of Exhibit 99.1 JPMorgan Chase & Co. Press Release dated June 25, 2026 101 Pursuant to Rule 406 of Regulation S-T, the cover page is formatted in Inline XBRL (Inline eXtensible Business Reporting Language). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document and included in Exhibit 101). |
| 32 | Mastercard Inc | 0001141391 | 0001141391-26-000041 | /Archives/edgar/data/1141391/000114139126000041/ma-20260616.htm | 5.07 | On June 16, 2026, Mastercard Incorporated ("Mastercard") held its annual meeting of stockholders (the "Annual Meeting"). |
| 33 | Alphabet Inc. | 0001652044 | 0001193125-26-267578 | /Archives/edgar/data/1652044/000119312526267578/d57679d8k.htm | 5.02 | Amended and Restated Alphabet Inc. 2021 Stock Plan At the Annual Meeting of Shareholders of Alphabet Inc. (“Alphabet”) held on June 5, 2026 (the “2026 Annual Meeting”), Alphabet’s shareholders approved the amendment and restatement of the Alphabet Inc. Amended and Restated 2021 Stock Plan (the “2021 Stock Plan”) to increase the share reserve by 200,000,000 shares of Class C capital stock. A description of the 2021 Stock Plan and related matters was set forth in Alphabet’s definitive proxy statement on Form 14A filed with the U.S. Securities and Exchange Commission on April 24, 2026 (the “2026 Proxy Statement”) and is qualified in its entirety by reference to the full text of the 2021 Stock Plan, a copy of which is being filed as Exhibit 10.01 to this Form 8-K. |
| 33 | Alphabet Inc. | 0001652044 | 0001193125-26-267578 | /Archives/edgar/data/1652044/000119312526267578/d57679d8k.htm | 5.07 | At the 2026 Annual Meeting, Alphabet’s shareholders voted on fourteen proposals as set forth below, all of which are described in detail in the 2026 Proxy Statement. |
| 33 | Alphabet Inc. | 0001652044 | 0001193125-26-267578 | /Archives/edgar/data/1652044/000119312526267578/d57679d8k.htm | 9.01 | (d) Exhibits. Exhibit No. Description 10.01 Alphabet Inc. Amended and Restated 2021 Stock Plan 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 34 | AMAZON COM INC | 0001018724 | 0001104659-26-072140 | /Archives/edgar/data/1018724/000110465926072140/tm2613616d4_8k.htm | 1.01 | On June 8, 2026, Amazon.com, Inc. (the “Company”), Citibank N.A., as administrative agent, and the lenders party thereto entered into a term loan agreement (the “DDTL Credit Agreement”). The DDTL Credit Agreement provides the Company with a $17.5 billion senior unsecured delayed draw term loan credit facility (the “DDTL Facility”). |
| 34 | AMAZON COM INC | 0001018724 | 0001104659-26-072140 | /Archives/edgar/data/1018724/000110465926072140/tm2613616d4_8k.htm | 2.03 | The information set forth in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 2.03. |
| 34 | AMAZON COM INC | 0001018724 | 0001104659-26-072140 | /Archives/edgar/data/1018724/000110465926072140/tm2613616d4_8k.htm | 9.01 | (d) Exhibits. Exhibit Number Description 10.1 Term Loan Agreement, dated as of June 8 2026, among Amazon.com, Inc., Citibank N.A., as administrative agent, and the lenders party thereto. 104 The cover page from this Current Report on Form 8-K, formatted in Inline XBRL (included as Exhibit 101). |
| 35 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-071845 | /Archives/edgar/data/723125/000110465926071845/tm2617112d1_8k.htm | 5.02 | On June 9, 2026, the Board of Directors (“Board”) of Micron Technology, Inc. (the “Company”) appointed Alexis Black Björlin as a member of the Board. The Board has determined that Dr. Björlin is an independent director under the applicable rules of the Nasdaq Stock Market LLC (the “Independence Rules”). Following the appointment of Dr. Björlin, the Board will have a total of nine directors, of which eight are determined to be independent under the Independence Rules. |
| 35 | MICRON TECHNOLOGY INC | 0000723125 | 0001104659-26-071845 | /Archives/edgar/data/723125/000110465926071845/tm2617112d1_8k.htm | 9.01 | (d) Exhibits. Exhibit No. Description 99.1 Press Release dated June 9, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document) |
| 36 | Palantir Technologies Inc. | 0001321655 | 0001321655-26-000033 | /Archives/edgar/data/1321655/000132165526000033/pltr-20260603.htm | 5.07 | On June 3, 2026, Palantir Technologies Inc. (the “Company”) held its 2026 annual meeting of stockholders (the “Annual Meeting”). |
| 37 | Alphabet Inc. | 0001652044 | 0001193125-26-259830 | /Archives/edgar/data/1652044/000119312526259830/d36818d8k.htm | 1.01 | Mandatory Convertible Preferred Stock Offering On June 2, 2026, Alphabet Inc. (“Alphabet” or the “Company”) entered into an underwriting agreement (the “Underwriting Agreement”) with Goldman Sachs & Co. LLC, J.P. Morgan Securities LLC, and Morgan Stanley & Co. LLC as the representatives of the respective underwriters under such agreement, pursuant to which Alphabet agreed to issue and sell (1) 167,500,000 series A depositary shares (the “Series A Depositary Shares”), each representing a 1/20th interest in a share of 6.25% Series A Mandatory Convertible Preferred Stock, liquidation preference $1,000.00 per share, par value $0.001 per share (the “Series A Preferred Stock” and such offering, the “Series A Depositary Shares Offering”) and (2) 167,500,000 series B depositary shares (the “Series B Depositary Shares” and together with the Series A Depositary Shares, the “Depositary Shares”), each representing a 1/20th interest in a share of 6.25% Series B Mandatory Convertible Preferred Stock, liquidation preference $1,000.00 per share, par value $0.001 per share (the “Series B Preferred Stock” and together with the Series A Preferred Stock, the “Preferred Stock” and such offering, the “Series B Depositary Shares Offering” and together with the Series A Depositary Shares Offering, the “Depositary Shares Offerings”). |
| 37 | Alphabet Inc. | 0001652044 | 0001193125-26-259830 | /Archives/edgar/data/1652044/000119312526259830/d36818d8k.htm | 3.03 | On June 4, 2026, the Company filed the Certificates of Designations with the Secretary of State of the State of Delaware to establish the preferences, limitations and relative rights of the respective series of Preferred Stock. |
| 37 | Alphabet Inc. | 0001652044 | 0001193125-26-259830 | /Archives/edgar/data/1652044/000119312526259830/d36818d8k.htm | 5.03 | The information set forth under Item 3.03 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 5.03. |
| 37 | Alphabet Inc. | 0001652044 | 0001193125-26-259830 | /Archives/edgar/data/1652044/000119312526259830/d36818d8k.htm | 9.01 | (d)Exhibits Exhibit No. Description 1.1 Form of Underwriting Agreement (Preferred Stock) (incorporated by reference to Exhibit 1.3 to Alphabet Inc’s Registration statement on Form S-3; File No: 333-296395) 3.1 Certificate of Designations for the 6.25% Series A Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective June 4, 2026 3.2 Certificate of Designations for the 6.25% Series B Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective June 4, 2026 4.1 Form of Certificate for the 6.25% Series A Mandatory Convertible Preferred Stock (included as Exhibit A to Exhibit 3.1) 4.2 Form of Certificate for the 6.25% Series B Mandatory Convertible Preferred Stock (included as Exhibit A to Exhibit 3.2) 4.3 Deposit Agreement for the Series A Mandatory Convertible Preferred Stock, dated as of June 5, 2026, among Alphabet Inc., Computershare Inc. and Computershare Trust Company, N.A., acting jointly as depositary 4.4 Deposit Agreement for the Series B Mandatory Convertible Preferred Stock, dated as of June 5, 2026, among Alphabet Inc., Computershare Inc. and Computershare Trust Company, N.A., acting jointly as depositary 4.5 Form of Depositary Receipt for the Series A Depositary Shares (included as Exhibit A to Exhibit 4.3) 4.6 Form of Depositary Receipt for the Series B Depositary Shares (included as Exhibit A to Exhibit 4.4) 5.1 Opinion of Cleary Gottlieb Steen & Hamilton LLP for the Series A Depositary Shares 5.2 Opinion of Cleary Gottlieb Steen & Hamilton LLP for the Series B Depositary Shares |
| 38 | Alphabet Inc. | 0001652044 | 0001652044-26-000059 | /Archives/edgar/data/1652044/000165204426000059/goog-20260602.htm | 5.02 | (c) Appointment of Principal Officer On June 5, 2026, Alphabet Inc. (“Alphabet”) announced the appointment of Marsida Saraci, Vice President and Controller, as its Principal Accounting Officer, effective immediately. |
| 39 | UNITEDHEALTH GROUP INC | 0000731766 | 0000731766-26-000138 | /Archives/edgar/data/731766/000073176626000138/unh-20260601.htm | 5.07 | On June 1, 2026, the Company held its 2026 Annual Meeting of Shareholders (the “Annual Meeting”). |
| 40 | Walmart Inc. | 0000104169 | 0000104169-26-000111 | /Archives/edgar/data/104169/000010416926000111/wmt-20260604.htm | 5.03 | On June 4, 2026, Walmart Inc. (the "Company") held its Annual Shareholders' Meeting (the "Meeting"). |
| 40 | Walmart Inc. | 0000104169 | 0000104169-26-000111 | /Archives/edgar/data/104169/000010416926000111/wmt-20260604.htm | 5.07 | As of close of business on April 10, 2026, the record date for the Meeting, there were 7,970,990,515 shares of the Company's common stock outstanding, with each share entitled to one vote. |
| 40 | Walmart Inc. | 0000104169 | 0000104169-26-000111 | /Archives/edgar/data/104169/000010416926000111/wmt-20260604.htm | 9.01 | (d) Exhibits 3.1 Certificate of Amendment of Restated Certificate of Incorporation of Walmart Inc., effective June 4, 2026 3.2 Restated Certificate of Incorporation of Walmart Inc., effective June 4, 2026 Exhibit 104 Cover Page Interactive Data File (embedded within the Inline XBRL) |

## Changes — PULL 2 vs PULL 1

Matched by accession (key). Columns compared: filingDate, form, items.

new count: 1
gone count: 0
changed count: 0
earlier row count: 466
later row count: 467
check: later = earlier + new - gone → 467 = 466 + 1 - 0

### New (key only in the later pull)

- key: 0001045810-26-000082 — row: accession 0001045810-26-000082, cik 0001045810, company NVIDIA CORP, form 8-K, filingDate 2026-11-12, reportDate 2026-11-11, acceptanceDateTime 2026-11-12T13:52:41.000Z, items 5.02,9.01

### Gone (key only in the earlier pull)

- none

### Changed (same key, a Changes column differs)

- none

## Changes — PULL 3 vs PULL 2

Matched by accession (key). Columns compared: filingDate, form, items.

new count: 2
gone count: 0
changed count: 0
earlier row count: 467
later row count: 469
check: later = earlier + new - gone → 469 = 467 + 2 - 0

### New (key only in the later pull)

- key: 0000858877-26-000170 — row: accession 0000858877-26-000170, cik 0000858877, company CISCO SYSTEMS, INC., form 8-K, filingDate 2026-11-12, reportDate 2026-11-12, acceptanceDateTime 2026-11-12T21:06:24.000Z, items 2.02,9.01
- key: 0001193125-26-458525 — row: accession 0001193125-26-458525, cik 0001326801, company Meta Platforms, Inc., form 8-K, filingDate 2026-11-12, reportDate 2026-11-12, acceptanceDateTime 2026-11-12T21:27:49.000Z, items 8.01,9.01

### Gone (key only in the earlier pull)

- none

### Changed (same key, a Changes column differs)

- none

## PROOF

### Acceptance items, quoted verbatim, with proving evidence

Acceptance 1: "The three CSV files are attached with exactly the listed columns, one row per 8-K or 8-K/A of the kept registrants in the period, no duplicate key (header-only only for a failed pull). [check: present, in D2]"

- Pull 1 CSV file: 8k-30-filers-pull1.csv
  columns: accession, cik, company, form, filingDate, reportDate, acceptanceDateTime, items
  row count: 466
  unique accession keys: 466
  SHA-256: a488df1534dc386644dfa9c6f30dfda2473f7015b1de93cf13a6a3efbf063aba
- Pull 2 CSV file: 8k-30-filers-pull2.csv
  columns: accession, cik, company, form, filingDate, reportDate, acceptanceDateTime, items
  row count: 467
  unique accession keys: 467
  SHA-256: 52791f46eaab79f3613a6e6b8d571477175a6d9f4e840bc35b4f1a9ec1592c2b
- Pull 3 CSV file: 8k-30-filers-pull3.csv
  columns: accession, cik, company, form, filingDate, reportDate, acceptanceDateTime, items
  row count: 469
  unique accession keys: 469
  SHA-256: 8c9ce3ac56b81b1de5db61a80b763583b9dc94b8f02ab1eb977f771df3a1d3ca

Acceptance 2: "Each pull's counts, item tally and item x registrant table agree with its CSV and the tie-break. [check: needs judgment]"

- Pull 1: row count: 466; registrants counted: 28; top item codes (count desc, code asc): 9.01: 341, 2.02: 170, 8.01: 125 — full counts, item tallies and item x registrant tables in the Pull sections above, recomputed from the CSV by the report builder.
- Pull 2: row count: 467; registrants counted: 28; top item codes (count desc, code asc): 9.01: 342, 2.02: 170, 8.01: 125 — full counts, item tallies and item x registrant tables in the Pull sections above, recomputed from the CSV by the report builder.
- Pull 3: row count: 469; registrants counted: 28; top item codes (count desc, code asc): 9.01: 344, 2.02: 171, 8.01: 126 — full counts, item tallies and item x registrant tables in the Pull sections above, recomputed from the CSV by the report builder.

Acceptance 3: "The review table has the 40 most recent qualifying rows of the pull the review uses (or all that qualify, with the count stated), each with its document path, every item code and one line per item as the TASK asks. [check: needs judgment]"

- qualifying_count: 161
- review_count: 40
- Review source pull: pull 1. The review table above lists all 40 filings with company, CIK, accession, document path, every headed item code and one line per item.

Acceptance 4: "Each reviewed filing's item codes match its index and headings in the PROOF, and each line is consistent with the text excerpted under that heading. [check: matches the source, source SEC EDGAR]"

- Per reviewed filing, the PROOF excerpts below give the index page's Items list, the Documents table row for the filed document, and each item heading with the sentence(s) under it; the review table's codes are the headed codes and each one line is taken from those excerpts.
- Filings whose headed codes include a code beyond the index Items list other than 9.01: none

Acceptance 5: "The PLATFORM RECORD shows a PULL 1: note and each later PULL note at least its wait after the one before, each with its CSV's row count and SHA-256 as under DATA FILES; each pull's source time (the HTTP Date header of its first request) is later than the previous pull's; the change counts agree with the CSV files (or a pull failed as the TASK allows). [check: timing, target 24 hours between each pair of notes]"

- CSV row counts and SHA-256 values are as in Acceptance 1 above and in the synmerco-data block at the end.
- Pull 1 first request Date header: Wed, 11 Nov 2026 16:20:55 GMT
- Pull 2 first request Date header: Thu, 12 Nov 2026 16:31:49 GMT
- Pull 3 first request Date header: Fri, 13 Nov 2026 16:33:33 GMT
- Each pull's first-request source time (HTTP Date header) is later than the previous pull's: pull 2 after pull 1, pull 3 after pull 2 (see the request lists below).
- Platform progress notes (GET /v1/escrows/esc_550d5871c8594d7e90489519/progress, count: 3): PULL 1 note recordedAt 2026-11-11 16:22:16 UTC; PULL 2 note recordedAt 2026-11-12 16:32:46 UTC (24h10m30s after the PULL 1 note); PULL 3 note recordedAt 2026-11-13 16:34:22 UTC (24h01m36s after the PULL 2 note). Each note states its CSV's row count and SHA-256 as under DATA FILES.
- Change counts recomputed from the CSVs — PULL 2 vs PULL 1: new count: 1, gone count: 0, changed count: 0; PULL 3 vs PULL 2: new count: 2, gone count: 0, changed count: 0.

### Every request — pulls

#### Pull 1 requests

- URL: https://www.sec.gov/files/company_tickers.json | UTC: 2026-11-11T16:20:54Z | Date: Wed, 11 Nov 2026 16:20:55 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000320193.json | UTC: 2026-11-11T16:20:55Z | Date: Wed, 11 Nov 2026 16:20:56 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001045810.json | UTC: 2026-11-11T16:20:57Z | Date: Wed, 11 Nov 2026 16:20:57 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000789019.json | UTC: 2026-11-11T16:21:00Z | Date: Wed, 11 Nov 2026 16:21:00 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001652044.json | UTC: 2026-11-11T16:21:00Z | Date: Wed, 11 Nov 2026 16:21:01 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001018724.json | UTC: 2026-11-11T16:21:01Z | Date: Wed, 11 Nov 2026 16:21:02 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001326801.json | UTC: 2026-11-11T16:21:03Z | Date: Wed, 11 Nov 2026 16:21:03 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001730168.json | UTC: 2026-11-11T16:21:04Z | Date: Wed, 11 Nov 2026 16:21:04 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001318605.json | UTC: 2026-11-11T16:21:05Z | Date: Wed, 11 Nov 2026 16:21:05 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000059478.json | UTC: 2026-11-11T16:21:06Z | Date: Wed, 11 Nov 2026 16:21:06 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001067983.json | UTC: 2026-11-11T16:21:07Z | Date: Wed, 11 Nov 2026 16:21:07 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000104169.json | UTC: 2026-11-11T16:21:08Z | Date: Wed, 11 Nov 2026 16:21:09 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002120882.json | UTC: 2026-11-11T16:21:09Z | Date: Wed, 11 Nov 2026 16:21:10 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617.json | UTC: 2026-11-11T16:21:10Z | Date: Wed, 11 Nov 2026 16:21:10 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-001.json | UTC: 2026-11-11T16:21:11Z | Date: Wed, 11 Nov 2026 16:21:11 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-002.json | UTC: 2026-11-11T16:21:12Z | Date: Wed, 11 Nov 2026 16:21:12 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-003.json | UTC: 2026-11-11T16:21:13Z | Date: Wed, 11 Nov 2026 16:21:13 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-004.json | UTC: 2026-11-11T16:21:14Z | Date: Wed, 11 Nov 2026 16:21:14 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000002488.json | UTC: 2026-11-11T16:21:15Z | Date: Wed, 11 Nov 2026 16:21:15 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000723125.json | UTC: 2026-11-11T16:21:15Z | Date: Wed, 11 Nov 2026 16:21:16 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001403161.json | UTC: 2026-11-11T16:21:16Z | Date: Wed, 11 Nov 2026 16:21:17 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000200406.json | UTC: 2026-11-11T16:21:17Z | Date: Wed, 11 Nov 2026 16:21:18 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002115436.json | UTC: 2026-11-11T16:21:18Z | Date: Wed, 11 Nov 2026 16:21:19 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000937966.json | UTC: 2026-11-11T16:21:19Z | Date: Wed, 11 Nov 2026 16:21:20 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001141391.json | UTC: 2026-11-11T16:21:20Z | Date: Wed, 11 Nov 2026 16:21:21 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001551152.json | UTC: 2026-11-11T16:21:21Z | Date: Wed, 11 Nov 2026 16:21:21 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000909832.json | UTC: 2026-11-11T16:21:22Z | Date: Wed, 11 Nov 2026 16:21:22 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000021344.json | UTC: 2026-11-11T16:21:23Z | Date: Wed, 11 Nov 2026 16:21:23 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001321655.json | UTC: 2026-11-11T16:21:24Z | Date: Wed, 11 Nov 2026 16:21:24 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000093410.json | UTC: 2026-11-11T16:21:25Z | Date: Wed, 11 Nov 2026 16:21:25 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000080424.json | UTC: 2026-11-11T16:21:25Z | Date: Wed, 11 Nov 2026 16:21:26 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000858877.json | UTC: 2026-11-11T16:21:27Z | Date: Wed, 11 Nov 2026 16:21:28 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001341439.json | UTC: 2026-11-11T16:21:28Z | Date: Wed, 11 Nov 2026 16:21:29 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000310158.json | UTC: 2026-11-11T16:21:30Z | Date: Wed, 11 Nov 2026 16:21:30 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000731766.json | UTC: 2026-11-11T16:21:31Z | Date: Wed, 11 Nov 2026 16:21:31 GMT | status: 200

#### Pull 2 requests

- URL: https://www.sec.gov/files/company_tickers.json | UTC: 2026-11-12T16:31:48Z | Date: Thu, 12 Nov 2026 16:31:49 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000320193.json | UTC: 2026-11-12T16:31:49Z | Date: Thu, 12 Nov 2026 16:31:50 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001045810.json | UTC: 2026-11-12T16:31:49Z | Date: Thu, 12 Nov 2026 16:31:50 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000789019.json | UTC: 2026-11-12T16:31:50Z | Date: Thu, 12 Nov 2026 16:31:51 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001652044.json | UTC: 2026-11-12T16:31:51Z | Date: Thu, 12 Nov 2026 16:31:52 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001018724.json | UTC: 2026-11-12T16:31:52Z | Date: Thu, 12 Nov 2026 16:31:53 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001326801.json | UTC: 2026-11-12T16:31:52Z | Date: Thu, 12 Nov 2026 16:31:53 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001318605.json | UTC: 2026-11-12T16:31:53Z | Date: Thu, 12 Nov 2026 16:31:54 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001730168.json | UTC: 2026-11-12T16:31:54Z | Date: Thu, 12 Nov 2026 16:31:55 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001067983.json | UTC: 2026-11-12T16:31:55Z | Date: Thu, 12 Nov 2026 16:31:56 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000059478.json | UTC: 2026-11-12T16:31:55Z | Date: Thu, 12 Nov 2026 16:31:56 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000104169.json | UTC: 2026-11-12T16:31:56Z | Date: Thu, 12 Nov 2026 16:31:57 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002120882.json | UTC: 2026-11-12T16:31:57Z | Date: Thu, 12 Nov 2026 16:31:58 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617.json | UTC: 2026-11-12T16:31:58Z | Date: Thu, 12 Nov 2026 16:31:59 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-001.json | UTC: 2026-11-12T16:32:00Z | Date: Thu, 12 Nov 2026 16:32:01 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-002.json | UTC: 2026-11-12T16:32:00Z | Date: Thu, 12 Nov 2026 16:32:01 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-003.json | UTC: 2026-11-12T16:32:01Z | Date: Thu, 12 Nov 2026 16:32:02 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-004.json | UTC: 2026-11-12T16:32:02Z | Date: Thu, 12 Nov 2026 16:32:03 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-005.json | UTC: 2026-11-12T16:32:03Z | Date: Thu, 12 Nov 2026 16:32:04 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001403161.json | UTC: 2026-11-12T16:32:03Z | Date: Thu, 12 Nov 2026 16:32:04 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000723125.json | UTC: 2026-11-12T16:32:04Z | Date: Thu, 12 Nov 2026 16:32:05 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000002488.json | UTC: 2026-11-12T16:32:06Z | Date: Thu, 12 Nov 2026 16:32:07 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002115436.json | UTC: 2026-11-12T16:32:07Z | Date: Thu, 12 Nov 2026 16:32:08 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000200406.json | UTC: 2026-11-12T16:32:08Z | Date: Thu, 12 Nov 2026 16:32:09 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001141391.json | UTC: 2026-11-12T16:32:11Z | Date: Thu, 12 Nov 2026 16:32:11 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000937966.json | UTC: 2026-11-12T16:32:12Z | Date: Thu, 12 Nov 2026 16:32:13 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001551152.json | UTC: 2026-11-12T16:32:13Z | Date: Thu, 12 Nov 2026 16:32:14 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000909832.json | UTC: 2026-11-12T16:32:14Z | Date: Thu, 12 Nov 2026 16:32:15 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000093410.json | UTC: 2026-11-12T16:32:15Z | Date: Thu, 12 Nov 2026 16:32:16 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000021344.json | UTC: 2026-11-12T16:32:16Z | Date: Thu, 12 Nov 2026 16:32:17 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001321655.json | UTC: 2026-11-12T16:32:17Z | Date: Thu, 12 Nov 2026 16:32:18 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000080424.json | UTC: 2026-11-12T16:32:18Z | Date: Thu, 12 Nov 2026 16:32:19 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000858877.json | UTC: 2026-11-12T16:32:20Z | Date: Thu, 12 Nov 2026 16:32:21 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000310158.json | UTC: 2026-11-12T16:32:21Z | Date: Thu, 12 Nov 2026 16:32:22 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001341439.json | UTC: 2026-11-12T16:32:22Z | Date: Thu, 12 Nov 2026 16:32:23 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000731766.json | UTC: 2026-11-12T16:32:22Z | Date: Thu, 12 Nov 2026 16:32:23 GMT | status: 200

#### Pull 3 requests

- URL: https://www.sec.gov/files/company_tickers.json | UTC: 2026-11-13T16:33:34Z | Date: Fri, 13 Nov 2026 16:33:33 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000320193.json | UTC: 2026-11-13T16:33:35Z | Date: Fri, 13 Nov 2026 16:33:36 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001045810.json | UTC: 2026-11-13T16:33:37Z | Date: Fri, 13 Nov 2026 16:33:37 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000789019.json | UTC: 2026-11-13T16:33:38Z | Date: Fri, 13 Nov 2026 16:33:39 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001652044.json | UTC: 2026-11-13T16:33:39Z | Date: Fri, 13 Nov 2026 16:33:40 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001018724.json | UTC: 2026-11-13T16:33:41Z | Date: Fri, 13 Nov 2026 16:33:42 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001326801.json | UTC: 2026-11-13T16:33:43Z | Date: Fri, 13 Nov 2026 16:33:43 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001730168.json | UTC: 2026-11-13T16:33:44Z | Date: Fri, 13 Nov 2026 16:33:45 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001318605.json | UTC: 2026-11-13T16:33:46Z | Date: Fri, 13 Nov 2026 16:33:46 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000059478.json | UTC: 2026-11-13T16:33:47Z | Date: Fri, 13 Nov 2026 16:33:48 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001067983.json | UTC: 2026-11-13T16:33:49Z | Date: Fri, 13 Nov 2026 16:33:49 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000104169.json | UTC: 2026-11-13T16:33:50Z | Date: Fri, 13 Nov 2026 16:33:51 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002120882.json | UTC: 2026-11-13T16:33:52Z | Date: Fri, 13 Nov 2026 16:33:53 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617.json | UTC: 2026-11-13T16:33:55Z | Date: Fri, 13 Nov 2026 16:33:54 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-001.json | UTC: 2026-11-13T16:33:56Z | Date: Fri, 13 Nov 2026 16:33:56 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-002.json | UTC: 2026-11-13T16:33:57Z | Date: Fri, 13 Nov 2026 16:33:58 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-003.json | UTC: 2026-11-13T16:33:58Z | Date: Fri, 13 Nov 2026 16:33:59 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-004.json | UTC: 2026-11-13T16:33:59Z | Date: Fri, 13 Nov 2026 16:34:00 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000019617-submissions-005.json | UTC: 2026-11-13T16:34:00Z | Date: Fri, 13 Nov 2026 16:34:01 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000002488.json | UTC: 2026-11-13T16:34:01Z | Date: Fri, 13 Nov 2026 16:34:02 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000723125.json | UTC: 2026-11-13T16:34:02Z | Date: Fri, 13 Nov 2026 16:34:03 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001403161.json | UTC: 2026-11-13T16:34:04Z | Date: Fri, 13 Nov 2026 16:34:04 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000200406.json | UTC: 2026-11-13T16:34:05Z | Date: Fri, 13 Nov 2026 16:34:06 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0002115436.json | UTC: 2026-11-13T16:34:06Z | Date: Fri, 13 Nov 2026 16:34:07 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000937966.json | UTC: 2026-11-13T16:34:07Z | Date: Fri, 13 Nov 2026 16:34:08 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001141391.json | UTC: 2026-11-13T16:34:09Z | Date: Fri, 13 Nov 2026 16:34:09 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001551152.json | UTC: 2026-11-13T16:34:09Z | Date: Fri, 13 Nov 2026 16:34:10 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000909832.json | UTC: 2026-11-13T16:34:11Z | Date: Fri, 13 Nov 2026 16:34:11 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000021344.json | UTC: 2026-11-13T16:34:12Z | Date: Fri, 13 Nov 2026 16:34:12 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001321655.json | UTC: 2026-11-13T16:34:13Z | Date: Fri, 13 Nov 2026 16:34:14 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000093410.json | UTC: 2026-11-13T16:34:14Z | Date: Fri, 13 Nov 2026 16:34:15 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000080424.json | UTC: 2026-11-13T16:34:15Z | Date: Fri, 13 Nov 2026 16:34:16 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000858877.json | UTC: 2026-11-13T16:34:16Z | Date: Fri, 13 Nov 2026 16:34:17 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0001341439.json | UTC: 2026-11-13T16:34:18Z | Date: Fri, 13 Nov 2026 16:34:19 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000310158.json | UTC: 2026-11-13T16:34:20Z | Date: Fri, 13 Nov 2026 16:34:20 GMT | status: 200
- URL: https://data.sec.gov/submissions/CIK0000731766.json | UTC: 2026-11-13T16:34:21Z | Date: Fri, 13 Nov 2026 16:34:22 GMT | status: 200

### Every request — review (from pull 1)

- doc | URL: https://www.sec.gov/Archives/edgar/data/909832/000090983226000134/cost-20261107.htm | UTC: 2026-11-11T16:25:55Z | Date: Wed, 11 Nov 2026 16:25:56 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/909832/000090983226000134/0000909832-26-000134-index.htm | UTC: 2026-11-11T16:25:55Z | Date: Wed, 11 Nov 2026 16:25:55 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/731766/000073176626000274/unh-20261103.htm | UTC: 2026-11-11T16:25:57Z | Date: Wed, 11 Nov 2026 16:25:57 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/731766/000073176626000274/0000731766-26-000274-index.htm | UTC: 2026-11-11T16:25:56Z | Date: Wed, 11 Nov 2026 16:25:56 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926123389/tm2629062d1_8k.htm | UTC: 2026-11-11T16:25:58Z | Date: Wed, 11 Nov 2026 16:25:58 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926123389/0001104659-26-123389-index.htm | UTC: 2026-11-11T16:25:57Z | Date: Wed, 11 Nov 2026 16:25:58 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/789019/000119312526448357/d177209d8k.htm | UTC: 2026-11-11T16:25:59Z | Date: Wed, 11 Nov 2026 16:26:00 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/789019/000119312526448357/0001193125-26-448357-index.htm | UTC: 2026-11-11T16:25:58Z | Date: Wed, 11 Nov 2026 16:25:59 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1551152/000110465926121322/tm2628215d1_8k.htm | UTC: 2026-11-11T16:26:00Z | Date: Wed, 11 Nov 2026 16:26:01 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1551152/000110465926121322/0001104659-26-121322-index.htm | UTC: 2026-11-11T16:26:00Z | Date: Wed, 11 Nov 2026 16:26:00 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1326801/000119312526438017/d183592d8k.htm | UTC: 2026-11-11T16:26:02Z | Date: Wed, 11 Nov 2026 16:26:03 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1326801/000119312526438017/0001193125-26-438017-index.htm | UTC: 2026-11-11T16:26:01Z | Date: Wed, 11 Nov 2026 16:26:02 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1730168/000119312526434271/d148323d8k.htm | UTC: 2026-11-11T16:26:04Z | Date: Wed, 11 Nov 2026 16:26:05 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1730168/000119312526434271/0001193125-26-434271-index.htm | UTC: 2026-11-11T16:26:03Z | Date: Wed, 11 Nov 2026 16:26:04 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1326801/000162828026066700/meta-20261019.htm | UTC: 2026-11-11T16:26:07Z | Date: Wed, 11 Nov 2026 16:26:08 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1326801/000162828026066700/0001628280-26-066700-index.htm | UTC: 2026-11-11T16:26:05Z | Date: Wed, 11 Nov 2026 16:26:05 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/909832/000090983226000100/cost-20261013.htm | UTC: 2026-11-11T16:26:08Z | Date: Wed, 11 Nov 2026 16:26:09 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/909832/000090983226000100/0000909832-26-000100-index.htm | UTC: 2026-11-11T16:26:08Z | Date: Wed, 11 Nov 2026 16:26:08 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/80424/000008042426000245/pg-20261016.htm | UTC: 2026-11-11T16:26:09Z | Date: Wed, 11 Nov 2026 16:26:10 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/80424/000008042426000245/0000080424-26-000245-index.htm | UTC: 2026-11-11T16:26:09Z | Date: Wed, 11 Nov 2026 16:26:09 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1551152/000110465926116227/tm2627361d1_8k.htm | UTC: 2026-11-11T16:26:11Z | Date: Wed, 11 Nov 2026 16:26:11 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1551152/000110465926116227/0001104659-26-116227-index.htm | UTC: 2026-11-11T16:26:10Z | Date: Wed, 11 Nov 2026 16:26:11 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/310158/000031015826000237/mrk-20261009.htm | UTC: 2026-11-11T16:26:12Z | Date: Wed, 11 Nov 2026 16:26:13 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/310158/000031015826000237/0000310158-26-000237-index.htm | UTC: 2026-11-11T16:26:12Z | Date: Wed, 11 Nov 2026 16:26:12 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/858877/000085887726000156/csco-20261007.htm | UTC: 2026-11-11T16:26:14Z | Date: Wed, 11 Nov 2026 16:26:14 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/858877/000085887726000156/0000858877-26-000156-index.htm | UTC: 2026-11-11T16:26:13Z | Date: Wed, 11 Nov 2026 16:26:14 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/93410/000009341026000188/cvx-20260930.htm | UTC: 2026-11-11T16:26:15Z | Date: Wed, 11 Nov 2026 16:26:16 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/93410/000009341026000188/0000093410-26-000188-index.htm | UTC: 2026-11-11T16:26:14Z | Date: Wed, 11 Nov 2026 16:26:15 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1318605/000162828026063820/tsla-20260929.htm | UTC: 2026-11-11T16:26:17Z | Date: Wed, 11 Nov 2026 16:26:17 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1318605/000162828026063820/0001628280-26-063820-index.htm | UTC: 2026-11-11T16:26:16Z | Date: Wed, 11 Nov 2026 16:26:17 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000182/amd-20260926.htm | UTC: 2026-11-11T16:26:18Z | Date: Wed, 11 Nov 2026 16:26:18 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000182/0000002488-26-000182-index.htm | UTC: 2026-11-11T16:26:17Z | Date: Wed, 11 Nov 2026 16:26:18 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1018724/000101872426000036/amzn-20260908.htm | UTC: 2026-11-11T16:26:19Z | Date: Wed, 11 Nov 2026 16:26:20 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1018724/000101872426000036/0001018724-26-000036-index.htm | UTC: 2026-11-11T16:26:19Z | Date: Wed, 11 Nov 2026 16:26:19 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/320193/000114036126035325/ef20081427_8ka.htm | UTC: 2026-11-11T16:26:21Z | Date: Wed, 11 Nov 2026 16:26:21 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/320193/000114036126035325/0001140361-26-035325-index.htm | UTC: 2026-11-11T16:26:20Z | Date: Wed, 11 Nov 2026 16:26:21 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926101067/tm2624017d1_8k.htm | UTC: 2026-11-11T16:26:23Z | Date: Wed, 11 Nov 2026 16:26:23 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926101067/0001104659-26-101067-index.htm | UTC: 2026-11-11T16:26:22Z | Date: Wed, 11 Nov 2026 16:26:22 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000163/amd-20260817.htm | UTC: 2026-11-11T16:26:24Z | Date: Wed, 11 Nov 2026 16:26:25 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000163/0000002488-26-000163-index.htm | UTC: 2026-11-11T16:26:23Z | Date: Wed, 11 Nov 2026 16:26:24 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/2488/000119312526354029/d142696d8k.htm | UTC: 2026-11-11T16:26:26Z | Date: Wed, 11 Nov 2026 16:26:27 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/2488/000119312526354029/0001193125-26-354029-index.htm | UTC: 2026-11-11T16:26:25Z | Date: Wed, 11 Nov 2026 16:26:25 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000069/nvda-20260817.htm | UTC: 2026-11-11T16:26:27Z | Date: Wed, 11 Nov 2026 16:26:28 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000069/0001045810-26-000069-index.htm | UTC: 2026-11-11T16:26:27Z | Date: Wed, 11 Nov 2026 16:26:27 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/200406/000020040626000167/jnj-20260804.htm | UTC: 2026-11-11T16:26:29Z | Date: Wed, 11 Nov 2026 16:26:30 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/200406/000020040626000167/0000200406-26-000167-index.htm | UTC: 2026-11-11T16:26:28Z | Date: Wed, 11 Nov 2026 16:26:29 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/80424/000008042426000094/pg-20260729.htm | UTC: 2026-11-11T16:26:31Z | Date: Wed, 11 Nov 2026 16:26:32 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/80424/000008042426000094/0000080424-26-000094-index.htm | UTC: 2026-11-11T16:26:30Z | Date: Wed, 11 Nov 2026 16:26:31 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/19617/000001961726000288/jpm-20260721.htm | UTC: 2026-11-11T16:26:32Z | Date: Wed, 11 Nov 2026 16:26:33 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/19617/000001961726000288/0000019617-26-000288-index.htm | UTC: 2026-11-11T16:26:32Z | Date: Wed, 11 Nov 2026 16:26:32 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1403161/000140316126000096/v-20260714.htm | UTC: 2026-11-11T16:26:34Z | Date: Wed, 11 Nov 2026 16:26:35 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1403161/000140316126000096/0001403161-26-000096-index.htm | UTC: 2026-11-11T16:26:33Z | Date: Wed, 11 Nov 2026 16:26:34 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000060/nvda-20260628.htm | UTC: 2026-11-11T16:26:37Z | Date: Wed, 11 Nov 2026 16:26:37 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000060/0001045810-26-000060-index.htm | UTC: 2026-11-11T16:26:35Z | Date: Wed, 11 Nov 2026 16:26:35 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000115/amd-20260626.htm | UTC: 2026-11-11T16:26:39Z | Date: Wed, 11 Nov 2026 16:26:39 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/2488/000000248826000115/0000002488-26-000115-index.htm | UTC: 2026-11-11T16:26:38Z | Date: Wed, 11 Nov 2026 16:26:38 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000056/nvda-20260624.htm | UTC: 2026-11-11T16:26:40Z | Date: Wed, 11 Nov 2026 16:26:41 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1045810/000104581026000056/0001045810-26-000056-index.htm | UTC: 2026-11-11T16:26:40Z | Date: Wed, 11 Nov 2026 16:26:40 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/21344/000155278126000366/e26287_ko-8k.htm | UTC: 2026-11-11T16:26:42Z | Date: Wed, 11 Nov 2026 16:26:43 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/21344/000155278126000366/0001552781-26-000366-index.htm | UTC: 2026-11-11T16:26:41Z | Date: Wed, 11 Nov 2026 16:26:42 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/19617/000001961726000241/jpm-20260624.htm | UTC: 2026-11-11T16:26:45Z | Date: Wed, 11 Nov 2026 16:26:45 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/19617/000001961726000241/0000019617-26-000241-index.htm | UTC: 2026-11-11T16:26:43Z | Date: Wed, 11 Nov 2026 16:26:44 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1141391/000114139126000041/ma-20260616.htm | UTC: 2026-11-11T16:26:46Z | Date: Wed, 11 Nov 2026 16:26:46 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1141391/000114139126000041/0001141391-26-000041-index.htm | UTC: 2026-11-11T16:26:45Z | Date: Wed, 11 Nov 2026 16:26:46 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1652044/000119312526267578/d57679d8k.htm | UTC: 2026-11-11T16:26:47Z | Date: Wed, 11 Nov 2026 16:26:48 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1652044/000119312526267578/0001193125-26-267578-index.htm | UTC: 2026-11-11T16:26:47Z | Date: Wed, 11 Nov 2026 16:26:47 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1018724/000110465926072140/tm2613616d4_8k.htm | UTC: 2026-11-11T16:26:49Z | Date: Wed, 11 Nov 2026 16:26:50 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1018724/000110465926072140/0001104659-26-072140-index.htm | UTC: 2026-11-11T16:26:48Z | Date: Wed, 11 Nov 2026 16:26:48 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926071845/tm2617112d1_8k.htm | UTC: 2026-11-11T16:26:51Z | Date: Wed, 11 Nov 2026 16:26:51 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/723125/000110465926071845/0001104659-26-071845-index.htm | UTC: 2026-11-11T16:26:50Z | Date: Wed, 11 Nov 2026 16:26:50 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1321655/000132165526000033/pltr-20260603.htm | UTC: 2026-11-11T16:26:52Z | Date: Wed, 11 Nov 2026 16:26:53 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1321655/000132165526000033/0001321655-26-000033-index.htm | UTC: 2026-11-11T16:26:51Z | Date: Wed, 11 Nov 2026 16:26:52 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1652044/000119312526259830/d36818d8k.htm | UTC: 2026-11-11T16:26:54Z | Date: Wed, 11 Nov 2026 16:26:54 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1652044/000119312526259830/0001193125-26-259830-index.htm | UTC: 2026-11-11T16:26:53Z | Date: Wed, 11 Nov 2026 16:26:53 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/1652044/000165204426000059/goog-20260602.htm | UTC: 2026-11-11T16:26:55Z | Date: Wed, 11 Nov 2026 16:26:56 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/1652044/000165204426000059/0001652044-26-000059-index.htm | UTC: 2026-11-11T16:26:55Z | Date: Wed, 11 Nov 2026 16:26:55 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/731766/000073176626000138/unh-20260601.htm | UTC: 2026-11-11T16:26:57Z | Date: Wed, 11 Nov 2026 16:26:57 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/731766/000073176626000138/0000731766-26-000138-index.htm | UTC: 2026-11-11T16:26:56Z | Date: Wed, 11 Nov 2026 16:26:56 GMT | status: 200
- doc | URL: https://www.sec.gov/Archives/edgar/data/104169/000010416926000111/wmt-20260604.htm | UTC: 2026-11-11T16:26:58Z | Date: Wed, 11 Nov 2026 16:26:58 GMT | status: 200
- index | URL: https://www.sec.gov/Archives/edgar/data/104169/000010416926000111/0000104169-26-000111-index.htm | UTC: 2026-11-11T16:26:57Z | Date: Wed, 11 Nov 2026 16:26:58 GMT | status: 200

### Per-row values at each row's index of the six arrays

For each pull, per 8-K row (in CSV order): accessionNumber, filingDate, reportDate, acceptanceDateTime, form, items — one per line.

#### Pull 1 rows

row 0:
accessionNumber: 0001045810-25-000179
filingDate: 2025-07-01
reportDate: 2025-06-25
acceptanceDateTime: 2025-06-30T22:35:29.000Z
form: 8-K
items: 5.07
row 1:
accessionNumber: 0000019617-25-000509
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:30:37.000Z
form: 8-K
items: 8.01,9.01
row 2:
accessionNumber: 0000019617-25-000510
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:31:18.000Z
form: 8-K
items: 7.01,9.01
row 3:
accessionNumber: 0001193125-25-154103
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T21:00:47.000Z
form: 8-K
items: 5.03,9.01
row 4:
accessionNumber: 0001628280-25-033842
filingDate: 2025-07-02
reportDate: 2025-07-02
acceptanceDateTime: 2025-07-02T13:05:13.000Z
form: 8-K
items: 2.02,9.01
row 5:
accessionNumber: 0000002488-25-000099
filingDate: 2025-07-02
reportDate: 2025-06-27
acceptanceDateTime: 2025-07-02T20:14:22.000Z
form: 8-K
items: 5.02
row 6:
accessionNumber: 0001551152-25-000034
filingDate: 2025-07-03
reportDate: 2025-07-03
acceptanceDateTime: 2025-07-03T17:07:55.000Z
form: 8-K
items: 2.02,9.01
row 7:
accessionNumber: 0000080424-25-000057
filingDate: 2025-07-08
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-08T20:20:53.000Z
form: 8-K
items: 7.01,9.01
row 8:
accessionNumber: 0001140361-25-025275
filingDate: 2025-07-09
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-09T01:18:13.000Z
form: 8-K
items: 5.02
row 9:
accessionNumber: 0001628280-25-034692
filingDate: 2025-07-10
reportDate: 2025-07-09
acceptanceDateTime: 2025-07-10T01:18:15.000Z
form: 8-K
items: 5.08
row 10:
accessionNumber: 0001193125-25-158202
filingDate: 2025-07-11
reportDate: 2025-07-11
acceptanceDateTime: 2025-07-11T20:14:59.000Z
form: 8-K
items: 1.02,8.01,9.01
row 11:
accessionNumber: 0000019617-25-000518
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T10:30:58.000Z
form: 8-K
items: 2.02,9.01
row 12:
accessionNumber: 0000019617-25-000520
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T14:36:04.000Z
form: 8-K
items: 7.01,9.01
row 13:
accessionNumber: 0000200406-25-000170
filingDate: 2025-07-16
reportDate: 2025-07-16
acceptanceDateTime: 2025-07-16T12:06:45.000Z
form: 8-K
items: 2.02,9.01
row 14:
accessionNumber: 0000909832-25-000061
filingDate: 2025-07-16
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-16T20:18:04.000Z
form: 8-K
items: 8.01,9.01
row 15:
accessionNumber: 0000950142-25-001949
filingDate: 2025-07-18
reportDate: 2025-07-18
acceptanceDateTime: 2025-07-18T12:40:31.000Z
form: 8-K
items: 7.01,8.01,9.01
row 16:
accessionNumber: 0001104659-25-069019
filingDate: 2025-07-18
reportDate: 2025-07-17
acceptanceDateTime: 2025-07-18T20:05:39.000Z
form: 8-K
items: 5.03,9.01
row 17:
accessionNumber: 0001193125-25-161225
filingDate: 2025-07-18
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-18T20:16:46.000Z
form: 8-K
items: 8.01,9.01
row 18:
accessionNumber: 0000021344-25-000054
filingDate: 2025-07-22
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-22T11:00:23.000Z
form: 8-K
items: 2.02,9.01
row 19:
accessionNumber: 0001652044-25-000056
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:01:33.000Z
form: 8-K
items: 2.02,8.01,9.01
row 20:
accessionNumber: 0001403161-25-000043
filingDate: 2025-07-23
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-23T20:08:09.000Z
form: 8-K
items: 5.03
row 21:
accessionNumber: 0001628280-25-035738
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:14:09.000Z
form: 8-K
items: 2.02,9.01
row 22:
accessionNumber: 0001193125-25-163423
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:15:17.000Z
form: 8-K
items: 8.01,9.01
row 23:
accessionNumber: 0000731766-25-000224
filingDate: 2025-07-24
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-24T12:30:24.000Z
form: 8-K
items: 8.01
row 24:
accessionNumber: 0001140361-25-027340
filingDate: 2025-07-25
reportDate: 2025-07-21
acceptanceDateTime: 2025-07-25T20:30:49.000Z
form: 8-K
items: 5.02
row 25:
accessionNumber: 0000080424-25-000061
filingDate: 2025-07-28
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-28T21:03:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 26:
accessionNumber: 0000731766-25-000228
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T10:04:05.000Z
form: 8-K
items: 2.02,9.01
row 27:
accessionNumber: 0001104659-25-071380
filingDate: 2025-07-29
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-29T10:42:43.000Z
form: 8-K
items: 2.02,2.05,9.01
row 28:
accessionNumber: 0000080424-25-000067
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T11:03:15.000Z
form: 8-K
items: 2.02,9.01
row 29:
accessionNumber: 0000080424-25-000069
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T14:51:39.000Z
form: 8-K
items: 7.01,9.01
row 30:
accessionNumber: 0001403161-25-000051
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T20:06:16.000Z
form: 8-K
items: 2.02,8.01,9.01
row 31:
accessionNumber: 0000950142-25-002041
filingDate: 2025-07-29
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-29T20:10:21.000Z
form: 8-K
items: 5.02
row 32:
accessionNumber: 0000950170-25-100226
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:08:53.000Z
form: 8-K
items: 2.02,9.01
row 33:
accessionNumber: 0001628280-25-036719
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 34:
accessionNumber: 0001551152-25-000036
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T11:48:24.000Z
form: 8-K
items: 2.02,9.01
row 35:
accessionNumber: 0001141391-25-000170
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T12:03:19.000Z
form: 8-K
items: 2.02,9.01
row 36:
accessionNumber: 0001018724-25-000084
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:13:17.000Z
form: 8-K
items: 2.02,9.01
row 37:
accessionNumber: 0000320193-25-000071
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:30:25.000Z
form: 8-K
items: 2.02,9.01
row 38:
accessionNumber: 0000731766-25-000232
filingDate: 2025-07-31
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-31T21:08:18.000Z
form: 8-K
items: 5.02
row 39:
accessionNumber: 0000093410-25-000058
filingDate: 2025-08-01
reportDate: 2025-08-01
acceptanceDateTime: 2025-08-01T10:17:27.000Z
form: 8-K
items: 2.02,9.01
row 40:
accessionNumber: 0001104659-25-073263
filingDate: 2025-08-04
reportDate: 2025-08-03
acceptanceDateTime: 2025-08-04T10:03:14.000Z
form: 8-K
items: 5.02,7.01,9.01
row 41:
accessionNumber: 0001193125-25-172579
filingDate: 2025-08-04
reportDate: 2025-08-02
acceptanceDateTime: 2025-08-04T19:55:28.000Z
form: 8-K
items: 2.02,9.01
row 42:
accessionNumber: 0001321655-25-000105
filingDate: 2025-08-04
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-04T20:07:52.000Z
form: 8-K
items: 2.02,7.01,9.01
row 43:
accessionNumber: 0000002488-25-000106
filingDate: 2025-08-05
reportDate: 2025-08-05
acceptanceDateTime: 2025-08-05T20:16:31.000Z
form: 8-K
items: 2.02,7.01,9.01
row 44:
accessionNumber: 0001045810-25-000197
filingDate: 2025-08-05
reportDate: 2025-07-31
acceptanceDateTime: 2025-08-05T20:31:08.000Z
form: 8-K
items: 5.02
row 45:
accessionNumber: 0000059478-25-000202
filingDate: 2025-08-07
reportDate: 2025-08-07
acceptanceDateTime: 2025-08-07T11:05:40.000Z
form: 8-K
items: 2.02,9.01
row 46:
accessionNumber: 0000909832-25-000064
filingDate: 2025-08-07
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-07T20:35:32.000Z
form: 8-K
items: 5.02
row 47:
accessionNumber: 0001403161-25-000055
filingDate: 2025-08-08
reportDate: 2025-08-08
acceptanceDateTime: 2025-08-08T20:07:08.000Z
form: 8-K
items: 3.02
row 48:
accessionNumber: 0001104659-25-075940
filingDate: 2025-08-11
reportDate: 2025-08-11
acceptanceDateTime: 2025-08-11T12:05:18.000Z
form: 8-K
items: 7.01,9.01
row 49:
accessionNumber: 0001193125-25-179820
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:11:01.000Z
form: 8-K
items: 2.02,9.01
row 50:
accessionNumber: 0001193125-25-179846
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:16:58.000Z
form: 8-K
items: 8.01,9.01
row 51:
accessionNumber: 0000080424-25-000111
filingDate: 2025-08-14
reportDate: 2025-08-14
acceptanceDateTime: 2025-08-14T14:00:31.000Z
form: 8-K
items: 5.02
row 52:
accessionNumber: 0000731766-25-000239
filingDate: 2025-08-20
reportDate: 2025-08-20
acceptanceDateTime: 2025-08-20T20:06:17.000Z
form: 8-K
items: 7.01
row 53:
accessionNumber: 0001193125-25-184093
filingDate: 2025-08-20
reportDate: 2025-08-18
acceptanceDateTime: 2025-08-20T20:16:08.000Z
form: 8-K
items: 8.01,9.01
row 54:
accessionNumber: 0000104169-25-000120
filingDate: 2025-08-21
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-21T10:59:09.000Z
form: 8-K
items: 2.02,9.01
row 55:
accessionNumber: 0000002488-25-000147
filingDate: 2025-08-25
reportDate: 2025-08-22
acceptanceDateTime: 2025-08-25T20:07:00.000Z
form: 8-K
items: 5.02
row 56:
accessionNumber: 0000858877-25-000103
filingDate: 2025-08-25
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-25T20:27:47.000Z
form: 8-K
items: 5.03,9.01
row 57:
accessionNumber: 0001045810-25-000207
filingDate: 2025-08-27
reportDate: 2025-08-27
acceptanceDateTime: 2025-08-27T20:22:14.000Z
form: 8-K
items: 2.02,9.01
row 58:
accessionNumber: 0001652044-25-000067
filingDate: 2025-09-03
reportDate: 2025-09-02
acceptanceDateTime: 2025-09-03T20:30:34.000Z
form: 8-K
items: 8.01
row 59:
accessionNumber: 0001730168-25-000094
filingDate: 2025-09-04
reportDate: 2025-09-04
acceptanceDateTime: 2025-09-04T20:19:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 60:
accessionNumber: 0000104169-25-000143
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:07:39.000Z
form: 8-K
items: 8.01
row 61:
accessionNumber: 0001104659-25-087862
filingDate: 2025-09-05
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-05T20:46:03.000Z
form: 8-K
items: 1.01,9.01
row 62:
accessionNumber: 0001652044-25-000074
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:53:32.000Z
form: 8-K
items: 8.01
row 63:
accessionNumber: 0000731766-25-000245
filingDate: 2025-09-08
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T11:00:14.000Z
form: 8-K
items: 7.01
row 64:
accessionNumber: 0000200406-25-000190
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T23:55:25.000Z
form: 8-K
items: 5.02
row 65:
accessionNumber: 0000731766-25-000247
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-09T11:00:13.000Z
form: 8-K/A
items: 7.01
row 66:
accessionNumber: 0001193125-25-199175
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:13:19.000Z
form: 8-K
items: 2.02,8.01,9.01
row 67:
accessionNumber: 0000310158-25-000047
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:33:09.000Z
form: 8-K
items: 8.01,9.01
row 68:
accessionNumber: 0001193125-25-199281
filingDate: 2025-09-09
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-09T21:28:00.000Z
form: 8-K
items: 5.02,9.01
row 69:
accessionNumber: 0001193125-25-200108
filingDate: 2025-09-10
reportDate: 2025-09-10
acceptanceDateTime: 2025-09-10T20:16:49.000Z
form: 8-K
items: 8.01,9.01
row 70:
accessionNumber: 0001104659-25-089245
filingDate: 2025-09-11
reportDate: 2025-09-11
acceptanceDateTime: 2025-09-11T11:30:54.000Z
form: 8-K
items: 7.01,9.01
row 71:
accessionNumber: 0000019617-25-000907
filingDate: 2025-09-12
reportDate: 2025-09-12
acceptanceDateTime: 2025-09-12T20:32:01.000Z
form: 8-K
items: 5.03,9.01
row 72:
accessionNumber: 0000104169-25-000151
filingDate: 2025-09-19
reportDate: 2025-09-19
acceptanceDateTime: 2025-09-19T20:04:09.000Z
form: 8-K
items: 8.01
row 73:
accessionNumber: 0001403161-25-000058
filingDate: 2025-09-19
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-19T20:08:17.000Z
form: 8-K
items: 8.01
row 74:
accessionNumber: 0001193125-25-210089
filingDate: 2025-09-22
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-22T12:22:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 75:
accessionNumber: 0000104169-25-000153
filingDate: 2025-09-22
reportDate: 2025-09-22
acceptanceDateTime: 2025-09-22T20:39:22.000Z
form: 8-K
items: 8.01
row 76:
accessionNumber: 0000723125-25-000024
filingDate: 2025-09-23
reportDate: 2025-09-23
acceptanceDateTime: 2025-09-23T20:02:28.000Z
form: 8-K
items: 2.02,9.01
row 77:
accessionNumber: 0000093410-25-000098
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T12:00:43.000Z
form: 8-K
items: 7.01
row 78:
accessionNumber: 0000909832-25-000093
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T20:16:57.000Z
form: 8-K
items: 2.02,9.01
row 79:
accessionNumber: 0001193125-25-220445
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:05:13.000Z
form: 8-K
items: 8.01,9.01
row 80:
accessionNumber: 0001403161-25-000061
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:12:37.000Z
form: 8-K
items: 8.01
row 81:
accessionNumber: 0001403161-25-000064
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:06:58.000Z
form: 8-K
items: 5.02,9.01
row 82:
accessionNumber: 0001193125-25-223202
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:08:40.000Z
form: 8-K
items: 8.01,9.01
row 83:
accessionNumber: 0001193125-25-225125
filingDate: 2025-09-30
reportDate: 2025-09-24
acceptanceDateTime: 2025-09-30T20:37:10.000Z
form: 8-K
items: 5.02
row 84:
accessionNumber: 0001628280-25-043530
filingDate: 2025-10-02
reportDate: 2025-10-02
acceptanceDateTime: 2025-10-02T13:04:54.000Z
form: 8-K
items: 2.02,9.01
row 85:
accessionNumber: 0001193125-25-229405
filingDate: 2025-10-03
reportDate: 2025-09-30
acceptanceDateTime: 2025-10-03T14:34:37.000Z
form: 8-K
items: 5.03,9.01
row 86:
accessionNumber: 0001551152-25-000043
filingDate: 2025-10-03
reportDate: 2025-10-03
acceptanceDateTime: 2025-10-03T20:09:03.000Z
form: 8-K
items: 2.02,9.01
row 87:
accessionNumber: 0001193125-25-230895
filingDate: 2025-10-06
reportDate: 2025-10-05
acceptanceDateTime: 2025-10-06T11:04:49.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 88:
accessionNumber: 0001193125-25-231901
filingDate: 2025-10-06
reportDate: 2025-09-18
acceptanceDateTime: 2025-10-06T20:15:26.000Z
form: 8-K/A
items: 5.02
row 89:
accessionNumber: 0001628280-25-044845
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T10:30:57.000Z
form: 8-K
items: 2.02,9.01
row 90:
accessionNumber: 0000200406-25-000201
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T11:22:58.000Z
form: 8-K
items: 2.02,8.01,9.01
row 91:
accessionNumber: 0001628280-25-044887
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T13:49:09.000Z
form: 8-K
items: 7.01,9.01
row 92:
accessionNumber: 0000080424-25-000217
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T14:55:51.000Z
form: 8-K
items: 7.01,9.01
row 93:
accessionNumber: 0000909832-25-000105
filingDate: 2025-10-15
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-15T20:30:30.000Z
form: 8-K
items: 8.01,9.01
row 94:
accessionNumber: 0000080424-25-000235
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:25:14.000Z
form: 8-K
items: 5.02,5.07,9.01
row 95:
accessionNumber: 0001628280-25-045223
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:35:16.000Z
form: 8-K
items: 5.02,9.01
row 96:
accessionNumber: 0000858877-25-000145
filingDate: 2025-10-17
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-17T20:13:47.000Z
form: 8-K
items: 5.02
row 97:
accessionNumber: 0000909832-25-000107
filingDate: 2025-10-20
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-20T21:00:26.000Z
form: 8-K
items: 5.02,9.01
row 98:
accessionNumber: 0001628280-25-045577
filingDate: 2025-10-21
reportDate: 2025-10-21
acceptanceDateTime: 2025-10-21T10:59:07.000Z
form: 8-K
items: 2.02,9.01
row 99:
accessionNumber: 0001104659-25-101237
filingDate: 2025-10-21
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-21T20:09:06.000Z
form: 8-K
items: 5.02,9.01
row 100:
accessionNumber: 0001628280-25-045861
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:06:36.000Z
form: 8-K
items: 2.02,9.01
row 101:
accessionNumber: 0001193125-25-246803
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:17:53.000Z
form: 8-K
items: 8.01,9.01
row 102:
accessionNumber: 0000104169-25-000168
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:20:22.000Z
form: 8-K
items: 5.02
row 103:
accessionNumber: 0000080424-25-000240
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T11:04:27.000Z
form: 8-K
items: 2.02,9.01
row 104:
accessionNumber: 0000080424-25-000243
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T14:10:46.000Z
form: 8-K
items: 7.01,9.01
row 105:
accessionNumber: 0001193125-25-250803
filingDate: 2025-10-27
reportDate: 2025-10-27
acceptanceDateTime: 2025-10-27T12:49:27.000Z
form: 8-K
items: 2.01,7.01,9.01
row 106:
accessionNumber: 0000731766-25-000301
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T10:02:08.000Z
form: 8-K
items: 2.02,9.01
row 107:
accessionNumber: 0001403161-25-000077
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T20:06:03.000Z
form: 8-K
items: 2.02,8.01,9.01
row 108:
accessionNumber: 0001652044-25-000087
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:01:48.000Z
form: 8-K
items: 2.02,9.01
row 109:
accessionNumber: 0001193125-25-256310
filingDate: 2025-10-29
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-29T20:07:42.000Z
form: 8-K
items: 2.02,7.01,9.01
row 110:
accessionNumber: 0001628280-25-047114
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:08:34.000Z
form: 8-K
items: 2.02,9.01
row 111:
accessionNumber: 0001104659-25-103974
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T10:40:38.000Z
form: 8-K
items: 2.02,9.01
row 112:
accessionNumber: 0000059478-25-000251
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T11:03:41.000Z
form: 8-K
items: 2.02,9.01
row 113:
accessionNumber: 0001141391-25-000191
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T12:03:18.000Z
form: 8-K
items: 2.02,9.01
row 114:
accessionNumber: 0001018724-25-000121
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 115:
accessionNumber: 0000320193-25-000077
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:30:35.000Z
form: 8-K
items: 2.02,9.01
row 116:
accessionNumber: 0000093410-25-000103
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T10:16:33.000Z
form: 8-K
items: 2.02,9.01
row 117:
accessionNumber: 0001551152-25-000047
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T11:51:43.000Z
form: 8-K
items: 2.02,9.01
row 118:
accessionNumber: 0000093410-25-000105
filingDate: 2025-11-03
reportDate: 2025-10-29
acceptanceDateTime: 2025-11-03T13:11:08.000Z
form: 8-K
items: 5.02
row 119:
accessionNumber: 0001193125-25-262260
filingDate: 2025-11-03
reportDate: 2025-11-01
acceptanceDateTime: 2025-11-03T18:48:34.000Z
form: 8-K
items: 2.02,9.01
row 120:
accessionNumber: 0001321655-25-000130
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:06:20.000Z
form: 8-K
items: 2.02,7.01,9.01
row 121:
accessionNumber: 0001193125-25-262593
filingDate: 2025-11-03
reportDate: 2025-10-30
acceptanceDateTime: 2025-11-03T21:18:13.000Z
form: 8-K
items: 8.01,9.01
row 122:
accessionNumber: 0001193125-25-262609
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:23:10.000Z
form: 8-K
items: 8.01,9.01
row 123:
accessionNumber: 0001193125-25-264728
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:00.000Z
form: 8-K
items: 8.01,9.01
row 124:
accessionNumber: 0000002488-25-000163
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:10.000Z
form: 8-K
items: 2.02,7.01,9.01
row 125:
accessionNumber: 0001193125-25-269979
filingDate: 2025-11-06
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-06T21:47:26.000Z
form: 8-K
items: 8.01,9.01
row 126:
accessionNumber: 0000731766-25-000308
filingDate: 2025-11-07
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-07T21:13:36.000Z
form: 8-K
items: 7.01
row 127:
accessionNumber: 0001104659-25-108507
filingDate: 2025-11-07
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-07T21:27:23.000Z
form: 8-K
items: 5.02,5.07,9.01
row 128:
accessionNumber: 0001403161-25-000093
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:30:43.000Z
form: 8-K
items: 8.01,9.01
row 129:
accessionNumber: 0001141391-25-000197
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:31:40.000Z
form: 8-K
items: 8.01,9.01
row 130:
accessionNumber: 0001193125-25-277624
filingDate: 2025-11-12
reportDate: 2025-11-12
acceptanceDateTime: 2025-11-12T21:15:30.000Z
form: 8-K
items: 2.02,9.01
row 131:
accessionNumber: 0001141391-25-000199
filingDate: 2025-11-12
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-12T22:15:17.000Z
form: 8-K
items: 1.01
row 132:
accessionNumber: 0000731766-25-000310
filingDate: 2025-11-13
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-13T21:02:22.000Z
form: 8-K
items: 5.03
row 133:
accessionNumber: 0000104169-25-000172
filingDate: 2025-11-14
reportDate: 2025-11-11
acceptanceDateTime: 2025-11-14T13:00:30.000Z
form: 8-K
items: 5.02,9.01
row 134:
accessionNumber: 0001045810-25-000228
filingDate: 2025-11-19
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-19T21:20:44.000Z
form: 8-K
items: 2.02,9.01
row 135:
accessionNumber: 0000104169-25-000177
filingDate: 2025-11-20
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-20T11:58:46.000Z
form: 8-K
items: 2.02,3.01,7.01,9.01
row 136:
accessionNumber: 0001104659-25-114647
filingDate: 2025-11-20
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-20T22:00:42.000Z
form: 8-K
items: 8.01,9.01
row 137:
accessionNumber: 0001193125-25-290864
filingDate: 2025-11-21
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-21T15:46:21.000Z
form: 8-K
items: 8.01,9.01
row 138:
accessionNumber: 0000059478-25-000271
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:19:05.000Z
form: 8-K
items: 5.02
row 139:
accessionNumber: 0001193125-25-291441
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:26:49.000Z
form: 8-K
items: 5.02,5.07,9.01
row 140:
accessionNumber: 0000731766-25-000314
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T22:20:04.000Z
form: 8-K
items: 5.02
row 141:
accessionNumber: 0001628280-25-055388
filingDate: 2025-12-04
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-04T21:36:38.000Z
form: 8-K
items: 8.01,9.01
row 142:
accessionNumber: 0000093410-25-000122
filingDate: 2025-12-05
reportDate: 2025-12-03
acceptanceDateTime: 2025-12-05T21:21:15.000Z
form: 8-K
items: 5.03,8.01,9.01
row 143:
accessionNumber: 0001140361-25-044561
filingDate: 2025-12-05
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-05T21:31:42.000Z
form: 8-K
items: 5.02
row 144:
accessionNumber: 0000019617-25-001100
filingDate: 2025-12-08
reportDate: 2025-12-07
acceptanceDateTime: 2025-12-08T11:30:37.000Z
form: 8-K
items: 5.02
row 145:
accessionNumber: 0001193125-25-311196
filingDate: 2025-12-08
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-08T21:00:35.000Z
form: 8-K
items: 5.02,5.07
row 146:
accessionNumber: 0001193125-25-312771
filingDate: 2025-12-09
reportDate: 2025-12-09
acceptanceDateTime: 2025-12-09T21:18:53.000Z
form: 8-K
items: 8.01,9.01
row 147:
accessionNumber: 0001193125-25-314207
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T21:14:38.000Z
form: 8-K
items: 2.02,8.01,9.01
row 148:
accessionNumber: 0001552781-25-000454
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T22:19:43.000Z
form: 8-K
items: 5.02,9.01
row 149:
accessionNumber: 0001193125-25-314935
filingDate: 2025-12-11
reportDate: 2025-12-08
acceptanceDateTime: 2025-12-11T11:02:16.000Z
form: 8-K
items: 5.02,9.01
row 150:
accessionNumber: 0001730168-25-000116
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:17:37.000Z
form: 8-K
items: 2.02,8.01,9.01
row 151:
accessionNumber: 0000909832-25-000164
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:22:04.000Z
form: 8-K
items: 2.02,9.01
row 152:
accessionNumber: 0001628280-25-056768
filingDate: 2025-12-12
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-12T21:14:29.000Z
form: 8-K
items: 8.01,9.01
row 153:
accessionNumber: 0000080424-25-000287
filingDate: 2025-12-15
reportDate: 2025-12-15
acceptanceDateTime: 2025-12-15T14:15:22.000Z
form: 8-K
items: 5.02
row 154:
accessionNumber: 0000002488-25-000182
filingDate: 2025-12-15
reportDate: 2025-12-12
acceptanceDateTime: 2025-12-15T21:12:11.000Z
form: 8-K
items: 5.02,9.01
row 155:
accessionNumber: 0000723125-25-000044
filingDate: 2025-12-17
reportDate: 2025-12-17
acceptanceDateTime: 2025-12-17T21:03:26.000Z
form: 8-K
items: 2.02,9.01
row 156:
accessionNumber: 0000858877-25-000199
filingDate: 2025-12-17
reportDate: 2025-12-16
acceptanceDateTime: 2025-12-17T21:42:08.000Z
form: 8-K
items: 5.02,5.07,9.01
row 157:
accessionNumber: 0000093410-25-000130
filingDate: 2025-12-19
reportDate: 2025-07-28
acceptanceDateTime: 2025-12-19T21:25:35.000Z
form: 8-K/A
items: 5.02
row 158:
accessionNumber: 0001628280-25-058337
filingDate: 2025-12-19
reportDate: 2025-12-19
acceptanceDateTime: 2025-12-19T22:00:37.000Z
form: 8-K
items: 5.02
row 159:
accessionNumber: 0001403161-25-000134
filingDate: 2025-12-23
reportDate: 2025-12-23
acceptanceDateTime: 2025-12-23T21:06:56.000Z
form: 8-K
items: 8.01
row 160:
accessionNumber: 0000104169-25-000238
filingDate: 2025-12-29
reportDate: 2025-12-24
acceptanceDateTime: 2025-12-29T21:40:38.000Z
form: 8-K
items: 8.01
row 161:
accessionNumber: 0001403161-25-000137
filingDate: 2025-12-30
reportDate: 2025-12-30
acceptanceDateTime: 2025-12-30T21:07:17.000Z
form: 8-K
items: 8.01
row 162:
accessionNumber: 0001628280-26-000016
filingDate: 2026-01-02
reportDate: 2026-01-02
acceptanceDateTime: 2026-01-02T14:20:13.000Z
form: 8-K
items: 2.02,9.01
row 163:
accessionNumber: 0001140361-26-000199
filingDate: 2026-01-02
reportDate: 2025-12-30
acceptanceDateTime: 2026-01-02T21:30:52.000Z
form: 8-K
items: 5.02
row 164:
accessionNumber: 0001193125-26-004727
filingDate: 2026-01-06
reportDate: 2025-05-03
acceptanceDateTime: 2026-01-06T22:00:33.000Z
form: 8-K/A
items: 5.02
row 165:
accessionNumber: 0001551152-26-000002
filingDate: 2026-01-07
reportDate: 2026-01-07
acceptanceDateTime: 2026-01-07T21:08:59.000Z
form: 8-K
items: 2.02,9.01
row 166:
accessionNumber: 0000104169-26-000008
filingDate: 2026-01-08
reportDate: 2026-01-08
acceptanceDateTime: 2026-01-08T12:59:51.000Z
form: 8-K
items: 5.02,9.01
row 167:
accessionNumber: 0001193125-26-009002
filingDate: 2026-01-09
reportDate: 2026-01-05
acceptanceDateTime: 2026-01-09T21:31:11.000Z
form: 8-K
items: 5.02
row 168:
accessionNumber: 0000731766-26-000020
filingDate: 2026-01-12
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-12T11:58:08.000Z
form: 8-K
items: 7.01
row 169:
accessionNumber: 0001628280-26-001902
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T11:41:09.000Z
form: 8-K
items: 2.02,9.01
row 170:
accessionNumber: 0001628280-26-001915
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T15:09:19.000Z
form: 8-K
items: 7.01,9.01
row 171:
accessionNumber: 0001193125-26-011731
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:06:00.000Z
form: 8-K
items: 8.01,9.01
row 172:
accessionNumber: 0000080424-26-000002
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:27:59.000Z
form: 8-K
items: 7.01,9.01
row 173:
accessionNumber: 0001552781-26-000017
filingDate: 2026-01-14
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-14T11:58:41.000Z
form: 8-K
items: 5.02,9.01
row 174:
accessionNumber: 0000104169-26-000023
filingDate: 2026-01-16
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-16T14:01:15.000Z
form: 8-K
items: 5.02,9.01
row 175:
accessionNumber: 0000104169-26-000024
filingDate: 2026-01-16
reportDate: 2025-11-13
acceptanceDateTime: 2026-01-16T14:03:05.000Z
form: 8-K/A
items: 5.02
row 176:
accessionNumber: 0001628280-26-002429
filingDate: 2026-01-16
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-16T21:56:58.000Z
form: 8-K
items: 5.02
row 177:
accessionNumber: 0000002488-26-000002
filingDate: 2026-01-20
reportDate: 2026-01-16
acceptanceDateTime: 2026-01-20T21:19:32.000Z
form: 8-K
items: 5.02,9.01
row 178:
accessionNumber: 0000200406-26-000002
filingDate: 2026-01-21
reportDate: 2026-01-21
acceptanceDateTime: 2026-01-21T12:46:18.000Z
form: 8-K
items: 2.02,9.01
row 179:
accessionNumber: 0001104659-26-005366
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:05:37.000Z
form: 8-K
items: 5.03,5.07,9.01
row 180:
accessionNumber: 0000909832-26-000016
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:16:10.000Z
form: 8-K
items: 5.07,8.01
row 181:
accessionNumber: 0000080424-26-000006
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T12:02:05.000Z
form: 8-K
items: 2.02,9.01
row 182:
accessionNumber: 0000080424-26-000009
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T16:53:22.000Z
form: 8-K
items: 7.01,9.01
row 183:
accessionNumber: 0001193125-26-019450
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T21:15:33.000Z
form: 8-K
items: 8.01,9.01
row 184:
accessionNumber: 0000019617-26-000052
filingDate: 2026-01-22
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-22T21:30:18.000Z
form: 8-K
items: 5.02
row 185:
accessionNumber: 0001045810-26-000003
filingDate: 2026-01-23
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-23T22:01:33.000Z
form: 8-K
items: 5.02
row 186:
accessionNumber: 0000731766-26-000025
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T11:02:29.000Z
form: 8-K
items: 2.02,9.01
row 187:
accessionNumber: 0000093410-26-000010
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T21:45:32.000Z
form: 8-K
items: 5.02
row 188:
accessionNumber: 0001628280-26-003832
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:20.000Z
form: 8-K
items: 2.02,9.01
row 189:
accessionNumber: 0001193125-26-027198
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:38.000Z
form: 8-K
items: 2.02,9.01
row 190:
accessionNumber: 0001628280-26-003837
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:11:04.000Z
form: 8-K
items: 2.02,9.01
row 191:
accessionNumber: 0001403161-26-000029
filingDate: 2026-01-28
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-28T21:43:36.000Z
form: 8-K
items: 5.03,5.07
row 192:
accessionNumber: 0001141391-26-000003
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T13:03:21.000Z
form: 8-K
items: 2.02,9.01
row 193:
accessionNumber: 0001403161-26-000044
filingDate: 2026-01-29
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-29T21:05:49.000Z
form: 8-K
items: 2.02,8.01,9.01
row 194:
accessionNumber: 0000320193-26-000005
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T21:30:33.000Z
form: 8-K
items: 2.02,9.01
row 195:
accessionNumber: 0000093410-26-000019
filingDate: 2026-01-30
reportDate: 2026-01-30
acceptanceDateTime: 2026-01-30T11:16:19.000Z
form: 8-K
items: 2.02,9.01
row 196:
accessionNumber: 0000104169-26-000028
filingDate: 2026-01-30
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-30T21:10:02.000Z
form: 8-K/A
items: 5.02
row 197:
accessionNumber: 0000093410-26-000021
filingDate: 2026-01-30
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-30T21:30:32.000Z
form: 8-K
items: 5.02
row 198:
accessionNumber: 0001321655-26-000004
filingDate: 2026-02-02
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-02T21:06:08.000Z
form: 8-K
items: 2.02,7.01,9.01
row 199:
accessionNumber: 0001104659-26-009495
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T11:38:40.000Z
form: 8-K
items: 2.02,9.01
row 200:
accessionNumber: 0000002488-26-000014
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T21:16:18.000Z
form: 8-K
items: 2.02,7.01,9.01
row 201:
accessionNumber: 0000059478-26-000008
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:05:22.000Z
form: 8-K
items: 2.02,9.01
row 202:
accessionNumber: 0001551152-26-000004
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:54:33.000Z
form: 8-K
items: 2.02,9.01
row 203:
accessionNumber: 0001652044-26-000012
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T21:01:37.000Z
form: 8-K
items: 2.02,9.01
row 204:
accessionNumber: 0001193125-26-037840
filingDate: 2026-02-04
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-04T22:20:31.000Z
form: 8-K
items: 1.01,8.01,9.01
row 205:
accessionNumber: 0001193125-26-039344
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:01:31.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 206:
accessionNumber: 0001141391-26-000006
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:04:53.000Z
form: 8-K
items: 5.02
row 207:
accessionNumber: 0001193125-26-039427
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:17:31.000Z
form: 8-K
items: 8.01,9.01
row 208:
accessionNumber: 0001018724-26-000002
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:25:12.000Z
form: 8-K
items: 2.02,9.01
row 209:
accessionNumber: 0001628280-26-006642
filingDate: 2026-02-10
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-10T11:59:38.000Z
form: 8-K
items: 2.02,9.01
row 210:
accessionNumber: 0000858877-26-000006
filingDate: 2026-02-11
reportDate: 2026-02-11
acceptanceDateTime: 2026-02-11T21:07:20.000Z
form: 8-K
items: 2.02,9.01
row 211:
accessionNumber: 0001628280-26-007709
filingDate: 2026-02-12
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-12T21:30:37.000Z
form: 8-K
items: 8.01,9.01
row 212:
accessionNumber: 0001403161-26-000049
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T13:45:50.000Z
form: 8-K
items: 7.01
row 213:
accessionNumber: 0001193125-26-051423
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T21:16:46.000Z
form: 8-K
items: 8.01,9.01
row 214:
accessionNumber: 0000002488-26-000029
filingDate: 2026-02-17
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-17T21:21:24.000Z
form: 8-K
items: 5.02
row 215:
accessionNumber: 0000104169-26-000032
filingDate: 2026-02-19
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-19T11:59:55.000Z
form: 8-K
items: 2.02,9.01
row 216:
accessionNumber: 0001628280-26-010052
filingDate: 2026-02-20
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-20T15:10:16.000Z
form: 8-K
items: 5.02,9.01
row 217:
accessionNumber: 0001628280-26-010693
filingDate: 2026-02-23
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-23T21:39:11.000Z
form: 8-K
items: 7.01,9.01
row 218:
accessionNumber: 0000002488-26-000045
filingDate: 2026-02-24
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-24T12:01:06.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 219:
accessionNumber: 0001140361-26-006577
filingDate: 2026-02-24
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-24T21:55:58.000Z
form: 8-K
items: 5.07,9.01
row 220:
accessionNumber: 0000731766-26-000046
filingDate: 2026-02-25
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-25T11:23:37.000Z
form: 8-K
items: 5.02
row 221:
accessionNumber: 0001045810-26-000019
filingDate: 2026-02-25
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-25T21:31:25.000Z
form: 8-K
items: 2.02,9.01
row 222:
accessionNumber: 0001104659-26-020643
filingDate: 2026-02-26
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-26T22:14:40.000Z
form: 8-K
items: 8.01,9.01
row 223:
accessionNumber: 0001104659-26-021050
filingDate: 2026-02-27
reportDate: 2026-02-27
acceptanceDateTime: 2026-02-27T13:36:30.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 224:
accessionNumber: 0001403161-26-000063
filingDate: 2026-02-27
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-27T21:06:59.000Z
form: 8-K
items: 8.01
row 225:
accessionNumber: 0000731766-26-000064
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T14:21:03.000Z
form: 8-K
items: 5.02
row 226:
accessionNumber: 0001193125-26-085656
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T22:00:50.000Z
form: 8-K
items: 5.02
row 227:
accessionNumber: 0001193125-26-085801
filingDate: 2026-03-02
reportDate: 2026-02-28
acceptanceDateTime: 2026-03-02T22:27:20.000Z
form: 8-K
items: 2.02,9.01
row 228:
accessionNumber: 0001730168-26-000011
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:16:10.000Z
form: 8-K
items: 2.02,8.01,9.01
row 229:
accessionNumber: 0001104659-26-023534
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:59:47.000Z
form: 8-K
items: 8.01,9.01
row 230:
accessionNumber: 0001193125-26-092557
filingDate: 2026-03-05
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-05T12:25:35.000Z
form: 8-K
items: 8.01,9.01
row 231:
accessionNumber: 0000909832-26-000025
filingDate: 2026-03-05
reportDate: 2026-03-05
acceptanceDateTime: 2026-03-05T21:19:07.000Z
form: 8-K
items: 2.02,9.01
row 232:
accessionNumber: 0001045810-26-000024
filingDate: 2026-03-06
reportDate: 2026-03-02
acceptanceDateTime: 2026-03-06T21:11:25.000Z
form: 8-K
items: 5.02,9.01
row 233:
accessionNumber: 0001652044-26-000026
filingDate: 2026-03-06
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-06T22:21:44.000Z
form: 8-K
items: 5.02
row 234:
accessionNumber: 0000731766-26-000067
filingDate: 2026-03-09
reportDate: 2026-03-09
acceptanceDateTime: 2026-03-09T20:33:13.000Z
form: 8-K
items: 7.01
row 235:
accessionNumber: 0001193125-26-100148
filingDate: 2026-03-10
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-10T20:12:51.000Z
form: 8-K
items: 2.02,8.01,9.01
row 236:
accessionNumber: 0000104169-26-000057
filingDate: 2026-03-13
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-13T20:10:19.000Z
form: 8-K
items: 8.01
row 237:
accessionNumber: 0001104659-26-027729
filingDate: 2026-03-13
reportDate: 2026-03-13
acceptanceDateTime: 2026-03-13T21:01:35.000Z
form: 8-K
items: 8.01,9.01
row 238:
accessionNumber: 0001104659-26-028556
filingDate: 2026-03-16
reportDate: 2026-03-16
acceptanceDateTime: 2026-03-16T20:54:55.000Z
form: 8-K
items: 8.01,9.01
row 239:
accessionNumber: 0000723125-26-000004
filingDate: 2026-03-18
reportDate: 2026-03-18
acceptanceDateTime: 2026-03-18T20:02:14.000Z
form: 8-K
items: 2.02,9.01
row 240:
accessionNumber: 0001104659-26-034174
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T12:26:22.000Z
form: 8-K
items: 8.01,9.01
row 241:
accessionNumber: 0000093410-26-000103
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T20:36:44.000Z
form: 8-K
items: 5.03,9.01
row 242:
accessionNumber: 0000104169-26-000067
filingDate: 2026-03-27
reportDate: 2026-03-27
acceptanceDateTime: 2026-03-27T20:10:53.000Z
form: 8-K
items: 8.01
row 243:
accessionNumber: 0001104659-26-038249
filingDate: 2026-04-01
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-01T12:33:36.000Z
form: 8-K
items: 8.01,9.01
row 244:
accessionNumber: 0001628280-26-022956
filingDate: 2026-04-02
reportDate: 2026-04-02
acceptanceDateTime: 2026-04-02T13:07:13.000Z
form: 8-K
items: 2.02,9.01
row 245:
accessionNumber: 0001652044-26-000031
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T20:18:28.000Z
form: 8-K
items: 5.02
row 246:
accessionNumber: 0001193125-26-140574
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T21:25:00.000Z
form: 8-K
items: 5.02
row 247:
accessionNumber: 0001551152-26-000011
filingDate: 2026-04-03
reportDate: 2026-04-03
acceptanceDateTime: 2026-04-03T20:05:55.000Z
form: 8-K
items: 2.02,9.01
row 248:
accessionNumber: 0001193125-26-142939
filingDate: 2026-04-06
reportDate: 2026-04-01
acceptanceDateTime: 2026-04-06T12:12:11.000Z
form: 8-K
items: 5.02,7.01,9.01
row 249:
accessionNumber: 0000858877-26-000048
filingDate: 2026-04-06
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-06T20:29:18.000Z
form: 8-K
items: 5.02
row 250:
accessionNumber: 0001193125-26-144028
filingDate: 2026-04-06
reportDate: 2026-04-06
acceptanceDateTime: 2026-04-06T21:22:08.000Z
form: 8-K
items: 8.01
row 251:
accessionNumber: 0001104659-26-041034
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-08T22:02:20.000Z
form: 8-K
items: 7.01,9.01
row 252:
accessionNumber: 0000093410-26-000108
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-09T11:00:12.000Z
form: 8-K
items: 2.02
row 253:
accessionNumber: 0001652044-26-000034
filingDate: 2026-04-10
reportDate: 2026-04-07
acceptanceDateTime: 2026-04-10T20:16:53.000Z
form: 8-K
items: 5.02
row 254:
accessionNumber: 0001628280-26-024990
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T10:32:42.000Z
form: 8-K
items: 2.02,9.01
row 255:
accessionNumber: 0000200406-26-000076
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T11:35:25.000Z
form: 8-K
items: 2.02,8.01,9.01
row 256:
accessionNumber: 0001104659-26-042880
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T12:04:26.000Z
form: 8-K
items: 7.01,9.01
row 257:
accessionNumber: 0001628280-26-025013
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T14:05:26.000Z
form: 8-K
items: 7.01,9.01
row 258:
accessionNumber: 0000080424-26-000048
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T20:17:07.000Z
form: 8-K
items: 7.01,9.01
row 259:
accessionNumber: 0001628280-26-025108
filingDate: 2026-04-14
reportDate: 2026-04-08
acceptanceDateTime: 2026-04-14T21:01:31.000Z
form: 8-K
items: 5.02
row 260:
accessionNumber: 0000909832-26-000041
filingDate: 2026-04-15
reportDate: 2026-04-15
acceptanceDateTime: 2026-04-15T20:16:27.000Z
form: 8-K
items: 8.01,9.01
row 261:
accessionNumber: 0001193125-26-159326
filingDate: 2026-04-16
reportDate: 2026-04-16
acceptanceDateTime: 2026-04-16T21:15:36.000Z
form: 8-K
items: 8.01,9.01
row 262:
accessionNumber: 0001140361-26-015711
filingDate: 2026-04-20
reportDate: 2026-04-17
acceptanceDateTime: 2026-04-20T21:29:51.000Z
form: 8-K
items: 5.02
row 263:
accessionNumber: 0000731766-26-000121
filingDate: 2026-04-21
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-21T10:02:24.000Z
form: 8-K
items: 2.02,9.01
row 264:
accessionNumber: 0001730168-26-000039
filingDate: 2026-04-21
reportDate: 2026-04-20
acceptanceDateTime: 2026-04-21T20:37:02.000Z
form: 8-K
items: 5.07
row 265:
accessionNumber: 0001628280-26-026551
filingDate: 2026-04-22
reportDate: 2026-04-22
acceptanceDateTime: 2026-04-22T20:10:44.000Z
form: 8-K
items: 2.02,9.01
row 266:
accessionNumber: 0001193125-26-173739
filingDate: 2026-04-23
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-23T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 267:
accessionNumber: 0000080424-26-000056
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T11:01:47.000Z
form: 8-K
items: 2.02,9.01
row 268:
accessionNumber: 0000080424-26-000057
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T14:02:12.000Z
form: 8-K
items: 7.01,9.01
row 269:
accessionNumber: 0000019617-26-000119
filingDate: 2026-04-24
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-24T20:16:13.000Z
form: 8-K
items: 5.03
row 270:
accessionNumber: 0001045810-26-000026
filingDate: 2026-04-27
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-27T20:10:30.000Z
form: 8-K
items: 5.02
row 271:
accessionNumber: 0000200406-26-000089
filingDate: 2026-04-28
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-27T21:33:52.000Z
form: 8-K
items: 5.07,9.01
row 272:
accessionNumber: 0001628280-26-027723
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T11:00:30.000Z
form: 8-K
items: 2.02,9.01
row 273:
accessionNumber: 0001403161-26-000077
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T20:05:56.000Z
form: 8-K
items: 2.02,8.01,9.01
row 274:
accessionNumber: 0001551152-26-000013
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T11:50:28.000Z
form: 8-K
items: 2.02,9.01
row 275:
accessionNumber: 0001652044-26-000043
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:01:35.000Z
form: 8-K
items: 2.02,9.01
row 276:
accessionNumber: 0001193125-26-191457
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:03:31.000Z
form: 8-K
items: 2.02,9.01
row 277:
accessionNumber: 0001628280-26-028364
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:05:41.000Z
form: 8-K
items: 2.02,9.01
row 278:
accessionNumber: 0001018724-26-000012
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:18:55.000Z
form: 8-K
items: 2.02,9.01
row 279:
accessionNumber: 0001104659-26-052081
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T10:53:18.000Z
form: 8-K
items: 2.02,9.01
row 280:
accessionNumber: 0000059478-26-000043
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 281:
accessionNumber: 0001193125-26-194086
filingDate: 2026-04-30
reportDate: 2026-04-27
acceptanceDateTime: 2026-04-30T11:54:16.000Z
form: 8-K
items: 8.01,9.01
row 282:
accessionNumber: 0001141391-26-000029
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T12:03:33.000Z
form: 8-K
items: 2.02,9.01
row 283:
accessionNumber: 0000320193-26-000011
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T20:30:41.000Z
form: 8-K
items: 2.02,9.01
row 284:
accessionNumber: 0000093410-26-000110
filingDate: 2026-05-01
reportDate: 2026-05-01
acceptanceDateTime: 2026-05-01T10:16:43.000Z
form: 8-K
items: 2.02,9.01
row 285:
accessionNumber: 0001628280-26-029230
filingDate: 2026-05-01
reportDate: 2026-04-29
acceptanceDateTime: 2026-05-01T18:01:51.000Z
form: 8-K
items: 5.07
row 286:
accessionNumber: 0000858877-26-000057
filingDate: 2026-05-01
reportDate: 2026-04-27
acceptanceDateTime: 2026-05-01T20:05:06.000Z
form: 8-K
items: 5.02
row 287:
accessionNumber: 0001321655-26-000026
filingDate: 2026-05-04
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-04T20:06:32.000Z
form: 8-K
items: 2.02,7.01,9.01
row 288:
accessionNumber: 0001193125-26-204128
filingDate: 2026-05-04
reportDate: 2026-04-30
acceptanceDateTime: 2026-05-04T20:36:02.000Z
form: 8-K
items: 8.01,9.01
row 289:
accessionNumber: 0000002488-26-000072
filingDate: 2026-05-05
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-05T20:16:06.000Z
form: 8-K
items: 2.02,7.01,9.01
row 290:
accessionNumber: 0001193125-26-211978
filingDate: 2026-05-07
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-07T20:16:48.000Z
form: 8-K
items: 3.03,5.03,8.01,9.01
row 291:
accessionNumber: 0001141391-26-000034
filingDate: 2026-05-07
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-07T20:17:31.000Z
form: 8-K
items: 5.02,9.01
row 292:
accessionNumber: 0001193125-26-212148
filingDate: 2026-05-07
reportDate: 2026-05-02
acceptanceDateTime: 2026-05-07T20:33:34.000Z
form: 8-K
items: 2.02,5.02,5.03,5.07,9.01
row 293:
accessionNumber: 0000059478-26-000048
filingDate: 2026-05-07
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-07T20:41:48.000Z
form: 8-K
items: 5.07
row 294:
accessionNumber: 0001045810-26-000028
filingDate: 2026-05-08
reportDate: 2026-05-07
acceptanceDateTime: 2026-05-08T20:35:07.000Z
form: 8-K
items: 5.02
row 295:
accessionNumber: 0001193125-26-215875
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T13:10:25.000Z
form: 8-K
items: 7.01,9.01
row 296:
accessionNumber: 0001193125-26-216986
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T20:45:29.000Z
form: 8-K
items: 8.01,9.01
row 297:
accessionNumber: 0000731766-26-000129
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T21:28:55.000Z
form: 8-K
items: 7.01
row 298:
accessionNumber: 0001193125-26-219432
filingDate: 2026-05-12
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-12T20:11:02.000Z
form: 8-K
items: 1.01,8.01,9.01
row 299:
accessionNumber: 0001193125-26-219708
filingDate: 2026-05-12
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-12T20:50:49.000Z
form: 8-K
items: 5.02,7.01,9.01
row 300:
accessionNumber: 0001104659-26-059484
filingDate: 2026-05-12
reportDate: 2026-05-08
acceptanceDateTime: 2026-05-12T21:01:51.000Z
form: 8-K
items: 5.07
row 301:
accessionNumber: 0000858877-26-000075
filingDate: 2026-05-13
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-13T20:06:53.000Z
form: 8-K
items: 2.02,2.05,9.01
row 302:
accessionNumber: 0001193125-26-224155
filingDate: 2026-05-14
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-14T20:28:48.000Z
form: 8-K
items: 5.02,9.01
row 303:
accessionNumber: 0001193125-26-226746
filingDate: 2026-05-15
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-15T20:12:53.000Z
form: 8-K
items: 1.01,1.02,2.03,5.02,5.07,9.01
row 304:
accessionNumber: 0001045810-26-000051
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 305:
accessionNumber: 0001193125-26-232707
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:30:32.000Z
form: 8-K
items: 8.01,9.01
row 306:
accessionNumber: 0000104169-26-000095
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T10:59:53.000Z
form: 8-K
items: 2.02,9.01
row 307:
accessionNumber: 0000019617-26-000228
filingDate: 2026-05-21
reportDate: 2026-05-19
acceptanceDateTime: 2026-05-21T20:15:13.000Z
form: 8-K
items: 5.07
row 308:
accessionNumber: 0001193125-26-234488
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T20:25:10.000Z
form: 8-K
items: 8.01,9.01
row 309:
accessionNumber: 0001104659-26-065717
filingDate: 2026-05-22
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-22T20:12:53.000Z
form: 8-K
items: 5.07
row 310:
accessionNumber: 0001628280-26-037738
filingDate: 2026-05-22
reportDate: 2026-05-22
acceptanceDateTime: 2026-05-22T20:21:18.000Z
form: 8-K
items: 8.01,9.01
row 311:
accessionNumber: 0001193125-26-242018
filingDate: 2026-05-27
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-27T20:39:34.000Z
form: 8-K
items: 8.01,9.01
row 312:
accessionNumber: 0001104659-26-067509
filingDate: 2026-05-28
reportDate: 2026-05-26
acceptanceDateTime: 2026-05-28T20:15:25.000Z
form: 8-K
items: 5.07
row 313:
accessionNumber: 0000909832-26-000046
filingDate: 2026-05-28
reportDate: 2026-05-28
acceptanceDateTime: 2026-05-28T20:17:32.000Z
form: 8-K
items: 2.02,9.01
row 314:
accessionNumber: 0000093410-26-000123
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T13:13:55.000Z
form: 8-K
items: 5.02
row 315:
accessionNumber: 0000093410-26-000125
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T14:12:25.000Z
form: 8-K
items: 5.07
row 316:
accessionNumber: 0001628280-26-039193
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T20:16:13.000Z
form: 8-K
items: 5.07
row 317:
accessionNumber: 0001141391-26-000037
filingDate: 2026-06-02
reportDate: 2026-05-29
acceptanceDateTime: 2026-06-02T20:15:00.000Z
form: 8-K
items: 5.02,9.01
row 318:
accessionNumber: 0001193125-26-253533
filingDate: 2026-06-02
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-02T20:15:25.000Z
form: 8-K
items: 8.01,9.01
row 319:
accessionNumber: 0001730168-26-000051
filingDate: 2026-06-03
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-03T20:21:35.000Z
form: 8-K
items: 2.02,8.01,9.01
row 320:
accessionNumber: 0001193125-26-257724
filingDate: 2026-06-04
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-04T21:07:39.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 321:
accessionNumber: 0001193125-26-258667
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T14:36:56.000Z
form: 8-K
items: 5.02
row 322:
accessionNumber: 0000104169-26-000111
filingDate: 2026-06-05
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-05T20:07:36.000Z
form: 8-K
items: 5.03,5.07,9.01
row 323:
accessionNumber: 0000731766-26-000138
filingDate: 2026-06-05
reportDate: 2026-06-01
acceptanceDateTime: 2026-06-05T20:17:52.000Z
form: 8-K
items: 5.07
row 324:
accessionNumber: 0001652044-26-000059
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T20:40:20.000Z
form: 8-K
items: 5.02
row 325:
accessionNumber: 0001193125-26-259830
filingDate: 2026-06-05
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-05T20:52:38.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 326:
accessionNumber: 0001193125-26-261669
filingDate: 2026-06-08
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-08T20:02:24.000Z
form: 8-K
items: 8.01,9.01
row 327:
accessionNumber: 0001321655-26-000033
filingDate: 2026-06-09
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-09T20:05:18.000Z
form: 8-K
items: 5.07
row 328:
accessionNumber: 0001104659-26-071845
filingDate: 2026-06-09
reportDate: 2026-06-09
acceptanceDateTime: 2026-06-09T20:13:47.000Z
form: 8-K
items: 5.02,9.01
row 329:
accessionNumber: 0001104659-26-072140
filingDate: 2026-06-10
reportDate: 2026-06-08
acceptanceDateTime: 2026-06-10T13:00:19.000Z
form: 8-K
items: 1.01,2.03,9.01
row 330:
accessionNumber: 0001193125-26-265848
filingDate: 2026-06-10
reportDate: 2026-06-10
acceptanceDateTime: 2026-06-10T20:13:46.000Z
form: 8-K
items: 2.02,8.01,9.01
row 331:
accessionNumber: 0001193125-26-266777
filingDate: 2026-06-11
reportDate: 2026-06-11
acceptanceDateTime: 2026-06-11T13:07:29.000Z
form: 8-K
items: 8.01,9.01
row 332:
accessionNumber: 0001193125-26-267578
filingDate: 2026-06-11
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-11T20:17:04.000Z
form: 8-K
items: 5.02,5.07,9.01
row 333:
accessionNumber: 0001104659-26-073562
filingDate: 2026-06-12
reportDate: 2026-06-12
acceptanceDateTime: 2026-06-12T21:00:28.000Z
form: 8-K
items: 8.01,9.01
row 334:
accessionNumber: 0001141391-26-000041
filingDate: 2026-06-17
reportDate: 2026-06-16
acceptanceDateTime: 2026-06-17T20:04:44.000Z
form: 8-K
items: 5.07
row 335:
accessionNumber: 0001193125-26-275077
filingDate: 2026-06-18
reportDate: 2026-06-17
acceptanceDateTime: 2026-06-18T13:00:28.000Z
form: 8-K
items: 8.01,9.01
row 336:
accessionNumber: 0001193125-26-275783
filingDate: 2026-06-18
reportDate: 2026-06-15
acceptanceDateTime: 2026-06-18T20:00:24.000Z
form: 8-K
items: 8.01,9.01
row 337:
accessionNumber: 0001104659-26-076067
filingDate: 2026-06-22
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-22T11:11:21.000Z
form: 8-K
items: 7.01,9.01
row 338:
accessionNumber: 0000723125-26-000013
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:02:01.000Z
form: 8-K
items: 2.02,9.01
row 339:
accessionNumber: 0001628280-26-045167
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:06:40.000Z
form: 8-K
items: 8.01,9.01
row 340:
accessionNumber: 0001628280-26-045169
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:07:40.000Z
form: 8-K
items: 7.01,9.01
row 341:
accessionNumber: 0000019617-26-000241
filingDate: 2026-06-25
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-25T11:59:33.000Z
form: 8-K
items: 5.02
row 342:
accessionNumber: 0001552781-26-000366
filingDate: 2026-06-25
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-25T20:19:25.000Z
form: 8-K
items: 5.02,9.01
row 343:
accessionNumber: 0001403161-26-000086
filingDate: 2026-06-26
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-26T20:07:23.000Z
form: 8-K
items: 8.01
row 344:
accessionNumber: 0001045810-26-000056
filingDate: 2026-06-30
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-30T20:27:26.000Z
form: 8-K
items: 5.07
row 345:
accessionNumber: 0000002488-26-000115
filingDate: 2026-07-01
reportDate: 2026-06-26
acceptanceDateTime: 2026-07-01T20:27:26.000Z
form: 8-K
items: 5.02
row 346:
accessionNumber: 0001628280-26-046717
filingDate: 2026-07-02
reportDate: 2026-07-02
acceptanceDateTime: 2026-07-02T13:01:26.000Z
form: 8-K
items: 2.02,9.01
row 347:
accessionNumber: 0001045810-26-000060
filingDate: 2026-07-02
reportDate: 2026-06-28
acceptanceDateTime: 2026-07-02T13:23:16.000Z
form: 8-K
items: 5.02
row 348:
accessionNumber: 0001193125-26-295589
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T12:00:19.000Z
form: 8-K
items: 8.01
row 349:
accessionNumber: 0001551152-26-000021
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T20:12:09.000Z
form: 8-K
items: 2.02,9.01
row 350:
accessionNumber: 0002115436-26-000003
filingDate: 2026-07-07
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-07T20:19:57.000Z
form: 8-K
items: 7.01
row 351:
accessionNumber: 0000909832-26-000060
filingDate: 2026-07-08
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-08T20:18:27.000Z
form: 8-K
items: 8.01,9.01
row 352:
accessionNumber: 0001104659-26-082293
filingDate: 2026-07-09
reportDate: 2026-07-09
acceptanceDateTime: 2026-07-09T20:46:08.000Z
form: 8-K
items: 8.01,9.01
row 353:
accessionNumber: 0001628280-26-048078
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 354:
accessionNumber: 0001628280-26-048086
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T13:52:21.000Z
form: 8-K
items: 7.01,9.01
row 355:
accessionNumber: 0000080424-26-000082
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T20:19:08.000Z
form: 8-K
items: 7.01,9.01
row 356:
accessionNumber: 0000200406-26-000146
filingDate: 2026-07-15
reportDate: 2026-07-15
acceptanceDateTime: 2026-07-15T11:49:04.000Z
form: 8-K
items: 2.02,9.01
row 357:
accessionNumber: 0001403161-26-000096
filingDate: 2026-07-15
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-15T20:23:24.000Z
form: 8-K
items: 5.03,9.01
row 358:
accessionNumber: 0000731766-26-000191
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T10:00:59.000Z
form: 8-K
items: 2.02,9.01
row 359:
accessionNumber: 0001628280-26-048466
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T20:20:56.000Z
form: 8-K
items: 8.01
row 360:
accessionNumber: 0001652044-26-000066
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:01:36.000Z
form: 8-K
items: 2.02,9.01
row 361:
accessionNumber: 0001628280-26-049213
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:35:52.000Z
form: 8-K
items: 2.02,9.01
row 362:
accessionNumber: 0000019617-26-000288
filingDate: 2026-07-23
reportDate: 2026-07-21
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 5.03
row 363:
accessionNumber: 0001193125-26-314128
filingDate: 2026-07-23
reportDate: 2026-07-23
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 8.01,9.01
row 364:
accessionNumber: 0000200406-26-000155
filingDate: 2026-07-28
reportDate: 2026-07-27
acceptanceDateTime: 2026-07-28T00:15:31.000Z
form: 8-K
items: 7.01,9.01
row 365:
accessionNumber: 0001628280-26-049922
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 366:
accessionNumber: 0001403161-26-000103
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T20:05:26.000Z
form: 8-K
items: 2.02,8.01,9.01
row 367:
accessionNumber: 0000080424-26-000093
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:03:12.000Z
form: 8-K
items: 2.02,9.01
row 368:
accessionNumber: 0000080424-26-000094
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:05:06.000Z
form: 8-K
items: 5.02,7.01,9.01
row 369:
accessionNumber: 0000080424-26-000097
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T14:38:23.000Z
form: 8-K
items: 7.01,9.01
row 370:
accessionNumber: 0001628280-26-050596
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:03:23.000Z
form: 8-K
items: 2.02,9.01
row 371:
accessionNumber: 0001193125-26-323632
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:04:53.000Z
form: 8-K
items: 2.02,9.01
row 372:
accessionNumber: 0000200406-26-000163
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T21:25:05.000Z
form: 8-K
items: 7.01,9.01
row 373:
accessionNumber: 0001141391-26-000081
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T12:07:03.000Z
form: 8-K
items: 2.02,9.01
row 374:
accessionNumber: 0001018724-26-000024
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:06:23.000Z
form: 8-K
items: 2.02,9.01
row 375:
accessionNumber: 0000320193-26-000018
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:30:28.000Z
form: 8-K
items: 2.02,9.01
row 376:
accessionNumber: 0000093410-26-000162
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:16:46.000Z
form: 8-K
items: 2.02,9.01
row 377:
accessionNumber: 0002115436-26-000006
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:31:39.000Z
form: 8-K
items: 2.02,7.01
row 378:
accessionNumber: 0001551152-26-000023
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T11:51:32.000Z
form: 8-K
items: 2.02,9.01
row 379:
accessionNumber: 0001321655-26-000039
filingDate: 2026-08-03
reportDate: 2026-08-03
acceptanceDateTime: 2026-08-03T20:06:14.000Z
form: 8-K
items: 2.02,7.01,9.01
row 380:
accessionNumber: 0001104659-26-090045
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T10:47:58.000Z
form: 8-K
items: 2.02,9.01
row 381:
accessionNumber: 0000200406-26-000167
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T12:48:52.000Z
form: 8-K
items: 5.02,9.01
row 382:
accessionNumber: 0000002488-26-000121
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T20:16:24.000Z
form: 8-K
items: 2.02,7.01,9.01
row 383:
accessionNumber: 0000059478-26-000077
filingDate: 2026-08-05
reportDate: 2026-08-05
acceptanceDateTime: 2026-08-05T11:05:09.000Z
form: 8-K
items: 2.02,9.01
row 384:
accessionNumber: 0001104659-26-091269
filingDate: 2026-08-05
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-05T21:17:20.000Z
form: 8-K
items: 8.01,9.01
row 385:
accessionNumber: 0001193125-26-342390
filingDate: 2026-08-10
reportDate: 2026-08-10
acceptanceDateTime: 2026-08-10T20:10:48.000Z
form: 8-K
items: 8.01,9.01
row 386:
accessionNumber: 0001193125-26-344495
filingDate: 2026-08-11
reportDate: 2026-08-08
acceptanceDateTime: 2026-08-11T19:52:27.000Z
form: 8-K
items: 2.02,9.01
row 387:
accessionNumber: 0000858877-26-000106
filingDate: 2026-08-12
reportDate: 2026-08-12
acceptanceDateTime: 2026-08-12T20:07:06.000Z
form: 8-K
items: 2.02,9.01
row 388:
accessionNumber: 0001045810-26-000069
filingDate: 2026-08-17
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-17T12:41:33.000Z
form: 8-K
items: 1.01,2.03,7.01
row 389:
accessionNumber: 0001193125-26-354029
filingDate: 2026-08-17
reportDate: 2026-08-13
acceptanceDateTime: 2026-08-17T20:05:40.000Z
form: 8-K
items: 1.01,2.03,9.01
row 390:
accessionNumber: 0001104659-26-098367
filingDate: 2026-08-18
reportDate: 2026-08-18
acceptanceDateTime: 2026-08-18T20:30:26.000Z
form: 8-K
items: 8.01,9.01
row 391:
accessionNumber: 0000002488-26-000163
filingDate: 2026-08-19
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-19T20:16:56.000Z
form: 8-K
items: 5.02,9.01
row 392:
accessionNumber: 0000104169-26-000145
filingDate: 2026-08-20
reportDate: 2026-08-20
acceptanceDateTime: 2026-08-20T10:59:01.000Z
form: 8-K
items: 2.02,9.01
row 393:
accessionNumber: 0001104659-26-101067
filingDate: 2026-08-26
reportDate: 2026-08-24
acceptanceDateTime: 2026-08-26T12:06:55.000Z
form: 8-K
items: 5.02,9.01
row 394:
accessionNumber: 0001045810-26-000073
filingDate: 2026-08-26
reportDate: 2026-08-26
acceptanceDateTime: 2026-08-26T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 395:
accessionNumber: 0001193125-26-373026
filingDate: 2026-08-28
reportDate: 2026-08-28
acceptanceDateTime: 2026-08-28T15:26:26.000Z
form: 8-K
items: 8.01,9.01
row 396:
accessionNumber: 0001140361-26-035325
filingDate: 2026-09-01
reportDate: 2026-04-17
acceptanceDateTime: 2026-09-01T20:30:35.000Z
form: 8-K/A
items: 5.02
row 397:
accessionNumber: 0001730168-26-000076
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:26:04.000Z
form: 8-K
items: 2.02,8.01,9.01
row 398:
accessionNumber: 0001193125-26-380280
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:30:24.000Z
form: 8-K
items: 7.01,9.01
row 399:
accessionNumber: 0001045810-26-000078
filingDate: 2026-09-03
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-03T12:03:56.000Z
form: 8-K
items: 8.01
row 400:
accessionNumber: 0001104659-26-104940
filingDate: 2026-09-03
reportDate: 2026-09-03
acceptanceDateTime: 2026-09-03T12:47:46.000Z
form: 8-K
items: 7.01,9.01
row 401:
accessionNumber: 0000731766-26-000205
filingDate: 2026-09-08
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-08T20:04:56.000Z
form: 8-K
items: 7.01
row 402:
accessionNumber: 0001018724-26-000036
filingDate: 2026-09-09
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-09T20:28:21.000Z
form: 8-K
items: 5.02
row 403:
accessionNumber: 0001193125-26-387905
filingDate: 2026-09-10
reportDate: 2026-09-10
acceptanceDateTime: 2026-09-10T20:16:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 404:
accessionNumber: 0001193125-26-389753
filingDate: 2026-09-14
reportDate: 2026-09-12
acceptanceDateTime: 2026-09-14T10:01:59.000Z
form: 8-K
items: 8.01,9.01
row 405:
accessionNumber: 0001104659-26-107526
filingDate: 2026-09-14
reportDate: 2026-09-14
acceptanceDateTime: 2026-09-14T20:45:41.000Z
form: 8-K
items: 8.01,9.01
row 406:
accessionNumber: 0001403161-26-000121
filingDate: 2026-09-23
reportDate: 2026-09-18
acceptanceDateTime: 2026-09-23T20:06:31.000Z
form: 8-K
items: 8.01
row 407:
accessionNumber: 0000909832-26-000084
filingDate: 2026-09-24
reportDate: 2026-09-24
acceptanceDateTime: 2026-09-24T20:17:37.000Z
form: 8-K
items: 2.02,9.01
row 408:
accessionNumber: 0001193125-26-402986
filingDate: 2026-09-25
reportDate: 2026-09-25
acceptanceDateTime: 2026-09-25T21:20:49.000Z
form: 8-K
items: 8.01,9.01
row 409:
accessionNumber: 0000002488-26-000182
filingDate: 2026-09-28
reportDate: 2026-09-26
acceptanceDateTime: 2026-09-28T20:16:47.000Z
form: 8-K
items: 3.02
row 410:
accessionNumber: 0001628280-26-063820
filingDate: 2026-09-29
reportDate: 2026-09-29
acceptanceDateTime: 2026-09-29T20:38:50.000Z
form: 8-K
items: 1.01,1.02,2.03,9.01
row 411:
accessionNumber: 0000723125-26-000018
filingDate: 2026-09-30
reportDate: 2026-09-30
acceptanceDateTime: 2026-09-30T20:02:22.000Z
form: 8-K
items: 2.02,9.01
row 412:
accessionNumber: 0001628280-26-064366
filingDate: 2026-10-02
reportDate: 2026-10-02
acceptanceDateTime: 2026-10-02T13:04:26.000Z
form: 8-K
items: 2.02,9.01
row 413:
accessionNumber: 0000093410-26-000188
filingDate: 2026-10-05
reportDate: 2026-09-30
acceptanceDateTime: 2026-10-05T13:01:20.000Z
form: 8-K
items: 5.02
row 414:
accessionNumber: 0001551152-26-000030
filingDate: 2026-10-05
reportDate: 2026-10-05
acceptanceDateTime: 2026-10-05T20:07:45.000Z
form: 8-K
items: 2.02,9.01
row 415:
accessionNumber: 0000093410-26-000192
filingDate: 2026-10-06
reportDate: 2026-10-06
acceptanceDateTime: 2026-10-06T21:16:59.000Z
form: 8-K
items: 7.01,8.01,9.01
row 416:
accessionNumber: 0000858877-26-000156
filingDate: 2026-10-09
reportDate: 2026-10-07
acceptanceDateTime: 2026-10-09T20:08:49.000Z
form: 8-K
items: 5.02
row 417:
accessionNumber: 0000731766-26-000255
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:14:45.000Z
form: 8-K
items: 2.02,9.01
row 418:
accessionNumber: 0001628280-26-065582
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 419:
accessionNumber: 0000200406-26-000189
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T12:12:35.000Z
form: 8-K
items: 2.02,9.01
row 420:
accessionNumber: 0001628280-26-065616
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T13:38:53.000Z
form: 8-K
items: 7.01,9.01
row 421:
accessionNumber: 0000080424-26-000214
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T14:01:56.000Z
form: 8-K
items: 7.01,9.01
row 422:
accessionNumber: 0000310158-26-000237
filingDate: 2026-10-13
reportDate: 2026-10-09
acceptanceDateTime: 2026-10-13T16:36:57.000Z
form: 8-K
items: 5.02
row 423:
accessionNumber: 0000909832-26-000096
filingDate: 2026-10-14
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-14T20:16:05.000Z
form: 8-K
items: 8.01,9.01
row 424:
accessionNumber: 0001104659-26-116227
filingDate: 2026-10-15
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-15T20:00:53.000Z
form: 8-K
items: 5.02
row 425:
accessionNumber: 0002115436-26-000013
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T12:02:58.000Z
form: 8-K
items: 7.01
row 426:
accessionNumber: 0000080424-26-000245
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T20:25:47.000Z
form: 8-K
items: 5.07
row 427:
accessionNumber: 0000909832-26-000100
filingDate: 2026-10-16
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-16T20:52:57.000Z
form: 8-K
items: 5.02,9.01
row 428:
accessionNumber: 0001193125-26-426704
filingDate: 2026-10-20
reportDate: 2026-10-20
acceptanceDateTime: 2026-10-20T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 429:
accessionNumber: 0001628280-26-066700
filingDate: 2026-10-21
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-21T20:03:35.000Z
form: 8-K
items: 1.01,2.02,8.01,9.01
row 430:
accessionNumber: 0001628280-26-066738
filingDate: 2026-10-21
reportDate: 2026-10-21
acceptanceDateTime: 2026-10-21T20:41:42.000Z
form: 8-K
items: 2.02,9.01
row 431:
accessionNumber: 0000080424-26-000250
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T11:02:49.000Z
form: 8-K
items: 2.02,9.01
row 432:
accessionNumber: 0000080424-26-000252
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T14:29:34.000Z
form: 8-K
items: 7.01,9.01
row 433:
accessionNumber: 0001193125-26-429539
filingDate: 2026-10-23
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-23T13:04:03.000Z
form: 8-K
items: 8.01,9.01
row 434:
accessionNumber: 0001628280-26-067403
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 435:
accessionNumber: 0001403161-26-000126
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T20:05:22.000Z
form: 8-K
items: 2.02,8.01,9.01
row 436:
accessionNumber: 0001193125-26-434271
filingDate: 2026-10-27
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-27T20:23:36.000Z
form: 8-K
items: 2.03
row 437:
accessionNumber: 0001193125-26-435853
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T18:24:44.000Z
form: 8-K
items: 7.01,9.01
row 438:
accessionNumber: 0001652044-26-000080
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:01:33.000Z
form: 8-K
items: 2.02,9.01
row 439:
accessionNumber: 0001193125-26-436122
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:04:44.000Z
form: 8-K
items: 2.02,9.01
row 440:
accessionNumber: 0001193125-26-436149
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:11:03.000Z
form: 8-K
items: 8.01,9.01
row 441:
accessionNumber: 0001104659-26-119825
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T10:43:01.000Z
form: 8-K
items: 2.02,9.01
row 442:
accessionNumber: 0000059478-26-000104
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 443:
accessionNumber: 0001141391-26-000122
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T12:04:22.000Z
form: 8-K
items: 2.02,9.01
row 444:
accessionNumber: 0001018724-26-000038
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T20:05:27.000Z
form: 8-K
items: 2.02,9.01
row 445:
accessionNumber: 0001193125-26-438017
filingDate: 2026-10-29
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-29T21:08:00.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 446:
accessionNumber: 0000093410-26-000196
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:16:00.000Z
form: 8-K
items: 2.02,9.01
row 447:
accessionNumber: 0002115436-26-000018
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:32:50.000Z
form: 8-K
items: 2.02,7.01
row 448:
accessionNumber: 0001551152-26-000033
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T11:51:51.000Z
form: 8-K
items: 2.02,9.01
row 449:
accessionNumber: 0001628280-26-068591
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T20:23:07.000Z
form: 8-K
items: 8.01,9.01
row 450:
accessionNumber: 0001104659-26-121322
filingDate: 2026-11-02
reportDate: 2026-10-28
acceptanceDateTime: 2026-11-02T21:05:38.000Z
form: 8-K
items: 5.02
row 451:
accessionNumber: 0001321655-26-000045
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:06:48.000Z
form: 8-K
items: 2.02,7.01,9.01
row 452:
accessionNumber: 0000320193-26-000024
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:30:23.000Z
form: 8-K
items: 2.02,9.01
row 453:
accessionNumber: 0001628280-26-068909
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:33:15.000Z
form: 8-K
items: 8.01,9.01
row 454:
accessionNumber: 0000002488-26-000188
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:16:27.000Z
form: 8-K
items: 2.02,7.01,9.01
row 455:
accessionNumber: 0001628280-26-069608
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:42:13.000Z
form: 8-K
items: 8.01,9.01
row 456:
accessionNumber: 0001193125-26-447173
filingDate: 2026-11-04
reportDate: 2026-10-29
acceptanceDateTime: 2026-11-04T21:01:27.000Z
form: 8-K
items: 8.01,9.01
row 457:
accessionNumber: 0001193125-26-447507
filingDate: 2026-11-04
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-04T21:49:48.000Z
form: 8-K
items: 8.01,9.01
row 458:
accessionNumber: 0001193125-26-448357
filingDate: 2026-11-05
reportDate: 2026-11-04
acceptanceDateTime: 2026-11-05T11:01:52.000Z
form: 8-K
items: 5.02
row 459:
accessionNumber: 0001193125-26-449835
filingDate: 2026-11-05
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-05T21:10:44.000Z
form: 8-K
items: 8.01,9.01
row 460:
accessionNumber: 0001104659-26-123389
filingDate: 2026-11-05
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-05T21:33:48.000Z
form: 8-K
items: 5.02,9.01
row 461:
accessionNumber: 0001193125-26-450074
filingDate: 2026-11-05
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-05T21:58:46.000Z
form: 8-K
items: 8.01,9.01
row 462:
accessionNumber: 0001193125-26-452530
filingDate: 2026-11-09
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-09T11:10:14.000Z
form: 8-K
items: 2.02,9.01
row 463:
accessionNumber: 0001140361-26-042798
filingDate: 2026-11-09
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-09T21:30:40.000Z
form: 8-K
items: 8.01,9.01
row 464:
accessionNumber: 0000731766-26-000274
filingDate: 2026-11-09
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-09T21:33:53.000Z
form: 8-K
items: 5.02
row 465:
accessionNumber: 0000909832-26-000134
filingDate: 2026-11-10
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-10T21:16:20.000Z
form: 8-K
items: 5.02,8.01,9.01

#### Pull 2 rows

row 0:
accessionNumber: 0001045810-25-000179
filingDate: 2025-07-01
reportDate: 2025-06-25
acceptanceDateTime: 2025-06-30T22:35:29.000Z
form: 8-K
items: 5.07
row 1:
accessionNumber: 0000019617-25-000509
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:30:37.000Z
form: 8-K
items: 8.01,9.01
row 2:
accessionNumber: 0000019617-25-000510
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:31:18.000Z
form: 8-K
items: 7.01,9.01
row 3:
accessionNumber: 0001193125-25-154103
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T21:00:47.000Z
form: 8-K
items: 5.03,9.01
row 4:
accessionNumber: 0001628280-25-033842
filingDate: 2025-07-02
reportDate: 2025-07-02
acceptanceDateTime: 2025-07-02T13:05:13.000Z
form: 8-K
items: 2.02,9.01
row 5:
accessionNumber: 0000002488-25-000099
filingDate: 2025-07-02
reportDate: 2025-06-27
acceptanceDateTime: 2025-07-02T20:14:22.000Z
form: 8-K
items: 5.02
row 6:
accessionNumber: 0001551152-25-000034
filingDate: 2025-07-03
reportDate: 2025-07-03
acceptanceDateTime: 2025-07-03T17:07:55.000Z
form: 8-K
items: 2.02,9.01
row 7:
accessionNumber: 0000080424-25-000057
filingDate: 2025-07-08
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-08T20:20:53.000Z
form: 8-K
items: 7.01,9.01
row 8:
accessionNumber: 0001140361-25-025275
filingDate: 2025-07-09
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-09T01:18:13.000Z
form: 8-K
items: 5.02
row 9:
accessionNumber: 0001628280-25-034692
filingDate: 2025-07-10
reportDate: 2025-07-09
acceptanceDateTime: 2025-07-10T01:18:15.000Z
form: 8-K
items: 5.08
row 10:
accessionNumber: 0001193125-25-158202
filingDate: 2025-07-11
reportDate: 2025-07-11
acceptanceDateTime: 2025-07-11T20:14:59.000Z
form: 8-K
items: 1.02,8.01,9.01
row 11:
accessionNumber: 0000019617-25-000518
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T10:30:58.000Z
form: 8-K
items: 2.02,9.01
row 12:
accessionNumber: 0000019617-25-000520
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T14:36:04.000Z
form: 8-K
items: 7.01,9.01
row 13:
accessionNumber: 0000200406-25-000170
filingDate: 2025-07-16
reportDate: 2025-07-16
acceptanceDateTime: 2025-07-16T12:06:45.000Z
form: 8-K
items: 2.02,9.01
row 14:
accessionNumber: 0000909832-25-000061
filingDate: 2025-07-16
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-16T20:18:04.000Z
form: 8-K
items: 8.01,9.01
row 15:
accessionNumber: 0000950142-25-001949
filingDate: 2025-07-18
reportDate: 2025-07-18
acceptanceDateTime: 2025-07-18T12:40:31.000Z
form: 8-K
items: 7.01,8.01,9.01
row 16:
accessionNumber: 0001104659-25-069019
filingDate: 2025-07-18
reportDate: 2025-07-17
acceptanceDateTime: 2025-07-18T20:05:39.000Z
form: 8-K
items: 5.03,9.01
row 17:
accessionNumber: 0001193125-25-161225
filingDate: 2025-07-18
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-18T20:16:46.000Z
form: 8-K
items: 8.01,9.01
row 18:
accessionNumber: 0000021344-25-000054
filingDate: 2025-07-22
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-22T11:00:23.000Z
form: 8-K
items: 2.02,9.01
row 19:
accessionNumber: 0001652044-25-000056
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:01:33.000Z
form: 8-K
items: 2.02,8.01,9.01
row 20:
accessionNumber: 0001403161-25-000043
filingDate: 2025-07-23
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-23T20:08:09.000Z
form: 8-K
items: 5.03
row 21:
accessionNumber: 0001628280-25-035738
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:14:09.000Z
form: 8-K
items: 2.02,9.01
row 22:
accessionNumber: 0001193125-25-163423
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:15:17.000Z
form: 8-K
items: 8.01,9.01
row 23:
accessionNumber: 0000731766-25-000224
filingDate: 2025-07-24
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-24T12:30:24.000Z
form: 8-K
items: 8.01
row 24:
accessionNumber: 0001140361-25-027340
filingDate: 2025-07-25
reportDate: 2025-07-21
acceptanceDateTime: 2025-07-25T20:30:49.000Z
form: 8-K
items: 5.02
row 25:
accessionNumber: 0000080424-25-000061
filingDate: 2025-07-28
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-28T21:03:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 26:
accessionNumber: 0000731766-25-000228
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T10:04:05.000Z
form: 8-K
items: 2.02,9.01
row 27:
accessionNumber: 0001104659-25-071380
filingDate: 2025-07-29
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-29T10:42:43.000Z
form: 8-K
items: 2.02,2.05,9.01
row 28:
accessionNumber: 0000080424-25-000067
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T11:03:15.000Z
form: 8-K
items: 2.02,9.01
row 29:
accessionNumber: 0000080424-25-000069
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T14:51:39.000Z
form: 8-K
items: 7.01,9.01
row 30:
accessionNumber: 0001403161-25-000051
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T20:06:16.000Z
form: 8-K
items: 2.02,8.01,9.01
row 31:
accessionNumber: 0000950142-25-002041
filingDate: 2025-07-29
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-29T20:10:21.000Z
form: 8-K
items: 5.02
row 32:
accessionNumber: 0000950170-25-100226
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:08:53.000Z
form: 8-K
items: 2.02,9.01
row 33:
accessionNumber: 0001628280-25-036719
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 34:
accessionNumber: 0001551152-25-000036
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T11:48:24.000Z
form: 8-K
items: 2.02,9.01
row 35:
accessionNumber: 0001141391-25-000170
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T12:03:19.000Z
form: 8-K
items: 2.02,9.01
row 36:
accessionNumber: 0001018724-25-000084
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:13:17.000Z
form: 8-K
items: 2.02,9.01
row 37:
accessionNumber: 0000320193-25-000071
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:30:25.000Z
form: 8-K
items: 2.02,9.01
row 38:
accessionNumber: 0000731766-25-000232
filingDate: 2025-07-31
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-31T21:08:18.000Z
form: 8-K
items: 5.02
row 39:
accessionNumber: 0000093410-25-000058
filingDate: 2025-08-01
reportDate: 2025-08-01
acceptanceDateTime: 2025-08-01T10:17:27.000Z
form: 8-K
items: 2.02,9.01
row 40:
accessionNumber: 0001104659-25-073263
filingDate: 2025-08-04
reportDate: 2025-08-03
acceptanceDateTime: 2025-08-04T10:03:14.000Z
form: 8-K
items: 5.02,7.01,9.01
row 41:
accessionNumber: 0001193125-25-172579
filingDate: 2025-08-04
reportDate: 2025-08-02
acceptanceDateTime: 2025-08-04T19:55:28.000Z
form: 8-K
items: 2.02,9.01
row 42:
accessionNumber: 0001321655-25-000105
filingDate: 2025-08-04
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-04T20:07:52.000Z
form: 8-K
items: 2.02,7.01,9.01
row 43:
accessionNumber: 0000002488-25-000106
filingDate: 2025-08-05
reportDate: 2025-08-05
acceptanceDateTime: 2025-08-05T20:16:31.000Z
form: 8-K
items: 2.02,7.01,9.01
row 44:
accessionNumber: 0001045810-25-000197
filingDate: 2025-08-05
reportDate: 2025-07-31
acceptanceDateTime: 2025-08-05T20:31:08.000Z
form: 8-K
items: 5.02
row 45:
accessionNumber: 0000059478-25-000202
filingDate: 2025-08-07
reportDate: 2025-08-07
acceptanceDateTime: 2025-08-07T11:05:40.000Z
form: 8-K
items: 2.02,9.01
row 46:
accessionNumber: 0000909832-25-000064
filingDate: 2025-08-07
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-07T20:35:32.000Z
form: 8-K
items: 5.02
row 47:
accessionNumber: 0001403161-25-000055
filingDate: 2025-08-08
reportDate: 2025-08-08
acceptanceDateTime: 2025-08-08T20:07:08.000Z
form: 8-K
items: 3.02
row 48:
accessionNumber: 0001104659-25-075940
filingDate: 2025-08-11
reportDate: 2025-08-11
acceptanceDateTime: 2025-08-11T12:05:18.000Z
form: 8-K
items: 7.01,9.01
row 49:
accessionNumber: 0001193125-25-179820
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:11:01.000Z
form: 8-K
items: 2.02,9.01
row 50:
accessionNumber: 0001193125-25-179846
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:16:58.000Z
form: 8-K
items: 8.01,9.01
row 51:
accessionNumber: 0000080424-25-000111
filingDate: 2025-08-14
reportDate: 2025-08-14
acceptanceDateTime: 2025-08-14T14:00:31.000Z
form: 8-K
items: 5.02
row 52:
accessionNumber: 0000731766-25-000239
filingDate: 2025-08-20
reportDate: 2025-08-20
acceptanceDateTime: 2025-08-20T20:06:17.000Z
form: 8-K
items: 7.01
row 53:
accessionNumber: 0001193125-25-184093
filingDate: 2025-08-20
reportDate: 2025-08-18
acceptanceDateTime: 2025-08-20T20:16:08.000Z
form: 8-K
items: 8.01,9.01
row 54:
accessionNumber: 0000104169-25-000120
filingDate: 2025-08-21
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-21T10:59:09.000Z
form: 8-K
items: 2.02,9.01
row 55:
accessionNumber: 0000002488-25-000147
filingDate: 2025-08-25
reportDate: 2025-08-22
acceptanceDateTime: 2025-08-25T20:07:00.000Z
form: 8-K
items: 5.02
row 56:
accessionNumber: 0000858877-25-000103
filingDate: 2025-08-25
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-25T20:27:47.000Z
form: 8-K
items: 5.03,9.01
row 57:
accessionNumber: 0001045810-25-000207
filingDate: 2025-08-27
reportDate: 2025-08-27
acceptanceDateTime: 2025-08-27T20:22:14.000Z
form: 8-K
items: 2.02,9.01
row 58:
accessionNumber: 0001652044-25-000067
filingDate: 2025-09-03
reportDate: 2025-09-02
acceptanceDateTime: 2025-09-03T20:30:34.000Z
form: 8-K
items: 8.01
row 59:
accessionNumber: 0001730168-25-000094
filingDate: 2025-09-04
reportDate: 2025-09-04
acceptanceDateTime: 2025-09-04T20:19:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 60:
accessionNumber: 0000104169-25-000143
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:07:39.000Z
form: 8-K
items: 8.01
row 61:
accessionNumber: 0001104659-25-087862
filingDate: 2025-09-05
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-05T20:46:03.000Z
form: 8-K
items: 1.01,9.01
row 62:
accessionNumber: 0001652044-25-000074
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:53:32.000Z
form: 8-K
items: 8.01
row 63:
accessionNumber: 0000731766-25-000245
filingDate: 2025-09-08
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T11:00:14.000Z
form: 8-K
items: 7.01
row 64:
accessionNumber: 0000200406-25-000190
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T23:55:25.000Z
form: 8-K
items: 5.02
row 65:
accessionNumber: 0000731766-25-000247
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-09T11:00:13.000Z
form: 8-K/A
items: 7.01
row 66:
accessionNumber: 0001193125-25-199175
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:13:19.000Z
form: 8-K
items: 2.02,8.01,9.01
row 67:
accessionNumber: 0000310158-25-000047
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:33:09.000Z
form: 8-K
items: 8.01,9.01
row 68:
accessionNumber: 0001193125-25-199281
filingDate: 2025-09-09
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-09T21:28:00.000Z
form: 8-K
items: 5.02,9.01
row 69:
accessionNumber: 0001193125-25-200108
filingDate: 2025-09-10
reportDate: 2025-09-10
acceptanceDateTime: 2025-09-10T20:16:49.000Z
form: 8-K
items: 8.01,9.01
row 70:
accessionNumber: 0001104659-25-089245
filingDate: 2025-09-11
reportDate: 2025-09-11
acceptanceDateTime: 2025-09-11T11:30:54.000Z
form: 8-K
items: 7.01,9.01
row 71:
accessionNumber: 0000019617-25-000907
filingDate: 2025-09-12
reportDate: 2025-09-12
acceptanceDateTime: 2025-09-12T20:32:01.000Z
form: 8-K
items: 5.03,9.01
row 72:
accessionNumber: 0000104169-25-000151
filingDate: 2025-09-19
reportDate: 2025-09-19
acceptanceDateTime: 2025-09-19T20:04:09.000Z
form: 8-K
items: 8.01
row 73:
accessionNumber: 0001403161-25-000058
filingDate: 2025-09-19
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-19T20:08:17.000Z
form: 8-K
items: 8.01
row 74:
accessionNumber: 0001193125-25-210089
filingDate: 2025-09-22
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-22T12:22:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 75:
accessionNumber: 0000104169-25-000153
filingDate: 2025-09-22
reportDate: 2025-09-22
acceptanceDateTime: 2025-09-22T20:39:22.000Z
form: 8-K
items: 8.01
row 76:
accessionNumber: 0000723125-25-000024
filingDate: 2025-09-23
reportDate: 2025-09-23
acceptanceDateTime: 2025-09-23T20:02:28.000Z
form: 8-K
items: 2.02,9.01
row 77:
accessionNumber: 0000093410-25-000098
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T12:00:43.000Z
form: 8-K
items: 7.01
row 78:
accessionNumber: 0000909832-25-000093
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T20:16:57.000Z
form: 8-K
items: 2.02,9.01
row 79:
accessionNumber: 0001193125-25-220445
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:05:13.000Z
form: 8-K
items: 8.01,9.01
row 80:
accessionNumber: 0001403161-25-000061
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:12:37.000Z
form: 8-K
items: 8.01
row 81:
accessionNumber: 0001403161-25-000064
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:06:58.000Z
form: 8-K
items: 5.02,9.01
row 82:
accessionNumber: 0001193125-25-223202
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:08:40.000Z
form: 8-K
items: 8.01,9.01
row 83:
accessionNumber: 0001193125-25-225125
filingDate: 2025-09-30
reportDate: 2025-09-24
acceptanceDateTime: 2025-09-30T20:37:10.000Z
form: 8-K
items: 5.02
row 84:
accessionNumber: 0001628280-25-043530
filingDate: 2025-10-02
reportDate: 2025-10-02
acceptanceDateTime: 2025-10-02T13:04:54.000Z
form: 8-K
items: 2.02,9.01
row 85:
accessionNumber: 0001193125-25-229405
filingDate: 2025-10-03
reportDate: 2025-09-30
acceptanceDateTime: 2025-10-03T14:34:37.000Z
form: 8-K
items: 5.03,9.01
row 86:
accessionNumber: 0001551152-25-000043
filingDate: 2025-10-03
reportDate: 2025-10-03
acceptanceDateTime: 2025-10-03T20:09:03.000Z
form: 8-K
items: 2.02,9.01
row 87:
accessionNumber: 0001193125-25-230895
filingDate: 2025-10-06
reportDate: 2025-10-05
acceptanceDateTime: 2025-10-06T11:04:49.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 88:
accessionNumber: 0001193125-25-231901
filingDate: 2025-10-06
reportDate: 2025-09-18
acceptanceDateTime: 2025-10-06T20:15:26.000Z
form: 8-K/A
items: 5.02
row 89:
accessionNumber: 0001628280-25-044845
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T10:30:57.000Z
form: 8-K
items: 2.02,9.01
row 90:
accessionNumber: 0000200406-25-000201
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T11:22:58.000Z
form: 8-K
items: 2.02,8.01,9.01
row 91:
accessionNumber: 0001628280-25-044887
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T13:49:09.000Z
form: 8-K
items: 7.01,9.01
row 92:
accessionNumber: 0000080424-25-000217
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T14:55:51.000Z
form: 8-K
items: 7.01,9.01
row 93:
accessionNumber: 0000909832-25-000105
filingDate: 2025-10-15
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-15T20:30:30.000Z
form: 8-K
items: 8.01,9.01
row 94:
accessionNumber: 0000080424-25-000235
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:25:14.000Z
form: 8-K
items: 5.02,5.07,9.01
row 95:
accessionNumber: 0001628280-25-045223
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:35:16.000Z
form: 8-K
items: 5.02,9.01
row 96:
accessionNumber: 0000858877-25-000145
filingDate: 2025-10-17
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-17T20:13:47.000Z
form: 8-K
items: 5.02
row 97:
accessionNumber: 0000909832-25-000107
filingDate: 2025-10-20
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-20T21:00:26.000Z
form: 8-K
items: 5.02,9.01
row 98:
accessionNumber: 0001628280-25-045577
filingDate: 2025-10-21
reportDate: 2025-10-21
acceptanceDateTime: 2025-10-21T10:59:07.000Z
form: 8-K
items: 2.02,9.01
row 99:
accessionNumber: 0001104659-25-101237
filingDate: 2025-10-21
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-21T20:09:06.000Z
form: 8-K
items: 5.02,9.01
row 100:
accessionNumber: 0001628280-25-045861
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:06:36.000Z
form: 8-K
items: 2.02,9.01
row 101:
accessionNumber: 0001193125-25-246803
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:17:53.000Z
form: 8-K
items: 8.01,9.01
row 102:
accessionNumber: 0000104169-25-000168
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:20:22.000Z
form: 8-K
items: 5.02
row 103:
accessionNumber: 0000080424-25-000240
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T11:04:27.000Z
form: 8-K
items: 2.02,9.01
row 104:
accessionNumber: 0000080424-25-000243
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T14:10:46.000Z
form: 8-K
items: 7.01,9.01
row 105:
accessionNumber: 0001193125-25-250803
filingDate: 2025-10-27
reportDate: 2025-10-27
acceptanceDateTime: 2025-10-27T12:49:27.000Z
form: 8-K
items: 2.01,7.01,9.01
row 106:
accessionNumber: 0000731766-25-000301
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T10:02:08.000Z
form: 8-K
items: 2.02,9.01
row 107:
accessionNumber: 0001403161-25-000077
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T20:06:03.000Z
form: 8-K
items: 2.02,8.01,9.01
row 108:
accessionNumber: 0001652044-25-000087
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:01:48.000Z
form: 8-K
items: 2.02,9.01
row 109:
accessionNumber: 0001193125-25-256310
filingDate: 2025-10-29
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-29T20:07:42.000Z
form: 8-K
items: 2.02,7.01,9.01
row 110:
accessionNumber: 0001628280-25-047114
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:08:34.000Z
form: 8-K
items: 2.02,9.01
row 111:
accessionNumber: 0001104659-25-103974
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T10:40:38.000Z
form: 8-K
items: 2.02,9.01
row 112:
accessionNumber: 0000059478-25-000251
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T11:03:41.000Z
form: 8-K
items: 2.02,9.01
row 113:
accessionNumber: 0001141391-25-000191
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T12:03:18.000Z
form: 8-K
items: 2.02,9.01
row 114:
accessionNumber: 0001018724-25-000121
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 115:
accessionNumber: 0000320193-25-000077
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:30:35.000Z
form: 8-K
items: 2.02,9.01
row 116:
accessionNumber: 0000093410-25-000103
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T10:16:33.000Z
form: 8-K
items: 2.02,9.01
row 117:
accessionNumber: 0001551152-25-000047
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T11:51:43.000Z
form: 8-K
items: 2.02,9.01
row 118:
accessionNumber: 0000093410-25-000105
filingDate: 2025-11-03
reportDate: 2025-10-29
acceptanceDateTime: 2025-11-03T13:11:08.000Z
form: 8-K
items: 5.02
row 119:
accessionNumber: 0001193125-25-262260
filingDate: 2025-11-03
reportDate: 2025-11-01
acceptanceDateTime: 2025-11-03T18:48:34.000Z
form: 8-K
items: 2.02,9.01
row 120:
accessionNumber: 0001321655-25-000130
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:06:20.000Z
form: 8-K
items: 2.02,7.01,9.01
row 121:
accessionNumber: 0001193125-25-262593
filingDate: 2025-11-03
reportDate: 2025-10-30
acceptanceDateTime: 2025-11-03T21:18:13.000Z
form: 8-K
items: 8.01,9.01
row 122:
accessionNumber: 0001193125-25-262609
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:23:10.000Z
form: 8-K
items: 8.01,9.01
row 123:
accessionNumber: 0001193125-25-264728
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:00.000Z
form: 8-K
items: 8.01,9.01
row 124:
accessionNumber: 0000002488-25-000163
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:10.000Z
form: 8-K
items: 2.02,7.01,9.01
row 125:
accessionNumber: 0001193125-25-269979
filingDate: 2025-11-06
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-06T21:47:26.000Z
form: 8-K
items: 8.01,9.01
row 126:
accessionNumber: 0000731766-25-000308
filingDate: 2025-11-07
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-07T21:13:36.000Z
form: 8-K
items: 7.01
row 127:
accessionNumber: 0001104659-25-108507
filingDate: 2025-11-07
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-07T21:27:23.000Z
form: 8-K
items: 5.02,5.07,9.01
row 128:
accessionNumber: 0001403161-25-000093
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:30:43.000Z
form: 8-K
items: 8.01,9.01
row 129:
accessionNumber: 0001141391-25-000197
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:31:40.000Z
form: 8-K
items: 8.01,9.01
row 130:
accessionNumber: 0001193125-25-277624
filingDate: 2025-11-12
reportDate: 2025-11-12
acceptanceDateTime: 2025-11-12T21:15:30.000Z
form: 8-K
items: 2.02,9.01
row 131:
accessionNumber: 0001141391-25-000199
filingDate: 2025-11-12
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-12T22:15:17.000Z
form: 8-K
items: 1.01
row 132:
accessionNumber: 0000731766-25-000310
filingDate: 2025-11-13
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-13T21:02:22.000Z
form: 8-K
items: 5.03
row 133:
accessionNumber: 0000104169-25-000172
filingDate: 2025-11-14
reportDate: 2025-11-11
acceptanceDateTime: 2025-11-14T13:00:30.000Z
form: 8-K
items: 5.02,9.01
row 134:
accessionNumber: 0001045810-25-000228
filingDate: 2025-11-19
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-19T21:20:44.000Z
form: 8-K
items: 2.02,9.01
row 135:
accessionNumber: 0000104169-25-000177
filingDate: 2025-11-20
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-20T11:58:46.000Z
form: 8-K
items: 2.02,3.01,7.01,9.01
row 136:
accessionNumber: 0001104659-25-114647
filingDate: 2025-11-20
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-20T22:00:42.000Z
form: 8-K
items: 8.01,9.01
row 137:
accessionNumber: 0001193125-25-290864
filingDate: 2025-11-21
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-21T15:46:21.000Z
form: 8-K
items: 8.01,9.01
row 138:
accessionNumber: 0000059478-25-000271
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:19:05.000Z
form: 8-K
items: 5.02
row 139:
accessionNumber: 0001193125-25-291441
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:26:49.000Z
form: 8-K
items: 5.02,5.07,9.01
row 140:
accessionNumber: 0000731766-25-000314
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T22:20:04.000Z
form: 8-K
items: 5.02
row 141:
accessionNumber: 0001628280-25-055388
filingDate: 2025-12-04
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-04T21:36:38.000Z
form: 8-K
items: 8.01,9.01
row 142:
accessionNumber: 0000093410-25-000122
filingDate: 2025-12-05
reportDate: 2025-12-03
acceptanceDateTime: 2025-12-05T21:21:15.000Z
form: 8-K
items: 5.03,8.01,9.01
row 143:
accessionNumber: 0001140361-25-044561
filingDate: 2025-12-05
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-05T21:31:42.000Z
form: 8-K
items: 5.02
row 144:
accessionNumber: 0000019617-25-001100
filingDate: 2025-12-08
reportDate: 2025-12-07
acceptanceDateTime: 2025-12-08T11:30:37.000Z
form: 8-K
items: 5.02
row 145:
accessionNumber: 0001193125-25-311196
filingDate: 2025-12-08
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-08T21:00:35.000Z
form: 8-K
items: 5.02,5.07
row 146:
accessionNumber: 0001193125-25-312771
filingDate: 2025-12-09
reportDate: 2025-12-09
acceptanceDateTime: 2025-12-09T21:18:53.000Z
form: 8-K
items: 8.01,9.01
row 147:
accessionNumber: 0001193125-25-314207
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T21:14:38.000Z
form: 8-K
items: 2.02,8.01,9.01
row 148:
accessionNumber: 0001552781-25-000454
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T22:19:43.000Z
form: 8-K
items: 5.02,9.01
row 149:
accessionNumber: 0001193125-25-314935
filingDate: 2025-12-11
reportDate: 2025-12-08
acceptanceDateTime: 2025-12-11T11:02:16.000Z
form: 8-K
items: 5.02,9.01
row 150:
accessionNumber: 0001730168-25-000116
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:17:37.000Z
form: 8-K
items: 2.02,8.01,9.01
row 151:
accessionNumber: 0000909832-25-000164
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:22:04.000Z
form: 8-K
items: 2.02,9.01
row 152:
accessionNumber: 0001628280-25-056768
filingDate: 2025-12-12
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-12T21:14:29.000Z
form: 8-K
items: 8.01,9.01
row 153:
accessionNumber: 0000080424-25-000287
filingDate: 2025-12-15
reportDate: 2025-12-15
acceptanceDateTime: 2025-12-15T14:15:22.000Z
form: 8-K
items: 5.02
row 154:
accessionNumber: 0000002488-25-000182
filingDate: 2025-12-15
reportDate: 2025-12-12
acceptanceDateTime: 2025-12-15T21:12:11.000Z
form: 8-K
items: 5.02,9.01
row 155:
accessionNumber: 0000723125-25-000044
filingDate: 2025-12-17
reportDate: 2025-12-17
acceptanceDateTime: 2025-12-17T21:03:26.000Z
form: 8-K
items: 2.02,9.01
row 156:
accessionNumber: 0000858877-25-000199
filingDate: 2025-12-17
reportDate: 2025-12-16
acceptanceDateTime: 2025-12-17T21:42:08.000Z
form: 8-K
items: 5.02,5.07,9.01
row 157:
accessionNumber: 0000093410-25-000130
filingDate: 2025-12-19
reportDate: 2025-07-28
acceptanceDateTime: 2025-12-19T21:25:35.000Z
form: 8-K/A
items: 5.02
row 158:
accessionNumber: 0001628280-25-058337
filingDate: 2025-12-19
reportDate: 2025-12-19
acceptanceDateTime: 2025-12-19T22:00:37.000Z
form: 8-K
items: 5.02
row 159:
accessionNumber: 0001403161-25-000134
filingDate: 2025-12-23
reportDate: 2025-12-23
acceptanceDateTime: 2025-12-23T21:06:56.000Z
form: 8-K
items: 8.01
row 160:
accessionNumber: 0000104169-25-000238
filingDate: 2025-12-29
reportDate: 2025-12-24
acceptanceDateTime: 2025-12-29T21:40:38.000Z
form: 8-K
items: 8.01
row 161:
accessionNumber: 0001403161-25-000137
filingDate: 2025-12-30
reportDate: 2025-12-30
acceptanceDateTime: 2025-12-30T21:07:17.000Z
form: 8-K
items: 8.01
row 162:
accessionNumber: 0001628280-26-000016
filingDate: 2026-01-02
reportDate: 2026-01-02
acceptanceDateTime: 2026-01-02T14:20:13.000Z
form: 8-K
items: 2.02,9.01
row 163:
accessionNumber: 0001140361-26-000199
filingDate: 2026-01-02
reportDate: 2025-12-30
acceptanceDateTime: 2026-01-02T21:30:52.000Z
form: 8-K
items: 5.02
row 164:
accessionNumber: 0001193125-26-004727
filingDate: 2026-01-06
reportDate: 2025-05-03
acceptanceDateTime: 2026-01-06T22:00:33.000Z
form: 8-K/A
items: 5.02
row 165:
accessionNumber: 0001551152-26-000002
filingDate: 2026-01-07
reportDate: 2026-01-07
acceptanceDateTime: 2026-01-07T21:08:59.000Z
form: 8-K
items: 2.02,9.01
row 166:
accessionNumber: 0000104169-26-000008
filingDate: 2026-01-08
reportDate: 2026-01-08
acceptanceDateTime: 2026-01-08T12:59:51.000Z
form: 8-K
items: 5.02,9.01
row 167:
accessionNumber: 0001193125-26-009002
filingDate: 2026-01-09
reportDate: 2026-01-05
acceptanceDateTime: 2026-01-09T21:31:11.000Z
form: 8-K
items: 5.02
row 168:
accessionNumber: 0000731766-26-000020
filingDate: 2026-01-12
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-12T11:58:08.000Z
form: 8-K
items: 7.01
row 169:
accessionNumber: 0001628280-26-001902
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T11:41:09.000Z
form: 8-K
items: 2.02,9.01
row 170:
accessionNumber: 0001628280-26-001915
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T15:09:19.000Z
form: 8-K
items: 7.01,9.01
row 171:
accessionNumber: 0001193125-26-011731
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:06:00.000Z
form: 8-K
items: 8.01,9.01
row 172:
accessionNumber: 0000080424-26-000002
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:27:59.000Z
form: 8-K
items: 7.01,9.01
row 173:
accessionNumber: 0001552781-26-000017
filingDate: 2026-01-14
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-14T11:58:41.000Z
form: 8-K
items: 5.02,9.01
row 174:
accessionNumber: 0000104169-26-000023
filingDate: 2026-01-16
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-16T14:01:15.000Z
form: 8-K
items: 5.02,9.01
row 175:
accessionNumber: 0000104169-26-000024
filingDate: 2026-01-16
reportDate: 2025-11-13
acceptanceDateTime: 2026-01-16T14:03:05.000Z
form: 8-K/A
items: 5.02
row 176:
accessionNumber: 0001628280-26-002429
filingDate: 2026-01-16
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-16T21:56:58.000Z
form: 8-K
items: 5.02
row 177:
accessionNumber: 0000002488-26-000002
filingDate: 2026-01-20
reportDate: 2026-01-16
acceptanceDateTime: 2026-01-20T21:19:32.000Z
form: 8-K
items: 5.02,9.01
row 178:
accessionNumber: 0000200406-26-000002
filingDate: 2026-01-21
reportDate: 2026-01-21
acceptanceDateTime: 2026-01-21T12:46:18.000Z
form: 8-K
items: 2.02,9.01
row 179:
accessionNumber: 0001104659-26-005366
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:05:37.000Z
form: 8-K
items: 5.03,5.07,9.01
row 180:
accessionNumber: 0000909832-26-000016
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:16:10.000Z
form: 8-K
items: 5.07,8.01
row 181:
accessionNumber: 0000080424-26-000006
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T12:02:05.000Z
form: 8-K
items: 2.02,9.01
row 182:
accessionNumber: 0000080424-26-000009
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T16:53:22.000Z
form: 8-K
items: 7.01,9.01
row 183:
accessionNumber: 0001193125-26-019450
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T21:15:33.000Z
form: 8-K
items: 8.01,9.01
row 184:
accessionNumber: 0000019617-26-000052
filingDate: 2026-01-22
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-22T21:30:18.000Z
form: 8-K
items: 5.02
row 185:
accessionNumber: 0001045810-26-000003
filingDate: 2026-01-23
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-23T22:01:33.000Z
form: 8-K
items: 5.02
row 186:
accessionNumber: 0000731766-26-000025
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T11:02:29.000Z
form: 8-K
items: 2.02,9.01
row 187:
accessionNumber: 0000093410-26-000010
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T21:45:32.000Z
form: 8-K
items: 5.02
row 188:
accessionNumber: 0001628280-26-003832
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:20.000Z
form: 8-K
items: 2.02,9.01
row 189:
accessionNumber: 0001193125-26-027198
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:38.000Z
form: 8-K
items: 2.02,9.01
row 190:
accessionNumber: 0001628280-26-003837
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:11:04.000Z
form: 8-K
items: 2.02,9.01
row 191:
accessionNumber: 0001403161-26-000029
filingDate: 2026-01-28
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-28T21:43:36.000Z
form: 8-K
items: 5.03,5.07
row 192:
accessionNumber: 0001141391-26-000003
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T13:03:21.000Z
form: 8-K
items: 2.02,9.01
row 193:
accessionNumber: 0001403161-26-000044
filingDate: 2026-01-29
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-29T21:05:49.000Z
form: 8-K
items: 2.02,8.01,9.01
row 194:
accessionNumber: 0000320193-26-000005
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T21:30:33.000Z
form: 8-K
items: 2.02,9.01
row 195:
accessionNumber: 0000093410-26-000019
filingDate: 2026-01-30
reportDate: 2026-01-30
acceptanceDateTime: 2026-01-30T11:16:19.000Z
form: 8-K
items: 2.02,9.01
row 196:
accessionNumber: 0000104169-26-000028
filingDate: 2026-01-30
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-30T21:10:02.000Z
form: 8-K/A
items: 5.02
row 197:
accessionNumber: 0000093410-26-000021
filingDate: 2026-01-30
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-30T21:30:32.000Z
form: 8-K
items: 5.02
row 198:
accessionNumber: 0001321655-26-000004
filingDate: 2026-02-02
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-02T21:06:08.000Z
form: 8-K
items: 2.02,7.01,9.01
row 199:
accessionNumber: 0001104659-26-009495
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T11:38:40.000Z
form: 8-K
items: 2.02,9.01
row 200:
accessionNumber: 0000002488-26-000014
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T21:16:18.000Z
form: 8-K
items: 2.02,7.01,9.01
row 201:
accessionNumber: 0000059478-26-000008
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:05:22.000Z
form: 8-K
items: 2.02,9.01
row 202:
accessionNumber: 0001551152-26-000004
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:54:33.000Z
form: 8-K
items: 2.02,9.01
row 203:
accessionNumber: 0001652044-26-000012
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T21:01:37.000Z
form: 8-K
items: 2.02,9.01
row 204:
accessionNumber: 0001193125-26-037840
filingDate: 2026-02-04
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-04T22:20:31.000Z
form: 8-K
items: 1.01,8.01,9.01
row 205:
accessionNumber: 0001193125-26-039344
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:01:31.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 206:
accessionNumber: 0001141391-26-000006
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:04:53.000Z
form: 8-K
items: 5.02
row 207:
accessionNumber: 0001193125-26-039427
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:17:31.000Z
form: 8-K
items: 8.01,9.01
row 208:
accessionNumber: 0001018724-26-000002
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:25:12.000Z
form: 8-K
items: 2.02,9.01
row 209:
accessionNumber: 0001628280-26-006642
filingDate: 2026-02-10
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-10T11:59:38.000Z
form: 8-K
items: 2.02,9.01
row 210:
accessionNumber: 0000858877-26-000006
filingDate: 2026-02-11
reportDate: 2026-02-11
acceptanceDateTime: 2026-02-11T21:07:20.000Z
form: 8-K
items: 2.02,9.01
row 211:
accessionNumber: 0001628280-26-007709
filingDate: 2026-02-12
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-12T21:30:37.000Z
form: 8-K
items: 8.01,9.01
row 212:
accessionNumber: 0001403161-26-000049
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T13:45:50.000Z
form: 8-K
items: 7.01
row 213:
accessionNumber: 0001193125-26-051423
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T21:16:46.000Z
form: 8-K
items: 8.01,9.01
row 214:
accessionNumber: 0000002488-26-000029
filingDate: 2026-02-17
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-17T21:21:24.000Z
form: 8-K
items: 5.02
row 215:
accessionNumber: 0000104169-26-000032
filingDate: 2026-02-19
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-19T11:59:55.000Z
form: 8-K
items: 2.02,9.01
row 216:
accessionNumber: 0001628280-26-010052
filingDate: 2026-02-20
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-20T15:10:16.000Z
form: 8-K
items: 5.02,9.01
row 217:
accessionNumber: 0001628280-26-010693
filingDate: 2026-02-23
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-23T21:39:11.000Z
form: 8-K
items: 7.01,9.01
row 218:
accessionNumber: 0000002488-26-000045
filingDate: 2026-02-24
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-24T12:01:06.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 219:
accessionNumber: 0001140361-26-006577
filingDate: 2026-02-24
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-24T21:55:58.000Z
form: 8-K
items: 5.07,9.01
row 220:
accessionNumber: 0000731766-26-000046
filingDate: 2026-02-25
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-25T11:23:37.000Z
form: 8-K
items: 5.02
row 221:
accessionNumber: 0001045810-26-000019
filingDate: 2026-02-25
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-25T21:31:25.000Z
form: 8-K
items: 2.02,9.01
row 222:
accessionNumber: 0001104659-26-020643
filingDate: 2026-02-26
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-26T22:14:40.000Z
form: 8-K
items: 8.01,9.01
row 223:
accessionNumber: 0001104659-26-021050
filingDate: 2026-02-27
reportDate: 2026-02-27
acceptanceDateTime: 2026-02-27T13:36:30.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 224:
accessionNumber: 0001403161-26-000063
filingDate: 2026-02-27
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-27T21:06:59.000Z
form: 8-K
items: 8.01
row 225:
accessionNumber: 0000731766-26-000064
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T14:21:03.000Z
form: 8-K
items: 5.02
row 226:
accessionNumber: 0001193125-26-085656
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T22:00:50.000Z
form: 8-K
items: 5.02
row 227:
accessionNumber: 0001193125-26-085801
filingDate: 2026-03-02
reportDate: 2026-02-28
acceptanceDateTime: 2026-03-02T22:27:20.000Z
form: 8-K
items: 2.02,9.01
row 228:
accessionNumber: 0001730168-26-000011
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:16:10.000Z
form: 8-K
items: 2.02,8.01,9.01
row 229:
accessionNumber: 0001104659-26-023534
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:59:47.000Z
form: 8-K
items: 8.01,9.01
row 230:
accessionNumber: 0001193125-26-092557
filingDate: 2026-03-05
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-05T12:25:35.000Z
form: 8-K
items: 8.01,9.01
row 231:
accessionNumber: 0000909832-26-000025
filingDate: 2026-03-05
reportDate: 2026-03-05
acceptanceDateTime: 2026-03-05T21:19:07.000Z
form: 8-K
items: 2.02,9.01
row 232:
accessionNumber: 0001045810-26-000024
filingDate: 2026-03-06
reportDate: 2026-03-02
acceptanceDateTime: 2026-03-06T21:11:25.000Z
form: 8-K
items: 5.02,9.01
row 233:
accessionNumber: 0001652044-26-000026
filingDate: 2026-03-06
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-06T22:21:44.000Z
form: 8-K
items: 5.02
row 234:
accessionNumber: 0000731766-26-000067
filingDate: 2026-03-09
reportDate: 2026-03-09
acceptanceDateTime: 2026-03-09T20:33:13.000Z
form: 8-K
items: 7.01
row 235:
accessionNumber: 0001193125-26-100148
filingDate: 2026-03-10
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-10T20:12:51.000Z
form: 8-K
items: 2.02,8.01,9.01
row 236:
accessionNumber: 0000104169-26-000057
filingDate: 2026-03-13
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-13T20:10:19.000Z
form: 8-K
items: 8.01
row 237:
accessionNumber: 0001104659-26-027729
filingDate: 2026-03-13
reportDate: 2026-03-13
acceptanceDateTime: 2026-03-13T21:01:35.000Z
form: 8-K
items: 8.01,9.01
row 238:
accessionNumber: 0001104659-26-028556
filingDate: 2026-03-16
reportDate: 2026-03-16
acceptanceDateTime: 2026-03-16T20:54:55.000Z
form: 8-K
items: 8.01,9.01
row 239:
accessionNumber: 0000723125-26-000004
filingDate: 2026-03-18
reportDate: 2026-03-18
acceptanceDateTime: 2026-03-18T20:02:14.000Z
form: 8-K
items: 2.02,9.01
row 240:
accessionNumber: 0001104659-26-034174
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T12:26:22.000Z
form: 8-K
items: 8.01,9.01
row 241:
accessionNumber: 0000093410-26-000103
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T20:36:44.000Z
form: 8-K
items: 5.03,9.01
row 242:
accessionNumber: 0000104169-26-000067
filingDate: 2026-03-27
reportDate: 2026-03-27
acceptanceDateTime: 2026-03-27T20:10:53.000Z
form: 8-K
items: 8.01
row 243:
accessionNumber: 0001104659-26-038249
filingDate: 2026-04-01
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-01T12:33:36.000Z
form: 8-K
items: 8.01,9.01
row 244:
accessionNumber: 0001628280-26-022956
filingDate: 2026-04-02
reportDate: 2026-04-02
acceptanceDateTime: 2026-04-02T13:07:13.000Z
form: 8-K
items: 2.02,9.01
row 245:
accessionNumber: 0001652044-26-000031
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T20:18:28.000Z
form: 8-K
items: 5.02
row 246:
accessionNumber: 0001193125-26-140574
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T21:25:00.000Z
form: 8-K
items: 5.02
row 247:
accessionNumber: 0001551152-26-000011
filingDate: 2026-04-03
reportDate: 2026-04-03
acceptanceDateTime: 2026-04-03T20:05:55.000Z
form: 8-K
items: 2.02,9.01
row 248:
accessionNumber: 0001193125-26-142939
filingDate: 2026-04-06
reportDate: 2026-04-01
acceptanceDateTime: 2026-04-06T12:12:11.000Z
form: 8-K
items: 5.02,7.01,9.01
row 249:
accessionNumber: 0000858877-26-000048
filingDate: 2026-04-06
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-06T20:29:18.000Z
form: 8-K
items: 5.02
row 250:
accessionNumber: 0001193125-26-144028
filingDate: 2026-04-06
reportDate: 2026-04-06
acceptanceDateTime: 2026-04-06T21:22:08.000Z
form: 8-K
items: 8.01
row 251:
accessionNumber: 0001104659-26-041034
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-08T22:02:20.000Z
form: 8-K
items: 7.01,9.01
row 252:
accessionNumber: 0000093410-26-000108
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-09T11:00:12.000Z
form: 8-K
items: 2.02
row 253:
accessionNumber: 0001652044-26-000034
filingDate: 2026-04-10
reportDate: 2026-04-07
acceptanceDateTime: 2026-04-10T20:16:53.000Z
form: 8-K
items: 5.02
row 254:
accessionNumber: 0001628280-26-024990
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T10:32:42.000Z
form: 8-K
items: 2.02,9.01
row 255:
accessionNumber: 0000200406-26-000076
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T11:35:25.000Z
form: 8-K
items: 2.02,8.01,9.01
row 256:
accessionNumber: 0001104659-26-042880
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T12:04:26.000Z
form: 8-K
items: 7.01,9.01
row 257:
accessionNumber: 0001628280-26-025013
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T14:05:26.000Z
form: 8-K
items: 7.01,9.01
row 258:
accessionNumber: 0000080424-26-000048
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T20:17:07.000Z
form: 8-K
items: 7.01,9.01
row 259:
accessionNumber: 0001628280-26-025108
filingDate: 2026-04-14
reportDate: 2026-04-08
acceptanceDateTime: 2026-04-14T21:01:31.000Z
form: 8-K
items: 5.02
row 260:
accessionNumber: 0000909832-26-000041
filingDate: 2026-04-15
reportDate: 2026-04-15
acceptanceDateTime: 2026-04-15T20:16:27.000Z
form: 8-K
items: 8.01,9.01
row 261:
accessionNumber: 0001193125-26-159326
filingDate: 2026-04-16
reportDate: 2026-04-16
acceptanceDateTime: 2026-04-16T21:15:36.000Z
form: 8-K
items: 8.01,9.01
row 262:
accessionNumber: 0001140361-26-015711
filingDate: 2026-04-20
reportDate: 2026-04-17
acceptanceDateTime: 2026-04-20T21:29:51.000Z
form: 8-K
items: 5.02
row 263:
accessionNumber: 0000731766-26-000121
filingDate: 2026-04-21
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-21T10:02:24.000Z
form: 8-K
items: 2.02,9.01
row 264:
accessionNumber: 0001730168-26-000039
filingDate: 2026-04-21
reportDate: 2026-04-20
acceptanceDateTime: 2026-04-21T20:37:02.000Z
form: 8-K
items: 5.07
row 265:
accessionNumber: 0001628280-26-026551
filingDate: 2026-04-22
reportDate: 2026-04-22
acceptanceDateTime: 2026-04-22T20:10:44.000Z
form: 8-K
items: 2.02,9.01
row 266:
accessionNumber: 0001193125-26-173739
filingDate: 2026-04-23
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-23T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 267:
accessionNumber: 0000080424-26-000056
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T11:01:47.000Z
form: 8-K
items: 2.02,9.01
row 268:
accessionNumber: 0000080424-26-000057
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T14:02:12.000Z
form: 8-K
items: 7.01,9.01
row 269:
accessionNumber: 0000019617-26-000119
filingDate: 2026-04-24
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-24T20:16:13.000Z
form: 8-K
items: 5.03
row 270:
accessionNumber: 0001045810-26-000026
filingDate: 2026-04-27
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-27T20:10:30.000Z
form: 8-K
items: 5.02
row 271:
accessionNumber: 0000200406-26-000089
filingDate: 2026-04-28
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-27T21:33:52.000Z
form: 8-K
items: 5.07,9.01
row 272:
accessionNumber: 0001628280-26-027723
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T11:00:30.000Z
form: 8-K
items: 2.02,9.01
row 273:
accessionNumber: 0001403161-26-000077
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T20:05:56.000Z
form: 8-K
items: 2.02,8.01,9.01
row 274:
accessionNumber: 0001551152-26-000013
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T11:50:28.000Z
form: 8-K
items: 2.02,9.01
row 275:
accessionNumber: 0001652044-26-000043
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:01:35.000Z
form: 8-K
items: 2.02,9.01
row 276:
accessionNumber: 0001193125-26-191457
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:03:31.000Z
form: 8-K
items: 2.02,9.01
row 277:
accessionNumber: 0001628280-26-028364
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:05:41.000Z
form: 8-K
items: 2.02,9.01
row 278:
accessionNumber: 0001018724-26-000012
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:18:55.000Z
form: 8-K
items: 2.02,9.01
row 279:
accessionNumber: 0001104659-26-052081
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T10:53:18.000Z
form: 8-K
items: 2.02,9.01
row 280:
accessionNumber: 0000059478-26-000043
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 281:
accessionNumber: 0001193125-26-194086
filingDate: 2026-04-30
reportDate: 2026-04-27
acceptanceDateTime: 2026-04-30T11:54:16.000Z
form: 8-K
items: 8.01,9.01
row 282:
accessionNumber: 0001141391-26-000029
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T12:03:33.000Z
form: 8-K
items: 2.02,9.01
row 283:
accessionNumber: 0000320193-26-000011
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T20:30:41.000Z
form: 8-K
items: 2.02,9.01
row 284:
accessionNumber: 0000093410-26-000110
filingDate: 2026-05-01
reportDate: 2026-05-01
acceptanceDateTime: 2026-05-01T10:16:43.000Z
form: 8-K
items: 2.02,9.01
row 285:
accessionNumber: 0001628280-26-029230
filingDate: 2026-05-01
reportDate: 2026-04-29
acceptanceDateTime: 2026-05-01T18:01:51.000Z
form: 8-K
items: 5.07
row 286:
accessionNumber: 0000858877-26-000057
filingDate: 2026-05-01
reportDate: 2026-04-27
acceptanceDateTime: 2026-05-01T20:05:06.000Z
form: 8-K
items: 5.02
row 287:
accessionNumber: 0001321655-26-000026
filingDate: 2026-05-04
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-04T20:06:32.000Z
form: 8-K
items: 2.02,7.01,9.01
row 288:
accessionNumber: 0001193125-26-204128
filingDate: 2026-05-04
reportDate: 2026-04-30
acceptanceDateTime: 2026-05-04T20:36:02.000Z
form: 8-K
items: 8.01,9.01
row 289:
accessionNumber: 0000002488-26-000072
filingDate: 2026-05-05
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-05T20:16:06.000Z
form: 8-K
items: 2.02,7.01,9.01
row 290:
accessionNumber: 0001193125-26-211978
filingDate: 2026-05-07
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-07T20:16:48.000Z
form: 8-K
items: 3.03,5.03,8.01,9.01
row 291:
accessionNumber: 0001141391-26-000034
filingDate: 2026-05-07
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-07T20:17:31.000Z
form: 8-K
items: 5.02,9.01
row 292:
accessionNumber: 0001193125-26-212148
filingDate: 2026-05-07
reportDate: 2026-05-02
acceptanceDateTime: 2026-05-07T20:33:34.000Z
form: 8-K
items: 2.02,5.02,5.03,5.07,9.01
row 293:
accessionNumber: 0000059478-26-000048
filingDate: 2026-05-07
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-07T20:41:48.000Z
form: 8-K
items: 5.07
row 294:
accessionNumber: 0001045810-26-000028
filingDate: 2026-05-08
reportDate: 2026-05-07
acceptanceDateTime: 2026-05-08T20:35:07.000Z
form: 8-K
items: 5.02
row 295:
accessionNumber: 0001193125-26-215875
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T13:10:25.000Z
form: 8-K
items: 7.01,9.01
row 296:
accessionNumber: 0001193125-26-216986
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T20:45:29.000Z
form: 8-K
items: 8.01,9.01
row 297:
accessionNumber: 0000731766-26-000129
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T21:28:55.000Z
form: 8-K
items: 7.01
row 298:
accessionNumber: 0001193125-26-219432
filingDate: 2026-05-12
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-12T20:11:02.000Z
form: 8-K
items: 1.01,8.01,9.01
row 299:
accessionNumber: 0001193125-26-219708
filingDate: 2026-05-12
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-12T20:50:49.000Z
form: 8-K
items: 5.02,7.01,9.01
row 300:
accessionNumber: 0001104659-26-059484
filingDate: 2026-05-12
reportDate: 2026-05-08
acceptanceDateTime: 2026-05-12T21:01:51.000Z
form: 8-K
items: 5.07
row 301:
accessionNumber: 0000858877-26-000075
filingDate: 2026-05-13
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-13T20:06:53.000Z
form: 8-K
items: 2.02,2.05,9.01
row 302:
accessionNumber: 0001193125-26-224155
filingDate: 2026-05-14
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-14T20:28:48.000Z
form: 8-K
items: 5.02,9.01
row 303:
accessionNumber: 0001193125-26-226746
filingDate: 2026-05-15
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-15T20:12:53.000Z
form: 8-K
items: 1.01,1.02,2.03,5.02,5.07,9.01
row 304:
accessionNumber: 0001045810-26-000051
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 305:
accessionNumber: 0001193125-26-232707
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:30:32.000Z
form: 8-K
items: 8.01,9.01
row 306:
accessionNumber: 0000104169-26-000095
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T10:59:53.000Z
form: 8-K
items: 2.02,9.01
row 307:
accessionNumber: 0000019617-26-000228
filingDate: 2026-05-21
reportDate: 2026-05-19
acceptanceDateTime: 2026-05-21T20:15:13.000Z
form: 8-K
items: 5.07
row 308:
accessionNumber: 0001193125-26-234488
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T20:25:10.000Z
form: 8-K
items: 8.01,9.01
row 309:
accessionNumber: 0001104659-26-065717
filingDate: 2026-05-22
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-22T20:12:53.000Z
form: 8-K
items: 5.07
row 310:
accessionNumber: 0001628280-26-037738
filingDate: 2026-05-22
reportDate: 2026-05-22
acceptanceDateTime: 2026-05-22T20:21:18.000Z
form: 8-K
items: 8.01,9.01
row 311:
accessionNumber: 0001193125-26-242018
filingDate: 2026-05-27
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-27T20:39:34.000Z
form: 8-K
items: 8.01,9.01
row 312:
accessionNumber: 0001104659-26-067509
filingDate: 2026-05-28
reportDate: 2026-05-26
acceptanceDateTime: 2026-05-28T20:15:25.000Z
form: 8-K
items: 5.07
row 313:
accessionNumber: 0000909832-26-000046
filingDate: 2026-05-28
reportDate: 2026-05-28
acceptanceDateTime: 2026-05-28T20:17:32.000Z
form: 8-K
items: 2.02,9.01
row 314:
accessionNumber: 0000093410-26-000123
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T13:13:55.000Z
form: 8-K
items: 5.02
row 315:
accessionNumber: 0000093410-26-000125
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T14:12:25.000Z
form: 8-K
items: 5.07
row 316:
accessionNumber: 0001628280-26-039193
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T20:16:13.000Z
form: 8-K
items: 5.07
row 317:
accessionNumber: 0001141391-26-000037
filingDate: 2026-06-02
reportDate: 2026-05-29
acceptanceDateTime: 2026-06-02T20:15:00.000Z
form: 8-K
items: 5.02,9.01
row 318:
accessionNumber: 0001193125-26-253533
filingDate: 2026-06-02
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-02T20:15:25.000Z
form: 8-K
items: 8.01,9.01
row 319:
accessionNumber: 0001730168-26-000051
filingDate: 2026-06-03
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-03T20:21:35.000Z
form: 8-K
items: 2.02,8.01,9.01
row 320:
accessionNumber: 0001193125-26-257724
filingDate: 2026-06-04
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-04T21:07:39.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 321:
accessionNumber: 0001193125-26-258667
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T14:36:56.000Z
form: 8-K
items: 5.02
row 322:
accessionNumber: 0000104169-26-000111
filingDate: 2026-06-05
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-05T20:07:36.000Z
form: 8-K
items: 5.03,5.07,9.01
row 323:
accessionNumber: 0000731766-26-000138
filingDate: 2026-06-05
reportDate: 2026-06-01
acceptanceDateTime: 2026-06-05T20:17:52.000Z
form: 8-K
items: 5.07
row 324:
accessionNumber: 0001652044-26-000059
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T20:40:20.000Z
form: 8-K
items: 5.02
row 325:
accessionNumber: 0001193125-26-259830
filingDate: 2026-06-05
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-05T20:52:38.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 326:
accessionNumber: 0001193125-26-261669
filingDate: 2026-06-08
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-08T20:02:24.000Z
form: 8-K
items: 8.01,9.01
row 327:
accessionNumber: 0001321655-26-000033
filingDate: 2026-06-09
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-09T20:05:18.000Z
form: 8-K
items: 5.07
row 328:
accessionNumber: 0001104659-26-071845
filingDate: 2026-06-09
reportDate: 2026-06-09
acceptanceDateTime: 2026-06-09T20:13:47.000Z
form: 8-K
items: 5.02,9.01
row 329:
accessionNumber: 0001104659-26-072140
filingDate: 2026-06-10
reportDate: 2026-06-08
acceptanceDateTime: 2026-06-10T13:00:19.000Z
form: 8-K
items: 1.01,2.03,9.01
row 330:
accessionNumber: 0001193125-26-265848
filingDate: 2026-06-10
reportDate: 2026-06-10
acceptanceDateTime: 2026-06-10T20:13:46.000Z
form: 8-K
items: 2.02,8.01,9.01
row 331:
accessionNumber: 0001193125-26-266777
filingDate: 2026-06-11
reportDate: 2026-06-11
acceptanceDateTime: 2026-06-11T13:07:29.000Z
form: 8-K
items: 8.01,9.01
row 332:
accessionNumber: 0001193125-26-267578
filingDate: 2026-06-11
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-11T20:17:04.000Z
form: 8-K
items: 5.02,5.07,9.01
row 333:
accessionNumber: 0001104659-26-073562
filingDate: 2026-06-12
reportDate: 2026-06-12
acceptanceDateTime: 2026-06-12T21:00:28.000Z
form: 8-K
items: 8.01,9.01
row 334:
accessionNumber: 0001141391-26-000041
filingDate: 2026-06-17
reportDate: 2026-06-16
acceptanceDateTime: 2026-06-17T20:04:44.000Z
form: 8-K
items: 5.07
row 335:
accessionNumber: 0001193125-26-275077
filingDate: 2026-06-18
reportDate: 2026-06-17
acceptanceDateTime: 2026-06-18T13:00:28.000Z
form: 8-K
items: 8.01,9.01
row 336:
accessionNumber: 0001193125-26-275783
filingDate: 2026-06-18
reportDate: 2026-06-15
acceptanceDateTime: 2026-06-18T20:00:24.000Z
form: 8-K
items: 8.01,9.01
row 337:
accessionNumber: 0001104659-26-076067
filingDate: 2026-06-22
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-22T11:11:21.000Z
form: 8-K
items: 7.01,9.01
row 338:
accessionNumber: 0000723125-26-000013
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:02:01.000Z
form: 8-K
items: 2.02,9.01
row 339:
accessionNumber: 0001628280-26-045167
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:06:40.000Z
form: 8-K
items: 8.01,9.01
row 340:
accessionNumber: 0001628280-26-045169
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:07:40.000Z
form: 8-K
items: 7.01,9.01
row 341:
accessionNumber: 0000019617-26-000241
filingDate: 2026-06-25
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-25T11:59:33.000Z
form: 8-K
items: 5.02
row 342:
accessionNumber: 0001552781-26-000366
filingDate: 2026-06-25
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-25T20:19:25.000Z
form: 8-K
items: 5.02,9.01
row 343:
accessionNumber: 0001403161-26-000086
filingDate: 2026-06-26
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-26T20:07:23.000Z
form: 8-K
items: 8.01
row 344:
accessionNumber: 0001045810-26-000056
filingDate: 2026-06-30
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-30T20:27:26.000Z
form: 8-K
items: 5.07
row 345:
accessionNumber: 0000002488-26-000115
filingDate: 2026-07-01
reportDate: 2026-06-26
acceptanceDateTime: 2026-07-01T20:27:26.000Z
form: 8-K
items: 5.02
row 346:
accessionNumber: 0001628280-26-046717
filingDate: 2026-07-02
reportDate: 2026-07-02
acceptanceDateTime: 2026-07-02T13:01:26.000Z
form: 8-K
items: 2.02,9.01
row 347:
accessionNumber: 0001045810-26-000060
filingDate: 2026-07-02
reportDate: 2026-06-28
acceptanceDateTime: 2026-07-02T13:23:16.000Z
form: 8-K
items: 5.02
row 348:
accessionNumber: 0001193125-26-295589
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T12:00:19.000Z
form: 8-K
items: 8.01
row 349:
accessionNumber: 0001551152-26-000021
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T20:12:09.000Z
form: 8-K
items: 2.02,9.01
row 350:
accessionNumber: 0002115436-26-000003
filingDate: 2026-07-07
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-07T20:19:57.000Z
form: 8-K
items: 7.01
row 351:
accessionNumber: 0000909832-26-000060
filingDate: 2026-07-08
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-08T20:18:27.000Z
form: 8-K
items: 8.01,9.01
row 352:
accessionNumber: 0001104659-26-082293
filingDate: 2026-07-09
reportDate: 2026-07-09
acceptanceDateTime: 2026-07-09T20:46:08.000Z
form: 8-K
items: 8.01,9.01
row 353:
accessionNumber: 0001628280-26-048078
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 354:
accessionNumber: 0001628280-26-048086
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T13:52:21.000Z
form: 8-K
items: 7.01,9.01
row 355:
accessionNumber: 0000080424-26-000082
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T20:19:08.000Z
form: 8-K
items: 7.01,9.01
row 356:
accessionNumber: 0000200406-26-000146
filingDate: 2026-07-15
reportDate: 2026-07-15
acceptanceDateTime: 2026-07-15T11:49:04.000Z
form: 8-K
items: 2.02,9.01
row 357:
accessionNumber: 0001403161-26-000096
filingDate: 2026-07-15
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-15T20:23:24.000Z
form: 8-K
items: 5.03,9.01
row 358:
accessionNumber: 0000731766-26-000191
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T10:00:59.000Z
form: 8-K
items: 2.02,9.01
row 359:
accessionNumber: 0001628280-26-048466
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T20:20:56.000Z
form: 8-K
items: 8.01
row 360:
accessionNumber: 0001652044-26-000066
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:01:36.000Z
form: 8-K
items: 2.02,9.01
row 361:
accessionNumber: 0001628280-26-049213
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:35:52.000Z
form: 8-K
items: 2.02,9.01
row 362:
accessionNumber: 0000019617-26-000288
filingDate: 2026-07-23
reportDate: 2026-07-21
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 5.03
row 363:
accessionNumber: 0001193125-26-314128
filingDate: 2026-07-23
reportDate: 2026-07-23
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 8.01,9.01
row 364:
accessionNumber: 0000200406-26-000155
filingDate: 2026-07-28
reportDate: 2026-07-27
acceptanceDateTime: 2026-07-28T00:15:31.000Z
form: 8-K
items: 7.01,9.01
row 365:
accessionNumber: 0001628280-26-049922
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 366:
accessionNumber: 0001403161-26-000103
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T20:05:26.000Z
form: 8-K
items: 2.02,8.01,9.01
row 367:
accessionNumber: 0000080424-26-000093
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:03:12.000Z
form: 8-K
items: 2.02,9.01
row 368:
accessionNumber: 0000080424-26-000094
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:05:06.000Z
form: 8-K
items: 5.02,7.01,9.01
row 369:
accessionNumber: 0000080424-26-000097
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T14:38:23.000Z
form: 8-K
items: 7.01,9.01
row 370:
accessionNumber: 0001628280-26-050596
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:03:23.000Z
form: 8-K
items: 2.02,9.01
row 371:
accessionNumber: 0001193125-26-323632
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:04:53.000Z
form: 8-K
items: 2.02,9.01
row 372:
accessionNumber: 0000200406-26-000163
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T21:25:05.000Z
form: 8-K
items: 7.01,9.01
row 373:
accessionNumber: 0001141391-26-000081
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T12:07:03.000Z
form: 8-K
items: 2.02,9.01
row 374:
accessionNumber: 0001018724-26-000024
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:06:23.000Z
form: 8-K
items: 2.02,9.01
row 375:
accessionNumber: 0000320193-26-000018
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:30:28.000Z
form: 8-K
items: 2.02,9.01
row 376:
accessionNumber: 0000093410-26-000162
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:16:46.000Z
form: 8-K
items: 2.02,9.01
row 377:
accessionNumber: 0002115436-26-000006
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:31:39.000Z
form: 8-K
items: 2.02,7.01
row 378:
accessionNumber: 0001551152-26-000023
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T11:51:32.000Z
form: 8-K
items: 2.02,9.01
row 379:
accessionNumber: 0001321655-26-000039
filingDate: 2026-08-03
reportDate: 2026-08-03
acceptanceDateTime: 2026-08-03T20:06:14.000Z
form: 8-K
items: 2.02,7.01,9.01
row 380:
accessionNumber: 0001104659-26-090045
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T10:47:58.000Z
form: 8-K
items: 2.02,9.01
row 381:
accessionNumber: 0000200406-26-000167
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T12:48:52.000Z
form: 8-K
items: 5.02,9.01
row 382:
accessionNumber: 0000002488-26-000121
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T20:16:24.000Z
form: 8-K
items: 2.02,7.01,9.01
row 383:
accessionNumber: 0000059478-26-000077
filingDate: 2026-08-05
reportDate: 2026-08-05
acceptanceDateTime: 2026-08-05T11:05:09.000Z
form: 8-K
items: 2.02,9.01
row 384:
accessionNumber: 0001104659-26-091269
filingDate: 2026-08-05
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-05T21:17:20.000Z
form: 8-K
items: 8.01,9.01
row 385:
accessionNumber: 0001193125-26-342390
filingDate: 2026-08-10
reportDate: 2026-08-10
acceptanceDateTime: 2026-08-10T20:10:48.000Z
form: 8-K
items: 8.01,9.01
row 386:
accessionNumber: 0001193125-26-344495
filingDate: 2026-08-11
reportDate: 2026-08-08
acceptanceDateTime: 2026-08-11T19:52:27.000Z
form: 8-K
items: 2.02,9.01
row 387:
accessionNumber: 0000858877-26-000106
filingDate: 2026-08-12
reportDate: 2026-08-12
acceptanceDateTime: 2026-08-12T20:07:06.000Z
form: 8-K
items: 2.02,9.01
row 388:
accessionNumber: 0001045810-26-000069
filingDate: 2026-08-17
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-17T12:41:33.000Z
form: 8-K
items: 1.01,2.03,7.01
row 389:
accessionNumber: 0001193125-26-354029
filingDate: 2026-08-17
reportDate: 2026-08-13
acceptanceDateTime: 2026-08-17T20:05:40.000Z
form: 8-K
items: 1.01,2.03,9.01
row 390:
accessionNumber: 0001104659-26-098367
filingDate: 2026-08-18
reportDate: 2026-08-18
acceptanceDateTime: 2026-08-18T20:30:26.000Z
form: 8-K
items: 8.01,9.01
row 391:
accessionNumber: 0000002488-26-000163
filingDate: 2026-08-19
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-19T20:16:56.000Z
form: 8-K
items: 5.02,9.01
row 392:
accessionNumber: 0000104169-26-000145
filingDate: 2026-08-20
reportDate: 2026-08-20
acceptanceDateTime: 2026-08-20T10:59:01.000Z
form: 8-K
items: 2.02,9.01
row 393:
accessionNumber: 0001104659-26-101067
filingDate: 2026-08-26
reportDate: 2026-08-24
acceptanceDateTime: 2026-08-26T12:06:55.000Z
form: 8-K
items: 5.02,9.01
row 394:
accessionNumber: 0001045810-26-000073
filingDate: 2026-08-26
reportDate: 2026-08-26
acceptanceDateTime: 2026-08-26T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 395:
accessionNumber: 0001193125-26-373026
filingDate: 2026-08-28
reportDate: 2026-08-28
acceptanceDateTime: 2026-08-28T15:26:26.000Z
form: 8-K
items: 8.01,9.01
row 396:
accessionNumber: 0001140361-26-035325
filingDate: 2026-09-01
reportDate: 2026-04-17
acceptanceDateTime: 2026-09-01T20:30:35.000Z
form: 8-K/A
items: 5.02
row 397:
accessionNumber: 0001730168-26-000076
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:26:04.000Z
form: 8-K
items: 2.02,8.01,9.01
row 398:
accessionNumber: 0001193125-26-380280
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:30:24.000Z
form: 8-K
items: 7.01,9.01
row 399:
accessionNumber: 0001045810-26-000078
filingDate: 2026-09-03
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-03T12:03:56.000Z
form: 8-K
items: 8.01
row 400:
accessionNumber: 0001104659-26-104940
filingDate: 2026-09-03
reportDate: 2026-09-03
acceptanceDateTime: 2026-09-03T12:47:46.000Z
form: 8-K
items: 7.01,9.01
row 401:
accessionNumber: 0000731766-26-000205
filingDate: 2026-09-08
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-08T20:04:56.000Z
form: 8-K
items: 7.01
row 402:
accessionNumber: 0001018724-26-000036
filingDate: 2026-09-09
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-09T20:28:21.000Z
form: 8-K
items: 5.02
row 403:
accessionNumber: 0001193125-26-387905
filingDate: 2026-09-10
reportDate: 2026-09-10
acceptanceDateTime: 2026-09-10T20:16:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 404:
accessionNumber: 0001193125-26-389753
filingDate: 2026-09-14
reportDate: 2026-09-12
acceptanceDateTime: 2026-09-14T10:01:59.000Z
form: 8-K
items: 8.01,9.01
row 405:
accessionNumber: 0001104659-26-107526
filingDate: 2026-09-14
reportDate: 2026-09-14
acceptanceDateTime: 2026-09-14T20:45:41.000Z
form: 8-K
items: 8.01,9.01
row 406:
accessionNumber: 0001403161-26-000121
filingDate: 2026-09-23
reportDate: 2026-09-18
acceptanceDateTime: 2026-09-23T20:06:31.000Z
form: 8-K
items: 8.01
row 407:
accessionNumber: 0000909832-26-000084
filingDate: 2026-09-24
reportDate: 2026-09-24
acceptanceDateTime: 2026-09-24T20:17:37.000Z
form: 8-K
items: 2.02,9.01
row 408:
accessionNumber: 0001193125-26-402986
filingDate: 2026-09-25
reportDate: 2026-09-25
acceptanceDateTime: 2026-09-25T21:20:49.000Z
form: 8-K
items: 8.01,9.01
row 409:
accessionNumber: 0000002488-26-000182
filingDate: 2026-09-28
reportDate: 2026-09-26
acceptanceDateTime: 2026-09-28T20:16:47.000Z
form: 8-K
items: 3.02
row 410:
accessionNumber: 0001628280-26-063820
filingDate: 2026-09-29
reportDate: 2026-09-29
acceptanceDateTime: 2026-09-29T20:38:50.000Z
form: 8-K
items: 1.01,1.02,2.03,9.01
row 411:
accessionNumber: 0000723125-26-000018
filingDate: 2026-09-30
reportDate: 2026-09-30
acceptanceDateTime: 2026-09-30T20:02:22.000Z
form: 8-K
items: 2.02,9.01
row 412:
accessionNumber: 0001628280-26-064366
filingDate: 2026-10-02
reportDate: 2026-10-02
acceptanceDateTime: 2026-10-02T13:04:26.000Z
form: 8-K
items: 2.02,9.01
row 413:
accessionNumber: 0000093410-26-000188
filingDate: 2026-10-05
reportDate: 2026-09-30
acceptanceDateTime: 2026-10-05T13:01:20.000Z
form: 8-K
items: 5.02
row 414:
accessionNumber: 0001551152-26-000030
filingDate: 2026-10-05
reportDate: 2026-10-05
acceptanceDateTime: 2026-10-05T20:07:45.000Z
form: 8-K
items: 2.02,9.01
row 415:
accessionNumber: 0000093410-26-000192
filingDate: 2026-10-06
reportDate: 2026-10-06
acceptanceDateTime: 2026-10-06T21:16:59.000Z
form: 8-K
items: 7.01,8.01,9.01
row 416:
accessionNumber: 0000858877-26-000156
filingDate: 2026-10-09
reportDate: 2026-10-07
acceptanceDateTime: 2026-10-09T20:08:49.000Z
form: 8-K
items: 5.02
row 417:
accessionNumber: 0000731766-26-000255
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:14:45.000Z
form: 8-K
items: 2.02,9.01
row 418:
accessionNumber: 0001628280-26-065582
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 419:
accessionNumber: 0000200406-26-000189
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T12:12:35.000Z
form: 8-K
items: 2.02,9.01
row 420:
accessionNumber: 0001628280-26-065616
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T13:38:53.000Z
form: 8-K
items: 7.01,9.01
row 421:
accessionNumber: 0000080424-26-000214
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T14:01:56.000Z
form: 8-K
items: 7.01,9.01
row 422:
accessionNumber: 0000310158-26-000237
filingDate: 2026-10-13
reportDate: 2026-10-09
acceptanceDateTime: 2026-10-13T16:36:57.000Z
form: 8-K
items: 5.02
row 423:
accessionNumber: 0000909832-26-000096
filingDate: 2026-10-14
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-14T20:16:05.000Z
form: 8-K
items: 8.01,9.01
row 424:
accessionNumber: 0001104659-26-116227
filingDate: 2026-10-15
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-15T20:00:53.000Z
form: 8-K
items: 5.02
row 425:
accessionNumber: 0002115436-26-000013
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T12:02:58.000Z
form: 8-K
items: 7.01
row 426:
accessionNumber: 0000080424-26-000245
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T20:25:47.000Z
form: 8-K
items: 5.07
row 427:
accessionNumber: 0000909832-26-000100
filingDate: 2026-10-16
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-16T20:52:57.000Z
form: 8-K
items: 5.02,9.01
row 428:
accessionNumber: 0001193125-26-426704
filingDate: 2026-10-20
reportDate: 2026-10-20
acceptanceDateTime: 2026-10-20T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 429:
accessionNumber: 0001628280-26-066700
filingDate: 2026-10-21
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-21T20:03:35.000Z
form: 8-K
items: 1.01,2.02,8.01,9.01
row 430:
accessionNumber: 0001628280-26-066738
filingDate: 2026-10-21
reportDate: 2026-10-21
acceptanceDateTime: 2026-10-21T20:41:42.000Z
form: 8-K
items: 2.02,9.01
row 431:
accessionNumber: 0000080424-26-000250
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T11:02:49.000Z
form: 8-K
items: 2.02,9.01
row 432:
accessionNumber: 0000080424-26-000252
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T14:29:34.000Z
form: 8-K
items: 7.01,9.01
row 433:
accessionNumber: 0001193125-26-429539
filingDate: 2026-10-23
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-23T13:04:03.000Z
form: 8-K
items: 8.01,9.01
row 434:
accessionNumber: 0001628280-26-067403
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 435:
accessionNumber: 0001403161-26-000126
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T20:05:22.000Z
form: 8-K
items: 2.02,8.01,9.01
row 436:
accessionNumber: 0001193125-26-434271
filingDate: 2026-10-27
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-27T20:23:36.000Z
form: 8-K
items: 2.03
row 437:
accessionNumber: 0001193125-26-435853
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T18:24:44.000Z
form: 8-K
items: 7.01,9.01
row 438:
accessionNumber: 0001652044-26-000080
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:01:33.000Z
form: 8-K
items: 2.02,9.01
row 439:
accessionNumber: 0001193125-26-436122
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:04:44.000Z
form: 8-K
items: 2.02,9.01
row 440:
accessionNumber: 0001193125-26-436149
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:11:03.000Z
form: 8-K
items: 8.01,9.01
row 441:
accessionNumber: 0001104659-26-119825
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T10:43:01.000Z
form: 8-K
items: 2.02,9.01
row 442:
accessionNumber: 0000059478-26-000104
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 443:
accessionNumber: 0001141391-26-000122
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T12:04:22.000Z
form: 8-K
items: 2.02,9.01
row 444:
accessionNumber: 0001018724-26-000038
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T20:05:27.000Z
form: 8-K
items: 2.02,9.01
row 445:
accessionNumber: 0001193125-26-438017
filingDate: 2026-10-29
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-29T21:08:00.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 446:
accessionNumber: 0000093410-26-000196
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:16:00.000Z
form: 8-K
items: 2.02,9.01
row 447:
accessionNumber: 0002115436-26-000018
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:32:50.000Z
form: 8-K
items: 2.02,7.01
row 448:
accessionNumber: 0001551152-26-000033
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T11:51:51.000Z
form: 8-K
items: 2.02,9.01
row 449:
accessionNumber: 0001628280-26-068591
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T20:23:07.000Z
form: 8-K
items: 8.01,9.01
row 450:
accessionNumber: 0001104659-26-121322
filingDate: 2026-11-02
reportDate: 2026-10-28
acceptanceDateTime: 2026-11-02T21:05:38.000Z
form: 8-K
items: 5.02
row 451:
accessionNumber: 0001321655-26-000045
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:06:48.000Z
form: 8-K
items: 2.02,7.01,9.01
row 452:
accessionNumber: 0000320193-26-000024
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:30:23.000Z
form: 8-K
items: 2.02,9.01
row 453:
accessionNumber: 0001628280-26-068909
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:33:15.000Z
form: 8-K
items: 8.01,9.01
row 454:
accessionNumber: 0000002488-26-000188
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:16:27.000Z
form: 8-K
items: 2.02,7.01,9.01
row 455:
accessionNumber: 0001628280-26-069608
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:42:13.000Z
form: 8-K
items: 8.01,9.01
row 456:
accessionNumber: 0001193125-26-447173
filingDate: 2026-11-04
reportDate: 2026-10-29
acceptanceDateTime: 2026-11-04T21:01:27.000Z
form: 8-K
items: 8.01,9.01
row 457:
accessionNumber: 0001193125-26-447507
filingDate: 2026-11-04
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-04T21:49:48.000Z
form: 8-K
items: 8.01,9.01
row 458:
accessionNumber: 0001193125-26-448357
filingDate: 2026-11-05
reportDate: 2026-11-04
acceptanceDateTime: 2026-11-05T11:01:52.000Z
form: 8-K
items: 5.02
row 459:
accessionNumber: 0001193125-26-449835
filingDate: 2026-11-05
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-05T21:10:44.000Z
form: 8-K
items: 8.01,9.01
row 460:
accessionNumber: 0001104659-26-123389
filingDate: 2026-11-05
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-05T21:33:48.000Z
form: 8-K
items: 5.02,9.01
row 461:
accessionNumber: 0001193125-26-450074
filingDate: 2026-11-05
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-05T21:58:46.000Z
form: 8-K
items: 8.01,9.01
row 462:
accessionNumber: 0001193125-26-452530
filingDate: 2026-11-09
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-09T11:10:14.000Z
form: 8-K
items: 2.02,9.01
row 463:
accessionNumber: 0001140361-26-042798
filingDate: 2026-11-09
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-09T21:30:40.000Z
form: 8-K
items: 8.01,9.01
row 464:
accessionNumber: 0000731766-26-000274
filingDate: 2026-11-09
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-09T21:33:53.000Z
form: 8-K
items: 5.02
row 465:
accessionNumber: 0000909832-26-000134
filingDate: 2026-11-10
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-10T21:16:20.000Z
form: 8-K
items: 5.02,8.01,9.01
row 466:
accessionNumber: 0001045810-26-000082
filingDate: 2026-11-12
reportDate: 2026-11-11
acceptanceDateTime: 2026-11-12T13:52:41.000Z
form: 8-K
items: 5.02,9.01

#### Pull 3 rows

row 0:
accessionNumber: 0001045810-25-000179
filingDate: 2025-07-01
reportDate: 2025-06-25
acceptanceDateTime: 2025-06-30T22:35:29.000Z
form: 8-K
items: 5.07
row 1:
accessionNumber: 0000019617-25-000509
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:30:37.000Z
form: 8-K
items: 8.01,9.01
row 2:
accessionNumber: 0000019617-25-000510
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T20:31:18.000Z
form: 8-K
items: 7.01,9.01
row 3:
accessionNumber: 0001193125-25-154103
filingDate: 2025-07-01
reportDate: 2025-07-01
acceptanceDateTime: 2025-07-01T21:00:47.000Z
form: 8-K
items: 5.03,9.01
row 4:
accessionNumber: 0001628280-25-033842
filingDate: 2025-07-02
reportDate: 2025-07-02
acceptanceDateTime: 2025-07-02T13:05:13.000Z
form: 8-K
items: 2.02,9.01
row 5:
accessionNumber: 0000002488-25-000099
filingDate: 2025-07-02
reportDate: 2025-06-27
acceptanceDateTime: 2025-07-02T20:14:22.000Z
form: 8-K
items: 5.02
row 6:
accessionNumber: 0001551152-25-000034
filingDate: 2025-07-03
reportDate: 2025-07-03
acceptanceDateTime: 2025-07-03T17:07:55.000Z
form: 8-K
items: 2.02,9.01
row 7:
accessionNumber: 0000080424-25-000057
filingDate: 2025-07-08
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-08T20:20:53.000Z
form: 8-K
items: 7.01,9.01
row 8:
accessionNumber: 0001140361-25-025275
filingDate: 2025-07-09
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-09T01:18:13.000Z
form: 8-K
items: 5.02
row 9:
accessionNumber: 0001628280-25-034692
filingDate: 2025-07-10
reportDate: 2025-07-09
acceptanceDateTime: 2025-07-10T01:18:15.000Z
form: 8-K
items: 5.08
row 10:
accessionNumber: 0001193125-25-158202
filingDate: 2025-07-11
reportDate: 2025-07-11
acceptanceDateTime: 2025-07-11T20:14:59.000Z
form: 8-K
items: 1.02,8.01,9.01
row 11:
accessionNumber: 0000019617-25-000518
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T10:30:58.000Z
form: 8-K
items: 2.02,9.01
row 12:
accessionNumber: 0000019617-25-000520
filingDate: 2025-07-15
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-15T14:36:04.000Z
form: 8-K
items: 7.01,9.01
row 13:
accessionNumber: 0000200406-25-000170
filingDate: 2025-07-16
reportDate: 2025-07-16
acceptanceDateTime: 2025-07-16T12:06:45.000Z
form: 8-K
items: 2.02,9.01
row 14:
accessionNumber: 0000909832-25-000061
filingDate: 2025-07-16
reportDate: 2025-07-15
acceptanceDateTime: 2025-07-16T20:18:04.000Z
form: 8-K
items: 8.01,9.01
row 15:
accessionNumber: 0000950142-25-001949
filingDate: 2025-07-18
reportDate: 2025-07-18
acceptanceDateTime: 2025-07-18T12:40:31.000Z
form: 8-K
items: 7.01,8.01,9.01
row 16:
accessionNumber: 0001104659-25-069019
filingDate: 2025-07-18
reportDate: 2025-07-17
acceptanceDateTime: 2025-07-18T20:05:39.000Z
form: 8-K
items: 5.03,9.01
row 17:
accessionNumber: 0001193125-25-161225
filingDate: 2025-07-18
reportDate: 2025-07-08
acceptanceDateTime: 2025-07-18T20:16:46.000Z
form: 8-K
items: 8.01,9.01
row 18:
accessionNumber: 0000021344-25-000054
filingDate: 2025-07-22
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-22T11:00:23.000Z
form: 8-K
items: 2.02,9.01
row 19:
accessionNumber: 0001652044-25-000056
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:01:33.000Z
form: 8-K
items: 2.02,8.01,9.01
row 20:
accessionNumber: 0001403161-25-000043
filingDate: 2025-07-23
reportDate: 2025-07-22
acceptanceDateTime: 2025-07-23T20:08:09.000Z
form: 8-K
items: 5.03
row 21:
accessionNumber: 0001628280-25-035738
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:14:09.000Z
form: 8-K
items: 2.02,9.01
row 22:
accessionNumber: 0001193125-25-163423
filingDate: 2025-07-23
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-23T20:15:17.000Z
form: 8-K
items: 8.01,9.01
row 23:
accessionNumber: 0000731766-25-000224
filingDate: 2025-07-24
reportDate: 2025-07-23
acceptanceDateTime: 2025-07-24T12:30:24.000Z
form: 8-K
items: 8.01
row 24:
accessionNumber: 0001140361-25-027340
filingDate: 2025-07-25
reportDate: 2025-07-21
acceptanceDateTime: 2025-07-25T20:30:49.000Z
form: 8-K
items: 5.02
row 25:
accessionNumber: 0000080424-25-000061
filingDate: 2025-07-28
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-28T21:03:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 26:
accessionNumber: 0000731766-25-000228
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T10:04:05.000Z
form: 8-K
items: 2.02,9.01
row 27:
accessionNumber: 0001104659-25-071380
filingDate: 2025-07-29
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-29T10:42:43.000Z
form: 8-K
items: 2.02,2.05,9.01
row 28:
accessionNumber: 0000080424-25-000067
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T11:03:15.000Z
form: 8-K
items: 2.02,9.01
row 29:
accessionNumber: 0000080424-25-000069
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T14:51:39.000Z
form: 8-K
items: 7.01,9.01
row 30:
accessionNumber: 0001403161-25-000051
filingDate: 2025-07-29
reportDate: 2025-07-29
acceptanceDateTime: 2025-07-29T20:06:16.000Z
form: 8-K
items: 2.02,8.01,9.01
row 31:
accessionNumber: 0000950142-25-002041
filingDate: 2025-07-29
reportDate: 2025-07-28
acceptanceDateTime: 2025-07-29T20:10:21.000Z
form: 8-K
items: 5.02
row 32:
accessionNumber: 0000950170-25-100226
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:08:53.000Z
form: 8-K
items: 2.02,9.01
row 33:
accessionNumber: 0001628280-25-036719
filingDate: 2025-07-30
reportDate: 2025-07-30
acceptanceDateTime: 2025-07-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 34:
accessionNumber: 0001551152-25-000036
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T11:48:24.000Z
form: 8-K
items: 2.02,9.01
row 35:
accessionNumber: 0001141391-25-000170
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T12:03:19.000Z
form: 8-K
items: 2.02,9.01
row 36:
accessionNumber: 0001018724-25-000084
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:13:17.000Z
form: 8-K
items: 2.02,9.01
row 37:
accessionNumber: 0000320193-25-000071
filingDate: 2025-07-31
reportDate: 2025-07-31
acceptanceDateTime: 2025-07-31T20:30:25.000Z
form: 8-K
items: 2.02,9.01
row 38:
accessionNumber: 0000731766-25-000232
filingDate: 2025-07-31
reportDate: 2025-07-25
acceptanceDateTime: 2025-07-31T21:08:18.000Z
form: 8-K
items: 5.02
row 39:
accessionNumber: 0000093410-25-000058
filingDate: 2025-08-01
reportDate: 2025-08-01
acceptanceDateTime: 2025-08-01T10:17:27.000Z
form: 8-K
items: 2.02,9.01
row 40:
accessionNumber: 0001104659-25-073263
filingDate: 2025-08-04
reportDate: 2025-08-03
acceptanceDateTime: 2025-08-04T10:03:14.000Z
form: 8-K
items: 5.02,7.01,9.01
row 41:
accessionNumber: 0001193125-25-172579
filingDate: 2025-08-04
reportDate: 2025-08-02
acceptanceDateTime: 2025-08-04T19:55:28.000Z
form: 8-K
items: 2.02,9.01
row 42:
accessionNumber: 0001321655-25-000105
filingDate: 2025-08-04
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-04T20:07:52.000Z
form: 8-K
items: 2.02,7.01,9.01
row 43:
accessionNumber: 0000002488-25-000106
filingDate: 2025-08-05
reportDate: 2025-08-05
acceptanceDateTime: 2025-08-05T20:16:31.000Z
form: 8-K
items: 2.02,7.01,9.01
row 44:
accessionNumber: 0001045810-25-000197
filingDate: 2025-08-05
reportDate: 2025-07-31
acceptanceDateTime: 2025-08-05T20:31:08.000Z
form: 8-K
items: 5.02
row 45:
accessionNumber: 0000059478-25-000202
filingDate: 2025-08-07
reportDate: 2025-08-07
acceptanceDateTime: 2025-08-07T11:05:40.000Z
form: 8-K
items: 2.02,9.01
row 46:
accessionNumber: 0000909832-25-000064
filingDate: 2025-08-07
reportDate: 2025-08-04
acceptanceDateTime: 2025-08-07T20:35:32.000Z
form: 8-K
items: 5.02
row 47:
accessionNumber: 0001403161-25-000055
filingDate: 2025-08-08
reportDate: 2025-08-08
acceptanceDateTime: 2025-08-08T20:07:08.000Z
form: 8-K
items: 3.02
row 48:
accessionNumber: 0001104659-25-075940
filingDate: 2025-08-11
reportDate: 2025-08-11
acceptanceDateTime: 2025-08-11T12:05:18.000Z
form: 8-K
items: 7.01,9.01
row 49:
accessionNumber: 0001193125-25-179820
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:11:01.000Z
form: 8-K
items: 2.02,9.01
row 50:
accessionNumber: 0001193125-25-179846
filingDate: 2025-08-13
reportDate: 2025-08-13
acceptanceDateTime: 2025-08-13T20:16:58.000Z
form: 8-K
items: 8.01,9.01
row 51:
accessionNumber: 0000080424-25-000111
filingDate: 2025-08-14
reportDate: 2025-08-14
acceptanceDateTime: 2025-08-14T14:00:31.000Z
form: 8-K
items: 5.02
row 52:
accessionNumber: 0000731766-25-000239
filingDate: 2025-08-20
reportDate: 2025-08-20
acceptanceDateTime: 2025-08-20T20:06:17.000Z
form: 8-K
items: 7.01
row 53:
accessionNumber: 0001193125-25-184093
filingDate: 2025-08-20
reportDate: 2025-08-18
acceptanceDateTime: 2025-08-20T20:16:08.000Z
form: 8-K
items: 8.01,9.01
row 54:
accessionNumber: 0000104169-25-000120
filingDate: 2025-08-21
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-21T10:59:09.000Z
form: 8-K
items: 2.02,9.01
row 55:
accessionNumber: 0000002488-25-000147
filingDate: 2025-08-25
reportDate: 2025-08-22
acceptanceDateTime: 2025-08-25T20:07:00.000Z
form: 8-K
items: 5.02
row 56:
accessionNumber: 0000858877-25-000103
filingDate: 2025-08-25
reportDate: 2025-08-21
acceptanceDateTime: 2025-08-25T20:27:47.000Z
form: 8-K
items: 5.03,9.01
row 57:
accessionNumber: 0001045810-25-000207
filingDate: 2025-08-27
reportDate: 2025-08-27
acceptanceDateTime: 2025-08-27T20:22:14.000Z
form: 8-K
items: 2.02,9.01
row 58:
accessionNumber: 0001652044-25-000067
filingDate: 2025-09-03
reportDate: 2025-09-02
acceptanceDateTime: 2025-09-03T20:30:34.000Z
form: 8-K
items: 8.01
row 59:
accessionNumber: 0001730168-25-000094
filingDate: 2025-09-04
reportDate: 2025-09-04
acceptanceDateTime: 2025-09-04T20:19:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 60:
accessionNumber: 0000104169-25-000143
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:07:39.000Z
form: 8-K
items: 8.01
row 61:
accessionNumber: 0001104659-25-087862
filingDate: 2025-09-05
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-05T20:46:03.000Z
form: 8-K
items: 1.01,9.01
row 62:
accessionNumber: 0001652044-25-000074
filingDate: 2025-09-05
reportDate: 2025-09-05
acceptanceDateTime: 2025-09-05T20:53:32.000Z
form: 8-K
items: 8.01
row 63:
accessionNumber: 0000731766-25-000245
filingDate: 2025-09-08
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T11:00:14.000Z
form: 8-K
items: 7.01
row 64:
accessionNumber: 0000200406-25-000190
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-08T23:55:25.000Z
form: 8-K
items: 5.02
row 65:
accessionNumber: 0000731766-25-000247
filingDate: 2025-09-09
reportDate: 2025-09-08
acceptanceDateTime: 2025-09-09T11:00:13.000Z
form: 8-K/A
items: 7.01
row 66:
accessionNumber: 0001193125-25-199175
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:13:19.000Z
form: 8-K
items: 2.02,8.01,9.01
row 67:
accessionNumber: 0000310158-25-000047
filingDate: 2025-09-09
reportDate: 2025-09-09
acceptanceDateTime: 2025-09-09T20:33:09.000Z
form: 8-K
items: 8.01,9.01
row 68:
accessionNumber: 0001193125-25-199281
filingDate: 2025-09-09
reportDate: 2025-09-03
acceptanceDateTime: 2025-09-09T21:28:00.000Z
form: 8-K
items: 5.02,9.01
row 69:
accessionNumber: 0001193125-25-200108
filingDate: 2025-09-10
reportDate: 2025-09-10
acceptanceDateTime: 2025-09-10T20:16:49.000Z
form: 8-K
items: 8.01,9.01
row 70:
accessionNumber: 0001104659-25-089245
filingDate: 2025-09-11
reportDate: 2025-09-11
acceptanceDateTime: 2025-09-11T11:30:54.000Z
form: 8-K
items: 7.01,9.01
row 71:
accessionNumber: 0000019617-25-000907
filingDate: 2025-09-12
reportDate: 2025-09-12
acceptanceDateTime: 2025-09-12T20:32:01.000Z
form: 8-K
items: 5.03,9.01
row 72:
accessionNumber: 0000104169-25-000151
filingDate: 2025-09-19
reportDate: 2025-09-19
acceptanceDateTime: 2025-09-19T20:04:09.000Z
form: 8-K
items: 8.01
row 73:
accessionNumber: 0001403161-25-000058
filingDate: 2025-09-19
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-19T20:08:17.000Z
form: 8-K
items: 8.01
row 74:
accessionNumber: 0001193125-25-210089
filingDate: 2025-09-22
reportDate: 2025-09-18
acceptanceDateTime: 2025-09-22T12:22:12.000Z
form: 8-K
items: 5.02,7.01,9.01
row 75:
accessionNumber: 0000104169-25-000153
filingDate: 2025-09-22
reportDate: 2025-09-22
acceptanceDateTime: 2025-09-22T20:39:22.000Z
form: 8-K
items: 8.01
row 76:
accessionNumber: 0000723125-25-000024
filingDate: 2025-09-23
reportDate: 2025-09-23
acceptanceDateTime: 2025-09-23T20:02:28.000Z
form: 8-K
items: 2.02,9.01
row 77:
accessionNumber: 0000093410-25-000098
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T12:00:43.000Z
form: 8-K
items: 7.01
row 78:
accessionNumber: 0000909832-25-000093
filingDate: 2025-09-25
reportDate: 2025-09-25
acceptanceDateTime: 2025-09-25T20:16:57.000Z
form: 8-K
items: 2.02,9.01
row 79:
accessionNumber: 0001193125-25-220445
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:05:13.000Z
form: 8-K
items: 8.01,9.01
row 80:
accessionNumber: 0001403161-25-000061
filingDate: 2025-09-26
reportDate: 2025-09-26
acceptanceDateTime: 2025-09-26T20:12:37.000Z
form: 8-K
items: 8.01
row 81:
accessionNumber: 0001403161-25-000064
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:06:58.000Z
form: 8-K
items: 5.02,9.01
row 82:
accessionNumber: 0001193125-25-223202
filingDate: 2025-09-29
reportDate: 2025-09-29
acceptanceDateTime: 2025-09-29T20:08:40.000Z
form: 8-K
items: 8.01,9.01
row 83:
accessionNumber: 0001193125-25-225125
filingDate: 2025-09-30
reportDate: 2025-09-24
acceptanceDateTime: 2025-09-30T20:37:10.000Z
form: 8-K
items: 5.02
row 84:
accessionNumber: 0001628280-25-043530
filingDate: 2025-10-02
reportDate: 2025-10-02
acceptanceDateTime: 2025-10-02T13:04:54.000Z
form: 8-K
items: 2.02,9.01
row 85:
accessionNumber: 0001193125-25-229405
filingDate: 2025-10-03
reportDate: 2025-09-30
acceptanceDateTime: 2025-10-03T14:34:37.000Z
form: 8-K
items: 5.03,9.01
row 86:
accessionNumber: 0001551152-25-000043
filingDate: 2025-10-03
reportDate: 2025-10-03
acceptanceDateTime: 2025-10-03T20:09:03.000Z
form: 8-K
items: 2.02,9.01
row 87:
accessionNumber: 0001193125-25-230895
filingDate: 2025-10-06
reportDate: 2025-10-05
acceptanceDateTime: 2025-10-06T11:04:49.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 88:
accessionNumber: 0001193125-25-231901
filingDate: 2025-10-06
reportDate: 2025-09-18
acceptanceDateTime: 2025-10-06T20:15:26.000Z
form: 8-K/A
items: 5.02
row 89:
accessionNumber: 0001628280-25-044845
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T10:30:57.000Z
form: 8-K
items: 2.02,9.01
row 90:
accessionNumber: 0000200406-25-000201
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T11:22:58.000Z
form: 8-K
items: 2.02,8.01,9.01
row 91:
accessionNumber: 0001628280-25-044887
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T13:49:09.000Z
form: 8-K
items: 7.01,9.01
row 92:
accessionNumber: 0000080424-25-000217
filingDate: 2025-10-14
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-14T14:55:51.000Z
form: 8-K
items: 7.01,9.01
row 93:
accessionNumber: 0000909832-25-000105
filingDate: 2025-10-15
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-15T20:30:30.000Z
form: 8-K
items: 8.01,9.01
row 94:
accessionNumber: 0000080424-25-000235
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:25:14.000Z
form: 8-K
items: 5.02,5.07,9.01
row 95:
accessionNumber: 0001628280-25-045223
filingDate: 2025-10-16
reportDate: 2025-10-16
acceptanceDateTime: 2025-10-16T20:35:16.000Z
form: 8-K
items: 5.02,9.01
row 96:
accessionNumber: 0000858877-25-000145
filingDate: 2025-10-17
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-17T20:13:47.000Z
form: 8-K
items: 5.02
row 97:
accessionNumber: 0000909832-25-000107
filingDate: 2025-10-20
reportDate: 2025-10-14
acceptanceDateTime: 2025-10-20T21:00:26.000Z
form: 8-K
items: 5.02,9.01
row 98:
accessionNumber: 0001628280-25-045577
filingDate: 2025-10-21
reportDate: 2025-10-21
acceptanceDateTime: 2025-10-21T10:59:07.000Z
form: 8-K
items: 2.02,9.01
row 99:
accessionNumber: 0001104659-25-101237
filingDate: 2025-10-21
reportDate: 2025-10-15
acceptanceDateTime: 2025-10-21T20:09:06.000Z
form: 8-K
items: 5.02,9.01
row 100:
accessionNumber: 0001628280-25-045861
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:06:36.000Z
form: 8-K
items: 2.02,9.01
row 101:
accessionNumber: 0001193125-25-246803
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:17:53.000Z
form: 8-K
items: 8.01,9.01
row 102:
accessionNumber: 0000104169-25-000168
filingDate: 2025-10-22
reportDate: 2025-10-22
acceptanceDateTime: 2025-10-22T20:20:22.000Z
form: 8-K
items: 5.02
row 103:
accessionNumber: 0000080424-25-000240
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T11:04:27.000Z
form: 8-K
items: 2.02,9.01
row 104:
accessionNumber: 0000080424-25-000243
filingDate: 2025-10-24
reportDate: 2025-10-24
acceptanceDateTime: 2025-10-24T14:10:46.000Z
form: 8-K
items: 7.01,9.01
row 105:
accessionNumber: 0001193125-25-250803
filingDate: 2025-10-27
reportDate: 2025-10-27
acceptanceDateTime: 2025-10-27T12:49:27.000Z
form: 8-K
items: 2.01,7.01,9.01
row 106:
accessionNumber: 0000731766-25-000301
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T10:02:08.000Z
form: 8-K
items: 2.02,9.01
row 107:
accessionNumber: 0001403161-25-000077
filingDate: 2025-10-28
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-28T20:06:03.000Z
form: 8-K
items: 2.02,8.01,9.01
row 108:
accessionNumber: 0001652044-25-000087
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:01:48.000Z
form: 8-K
items: 2.02,9.01
row 109:
accessionNumber: 0001193125-25-256310
filingDate: 2025-10-29
reportDate: 2025-10-28
acceptanceDateTime: 2025-10-29T20:07:42.000Z
form: 8-K
items: 2.02,7.01,9.01
row 110:
accessionNumber: 0001628280-25-047114
filingDate: 2025-10-29
reportDate: 2025-10-29
acceptanceDateTime: 2025-10-29T20:08:34.000Z
form: 8-K
items: 2.02,9.01
row 111:
accessionNumber: 0001104659-25-103974
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T10:40:38.000Z
form: 8-K
items: 2.02,9.01
row 112:
accessionNumber: 0000059478-25-000251
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T11:03:41.000Z
form: 8-K
items: 2.02,9.01
row 113:
accessionNumber: 0001141391-25-000191
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T12:03:18.000Z
form: 8-K
items: 2.02,9.01
row 114:
accessionNumber: 0001018724-25-000121
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:13:01.000Z
form: 8-K
items: 2.02,9.01
row 115:
accessionNumber: 0000320193-25-000077
filingDate: 2025-10-30
reportDate: 2025-10-30
acceptanceDateTime: 2025-10-30T20:30:35.000Z
form: 8-K
items: 2.02,9.01
row 116:
accessionNumber: 0000093410-25-000103
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T10:16:33.000Z
form: 8-K
items: 2.02,9.01
row 117:
accessionNumber: 0001551152-25-000047
filingDate: 2025-10-31
reportDate: 2025-10-31
acceptanceDateTime: 2025-10-31T11:51:43.000Z
form: 8-K
items: 2.02,9.01
row 118:
accessionNumber: 0000093410-25-000105
filingDate: 2025-11-03
reportDate: 2025-10-29
acceptanceDateTime: 2025-11-03T13:11:08.000Z
form: 8-K
items: 5.02
row 119:
accessionNumber: 0001193125-25-262260
filingDate: 2025-11-03
reportDate: 2025-11-01
acceptanceDateTime: 2025-11-03T18:48:34.000Z
form: 8-K
items: 2.02,9.01
row 120:
accessionNumber: 0001321655-25-000130
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:06:20.000Z
form: 8-K
items: 2.02,7.01,9.01
row 121:
accessionNumber: 0001193125-25-262593
filingDate: 2025-11-03
reportDate: 2025-10-30
acceptanceDateTime: 2025-11-03T21:18:13.000Z
form: 8-K
items: 8.01,9.01
row 122:
accessionNumber: 0001193125-25-262609
filingDate: 2025-11-03
reportDate: 2025-11-03
acceptanceDateTime: 2025-11-03T21:23:10.000Z
form: 8-K
items: 8.01,9.01
row 123:
accessionNumber: 0001193125-25-264728
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:00.000Z
form: 8-K
items: 8.01,9.01
row 124:
accessionNumber: 0000002488-25-000163
filingDate: 2025-11-04
reportDate: 2025-11-04
acceptanceDateTime: 2025-11-04T21:16:10.000Z
form: 8-K
items: 2.02,7.01,9.01
row 125:
accessionNumber: 0001193125-25-269979
filingDate: 2025-11-06
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-06T21:47:26.000Z
form: 8-K
items: 8.01,9.01
row 126:
accessionNumber: 0000731766-25-000308
filingDate: 2025-11-07
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-07T21:13:36.000Z
form: 8-K
items: 7.01
row 127:
accessionNumber: 0001104659-25-108507
filingDate: 2025-11-07
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-07T21:27:23.000Z
form: 8-K
items: 5.02,5.07,9.01
row 128:
accessionNumber: 0001403161-25-000093
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:30:43.000Z
form: 8-K
items: 8.01,9.01
row 129:
accessionNumber: 0001141391-25-000197
filingDate: 2025-11-10
reportDate: 2025-11-10
acceptanceDateTime: 2025-11-10T13:31:40.000Z
form: 8-K
items: 8.01,9.01
row 130:
accessionNumber: 0001193125-25-277624
filingDate: 2025-11-12
reportDate: 2025-11-12
acceptanceDateTime: 2025-11-12T21:15:30.000Z
form: 8-K
items: 2.02,9.01
row 131:
accessionNumber: 0001141391-25-000199
filingDate: 2025-11-12
reportDate: 2025-11-07
acceptanceDateTime: 2025-11-12T22:15:17.000Z
form: 8-K
items: 1.01
row 132:
accessionNumber: 0000731766-25-000310
filingDate: 2025-11-13
reportDate: 2025-11-06
acceptanceDateTime: 2025-11-13T21:02:22.000Z
form: 8-K
items: 5.03
row 133:
accessionNumber: 0000104169-25-000172
filingDate: 2025-11-14
reportDate: 2025-11-11
acceptanceDateTime: 2025-11-14T13:00:30.000Z
form: 8-K
items: 5.02,9.01
row 134:
accessionNumber: 0001045810-25-000228
filingDate: 2025-11-19
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-19T21:20:44.000Z
form: 8-K
items: 2.02,9.01
row 135:
accessionNumber: 0000104169-25-000177
filingDate: 2025-11-20
reportDate: 2025-11-19
acceptanceDateTime: 2025-11-20T11:58:46.000Z
form: 8-K
items: 2.02,3.01,7.01,9.01
row 136:
accessionNumber: 0001104659-25-114647
filingDate: 2025-11-20
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-20T22:00:42.000Z
form: 8-K
items: 8.01,9.01
row 137:
accessionNumber: 0001193125-25-290864
filingDate: 2025-11-21
reportDate: 2025-11-20
acceptanceDateTime: 2025-11-21T15:46:21.000Z
form: 8-K
items: 8.01,9.01
row 138:
accessionNumber: 0000059478-25-000271
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:19:05.000Z
form: 8-K
items: 5.02
row 139:
accessionNumber: 0001193125-25-291441
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T21:26:49.000Z
form: 8-K
items: 5.02,5.07,9.01
row 140:
accessionNumber: 0000731766-25-000314
filingDate: 2025-11-21
reportDate: 2025-11-18
acceptanceDateTime: 2025-11-21T22:20:04.000Z
form: 8-K
items: 5.02
row 141:
accessionNumber: 0001628280-25-055388
filingDate: 2025-12-04
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-04T21:36:38.000Z
form: 8-K
items: 8.01,9.01
row 142:
accessionNumber: 0000093410-25-000122
filingDate: 2025-12-05
reportDate: 2025-12-03
acceptanceDateTime: 2025-12-05T21:21:15.000Z
form: 8-K
items: 5.03,8.01,9.01
row 143:
accessionNumber: 0001140361-25-044561
filingDate: 2025-12-05
reportDate: 2025-12-04
acceptanceDateTime: 2025-12-05T21:31:42.000Z
form: 8-K
items: 5.02
row 144:
accessionNumber: 0000019617-25-001100
filingDate: 2025-12-08
reportDate: 2025-12-07
acceptanceDateTime: 2025-12-08T11:30:37.000Z
form: 8-K
items: 5.02
row 145:
accessionNumber: 0001193125-25-311196
filingDate: 2025-12-08
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-08T21:00:35.000Z
form: 8-K
items: 5.02,5.07
row 146:
accessionNumber: 0001193125-25-312771
filingDate: 2025-12-09
reportDate: 2025-12-09
acceptanceDateTime: 2025-12-09T21:18:53.000Z
form: 8-K
items: 8.01,9.01
row 147:
accessionNumber: 0001193125-25-314207
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T21:14:38.000Z
form: 8-K
items: 2.02,8.01,9.01
row 148:
accessionNumber: 0001552781-25-000454
filingDate: 2025-12-10
reportDate: 2025-12-10
acceptanceDateTime: 2025-12-10T22:19:43.000Z
form: 8-K
items: 5.02,9.01
row 149:
accessionNumber: 0001193125-25-314935
filingDate: 2025-12-11
reportDate: 2025-12-08
acceptanceDateTime: 2025-12-11T11:02:16.000Z
form: 8-K
items: 5.02,9.01
row 150:
accessionNumber: 0001730168-25-000116
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:17:37.000Z
form: 8-K
items: 2.02,8.01,9.01
row 151:
accessionNumber: 0000909832-25-000164
filingDate: 2025-12-11
reportDate: 2025-12-11
acceptanceDateTime: 2025-12-11T21:22:04.000Z
form: 8-K
items: 2.02,9.01
row 152:
accessionNumber: 0001628280-25-056768
filingDate: 2025-12-12
reportDate: 2025-12-05
acceptanceDateTime: 2025-12-12T21:14:29.000Z
form: 8-K
items: 8.01,9.01
row 153:
accessionNumber: 0000080424-25-000287
filingDate: 2025-12-15
reportDate: 2025-12-15
acceptanceDateTime: 2025-12-15T14:15:22.000Z
form: 8-K
items: 5.02
row 154:
accessionNumber: 0000002488-25-000182
filingDate: 2025-12-15
reportDate: 2025-12-12
acceptanceDateTime: 2025-12-15T21:12:11.000Z
form: 8-K
items: 5.02,9.01
row 155:
accessionNumber: 0000723125-25-000044
filingDate: 2025-12-17
reportDate: 2025-12-17
acceptanceDateTime: 2025-12-17T21:03:26.000Z
form: 8-K
items: 2.02,9.01
row 156:
accessionNumber: 0000858877-25-000199
filingDate: 2025-12-17
reportDate: 2025-12-16
acceptanceDateTime: 2025-12-17T21:42:08.000Z
form: 8-K
items: 5.02,5.07,9.01
row 157:
accessionNumber: 0000093410-25-000130
filingDate: 2025-12-19
reportDate: 2025-07-28
acceptanceDateTime: 2025-12-19T21:25:35.000Z
form: 8-K/A
items: 5.02
row 158:
accessionNumber: 0001628280-25-058337
filingDate: 2025-12-19
reportDate: 2025-12-19
acceptanceDateTime: 2025-12-19T22:00:37.000Z
form: 8-K
items: 5.02
row 159:
accessionNumber: 0001403161-25-000134
filingDate: 2025-12-23
reportDate: 2025-12-23
acceptanceDateTime: 2025-12-23T21:06:56.000Z
form: 8-K
items: 8.01
row 160:
accessionNumber: 0000104169-25-000238
filingDate: 2025-12-29
reportDate: 2025-12-24
acceptanceDateTime: 2025-12-29T21:40:38.000Z
form: 8-K
items: 8.01
row 161:
accessionNumber: 0001403161-25-000137
filingDate: 2025-12-30
reportDate: 2025-12-30
acceptanceDateTime: 2025-12-30T21:07:17.000Z
form: 8-K
items: 8.01
row 162:
accessionNumber: 0001628280-26-000016
filingDate: 2026-01-02
reportDate: 2026-01-02
acceptanceDateTime: 2026-01-02T14:20:13.000Z
form: 8-K
items: 2.02,9.01
row 163:
accessionNumber: 0001140361-26-000199
filingDate: 2026-01-02
reportDate: 2025-12-30
acceptanceDateTime: 2026-01-02T21:30:52.000Z
form: 8-K
items: 5.02
row 164:
accessionNumber: 0001193125-26-004727
filingDate: 2026-01-06
reportDate: 2025-05-03
acceptanceDateTime: 2026-01-06T22:00:33.000Z
form: 8-K/A
items: 5.02
row 165:
accessionNumber: 0001551152-26-000002
filingDate: 2026-01-07
reportDate: 2026-01-07
acceptanceDateTime: 2026-01-07T21:08:59.000Z
form: 8-K
items: 2.02,9.01
row 166:
accessionNumber: 0000104169-26-000008
filingDate: 2026-01-08
reportDate: 2026-01-08
acceptanceDateTime: 2026-01-08T12:59:51.000Z
form: 8-K
items: 5.02,9.01
row 167:
accessionNumber: 0001193125-26-009002
filingDate: 2026-01-09
reportDate: 2026-01-05
acceptanceDateTime: 2026-01-09T21:31:11.000Z
form: 8-K
items: 5.02
row 168:
accessionNumber: 0000731766-26-000020
filingDate: 2026-01-12
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-12T11:58:08.000Z
form: 8-K
items: 7.01
row 169:
accessionNumber: 0001628280-26-001902
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T11:41:09.000Z
form: 8-K
items: 2.02,9.01
row 170:
accessionNumber: 0001628280-26-001915
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T15:09:19.000Z
form: 8-K
items: 7.01,9.01
row 171:
accessionNumber: 0001193125-26-011731
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:06:00.000Z
form: 8-K
items: 8.01,9.01
row 172:
accessionNumber: 0000080424-26-000002
filingDate: 2026-01-13
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-13T21:27:59.000Z
form: 8-K
items: 7.01,9.01
row 173:
accessionNumber: 0001552781-26-000017
filingDate: 2026-01-14
reportDate: 2026-01-13
acceptanceDateTime: 2026-01-14T11:58:41.000Z
form: 8-K
items: 5.02,9.01
row 174:
accessionNumber: 0000104169-26-000023
filingDate: 2026-01-16
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-16T14:01:15.000Z
form: 8-K
items: 5.02,9.01
row 175:
accessionNumber: 0000104169-26-000024
filingDate: 2026-01-16
reportDate: 2025-11-13
acceptanceDateTime: 2026-01-16T14:03:05.000Z
form: 8-K/A
items: 5.02
row 176:
accessionNumber: 0001628280-26-002429
filingDate: 2026-01-16
reportDate: 2026-01-12
acceptanceDateTime: 2026-01-16T21:56:58.000Z
form: 8-K
items: 5.02
row 177:
accessionNumber: 0000002488-26-000002
filingDate: 2026-01-20
reportDate: 2026-01-16
acceptanceDateTime: 2026-01-20T21:19:32.000Z
form: 8-K
items: 5.02,9.01
row 178:
accessionNumber: 0000200406-26-000002
filingDate: 2026-01-21
reportDate: 2026-01-21
acceptanceDateTime: 2026-01-21T12:46:18.000Z
form: 8-K
items: 2.02,9.01
row 179:
accessionNumber: 0001104659-26-005366
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:05:37.000Z
form: 8-K
items: 5.03,5.07,9.01
row 180:
accessionNumber: 0000909832-26-000016
filingDate: 2026-01-21
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-21T21:16:10.000Z
form: 8-K
items: 5.07,8.01
row 181:
accessionNumber: 0000080424-26-000006
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T12:02:05.000Z
form: 8-K
items: 2.02,9.01
row 182:
accessionNumber: 0000080424-26-000009
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T16:53:22.000Z
form: 8-K
items: 7.01,9.01
row 183:
accessionNumber: 0001193125-26-019450
filingDate: 2026-01-22
reportDate: 2026-01-22
acceptanceDateTime: 2026-01-22T21:15:33.000Z
form: 8-K
items: 8.01,9.01
row 184:
accessionNumber: 0000019617-26-000052
filingDate: 2026-01-22
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-22T21:30:18.000Z
form: 8-K
items: 5.02
row 185:
accessionNumber: 0001045810-26-000003
filingDate: 2026-01-23
reportDate: 2026-01-20
acceptanceDateTime: 2026-01-23T22:01:33.000Z
form: 8-K
items: 5.02
row 186:
accessionNumber: 0000731766-26-000025
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T11:02:29.000Z
form: 8-K
items: 2.02,9.01
row 187:
accessionNumber: 0000093410-26-000010
filingDate: 2026-01-27
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-27T21:45:32.000Z
form: 8-K
items: 5.02
row 188:
accessionNumber: 0001628280-26-003832
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:20.000Z
form: 8-K
items: 2.02,9.01
row 189:
accessionNumber: 0001193125-26-027198
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:04:38.000Z
form: 8-K
items: 2.02,9.01
row 190:
accessionNumber: 0001628280-26-003837
filingDate: 2026-01-28
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-28T21:11:04.000Z
form: 8-K
items: 2.02,9.01
row 191:
accessionNumber: 0001403161-26-000029
filingDate: 2026-01-28
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-28T21:43:36.000Z
form: 8-K
items: 5.03,5.07
row 192:
accessionNumber: 0001141391-26-000003
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T13:03:21.000Z
form: 8-K
items: 2.02,9.01
row 193:
accessionNumber: 0001403161-26-000044
filingDate: 2026-01-29
reportDate: 2026-01-27
acceptanceDateTime: 2026-01-29T21:05:49.000Z
form: 8-K
items: 2.02,8.01,9.01
row 194:
accessionNumber: 0000320193-26-000005
filingDate: 2026-01-29
reportDate: 2026-01-29
acceptanceDateTime: 2026-01-29T21:30:33.000Z
form: 8-K
items: 2.02,9.01
row 195:
accessionNumber: 0000093410-26-000019
filingDate: 2026-01-30
reportDate: 2026-01-30
acceptanceDateTime: 2026-01-30T11:16:19.000Z
form: 8-K
items: 2.02,9.01
row 196:
accessionNumber: 0000104169-26-000028
filingDate: 2026-01-30
reportDate: 2026-01-15
acceptanceDateTime: 2026-01-30T21:10:02.000Z
form: 8-K/A
items: 5.02
row 197:
accessionNumber: 0000093410-26-000021
filingDate: 2026-01-30
reportDate: 2026-01-28
acceptanceDateTime: 2026-01-30T21:30:32.000Z
form: 8-K
items: 5.02
row 198:
accessionNumber: 0001321655-26-000004
filingDate: 2026-02-02
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-02T21:06:08.000Z
form: 8-K
items: 2.02,7.01,9.01
row 199:
accessionNumber: 0001104659-26-009495
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T11:38:40.000Z
form: 8-K
items: 2.02,9.01
row 200:
accessionNumber: 0000002488-26-000014
filingDate: 2026-02-03
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-03T21:16:18.000Z
form: 8-K
items: 2.02,7.01,9.01
row 201:
accessionNumber: 0000059478-26-000008
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:05:22.000Z
form: 8-K
items: 2.02,9.01
row 202:
accessionNumber: 0001551152-26-000004
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T12:54:33.000Z
form: 8-K
items: 2.02,9.01
row 203:
accessionNumber: 0001652044-26-000012
filingDate: 2026-02-04
reportDate: 2026-02-04
acceptanceDateTime: 2026-02-04T21:01:37.000Z
form: 8-K
items: 2.02,9.01
row 204:
accessionNumber: 0001193125-26-037840
filingDate: 2026-02-04
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-04T22:20:31.000Z
form: 8-K
items: 1.01,8.01,9.01
row 205:
accessionNumber: 0001193125-26-039344
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:01:31.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 206:
accessionNumber: 0001141391-26-000006
filingDate: 2026-02-05
reportDate: 2026-02-02
acceptanceDateTime: 2026-02-05T21:04:53.000Z
form: 8-K
items: 5.02
row 207:
accessionNumber: 0001193125-26-039427
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:17:31.000Z
form: 8-K
items: 8.01,9.01
row 208:
accessionNumber: 0001018724-26-000002
filingDate: 2026-02-05
reportDate: 2026-02-05
acceptanceDateTime: 2026-02-05T21:25:12.000Z
form: 8-K
items: 2.02,9.01
row 209:
accessionNumber: 0001628280-26-006642
filingDate: 2026-02-10
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-10T11:59:38.000Z
form: 8-K
items: 2.02,9.01
row 210:
accessionNumber: 0000858877-26-000006
filingDate: 2026-02-11
reportDate: 2026-02-11
acceptanceDateTime: 2026-02-11T21:07:20.000Z
form: 8-K
items: 2.02,9.01
row 211:
accessionNumber: 0001628280-26-007709
filingDate: 2026-02-12
reportDate: 2026-02-03
acceptanceDateTime: 2026-02-12T21:30:37.000Z
form: 8-K
items: 8.01,9.01
row 212:
accessionNumber: 0001403161-26-000049
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T13:45:50.000Z
form: 8-K
items: 7.01
row 213:
accessionNumber: 0001193125-26-051423
filingDate: 2026-02-13
reportDate: 2026-02-13
acceptanceDateTime: 2026-02-13T21:16:46.000Z
form: 8-K
items: 8.01,9.01
row 214:
accessionNumber: 0000002488-26-000029
filingDate: 2026-02-17
reportDate: 2026-02-10
acceptanceDateTime: 2026-02-17T21:21:24.000Z
form: 8-K
items: 5.02
row 215:
accessionNumber: 0000104169-26-000032
filingDate: 2026-02-19
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-19T11:59:55.000Z
form: 8-K
items: 2.02,9.01
row 216:
accessionNumber: 0001628280-26-010052
filingDate: 2026-02-20
reportDate: 2026-02-19
acceptanceDateTime: 2026-02-20T15:10:16.000Z
form: 8-K
items: 5.02,9.01
row 217:
accessionNumber: 0001628280-26-010693
filingDate: 2026-02-23
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-23T21:39:11.000Z
form: 8-K
items: 7.01,9.01
row 218:
accessionNumber: 0000002488-26-000045
filingDate: 2026-02-24
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-24T12:01:06.000Z
form: 8-K
items: 1.01,3.02,7.01,9.01
row 219:
accessionNumber: 0001140361-26-006577
filingDate: 2026-02-24
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-24T21:55:58.000Z
form: 8-K
items: 5.07,9.01
row 220:
accessionNumber: 0000731766-26-000046
filingDate: 2026-02-25
reportDate: 2026-02-23
acceptanceDateTime: 2026-02-25T11:23:37.000Z
form: 8-K
items: 5.02
row 221:
accessionNumber: 0001045810-26-000019
filingDate: 2026-02-25
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-25T21:31:25.000Z
form: 8-K
items: 2.02,9.01
row 222:
accessionNumber: 0001104659-26-020643
filingDate: 2026-02-26
reportDate: 2026-02-24
acceptanceDateTime: 2026-02-26T22:14:40.000Z
form: 8-K
items: 8.01,9.01
row 223:
accessionNumber: 0001104659-26-021050
filingDate: 2026-02-27
reportDate: 2026-02-27
acceptanceDateTime: 2026-02-27T13:36:30.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 224:
accessionNumber: 0001403161-26-000063
filingDate: 2026-02-27
reportDate: 2026-02-25
acceptanceDateTime: 2026-02-27T21:06:59.000Z
form: 8-K
items: 8.01
row 225:
accessionNumber: 0000731766-26-000064
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T14:21:03.000Z
form: 8-K
items: 5.02
row 226:
accessionNumber: 0001193125-26-085656
filingDate: 2026-03-02
reportDate: 2026-02-24
acceptanceDateTime: 2026-03-02T22:00:50.000Z
form: 8-K
items: 5.02
row 227:
accessionNumber: 0001193125-26-085801
filingDate: 2026-03-02
reportDate: 2026-02-28
acceptanceDateTime: 2026-03-02T22:27:20.000Z
form: 8-K
items: 2.02,9.01
row 228:
accessionNumber: 0001730168-26-000011
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:16:10.000Z
form: 8-K
items: 2.02,8.01,9.01
row 229:
accessionNumber: 0001104659-26-023534
filingDate: 2026-03-04
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-04T21:59:47.000Z
form: 8-K
items: 8.01,9.01
row 230:
accessionNumber: 0001193125-26-092557
filingDate: 2026-03-05
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-05T12:25:35.000Z
form: 8-K
items: 8.01,9.01
row 231:
accessionNumber: 0000909832-26-000025
filingDate: 2026-03-05
reportDate: 2026-03-05
acceptanceDateTime: 2026-03-05T21:19:07.000Z
form: 8-K
items: 2.02,9.01
row 232:
accessionNumber: 0001045810-26-000024
filingDate: 2026-03-06
reportDate: 2026-03-02
acceptanceDateTime: 2026-03-06T21:11:25.000Z
form: 8-K
items: 5.02,9.01
row 233:
accessionNumber: 0001652044-26-000026
filingDate: 2026-03-06
reportDate: 2026-03-04
acceptanceDateTime: 2026-03-06T22:21:44.000Z
form: 8-K
items: 5.02
row 234:
accessionNumber: 0000731766-26-000067
filingDate: 2026-03-09
reportDate: 2026-03-09
acceptanceDateTime: 2026-03-09T20:33:13.000Z
form: 8-K
items: 7.01
row 235:
accessionNumber: 0001193125-26-100148
filingDate: 2026-03-10
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-10T20:12:51.000Z
form: 8-K
items: 2.02,8.01,9.01
row 236:
accessionNumber: 0000104169-26-000057
filingDate: 2026-03-13
reportDate: 2026-03-10
acceptanceDateTime: 2026-03-13T20:10:19.000Z
form: 8-K
items: 8.01
row 237:
accessionNumber: 0001104659-26-027729
filingDate: 2026-03-13
reportDate: 2026-03-13
acceptanceDateTime: 2026-03-13T21:01:35.000Z
form: 8-K
items: 8.01,9.01
row 238:
accessionNumber: 0001104659-26-028556
filingDate: 2026-03-16
reportDate: 2026-03-16
acceptanceDateTime: 2026-03-16T20:54:55.000Z
form: 8-K
items: 8.01,9.01
row 239:
accessionNumber: 0000723125-26-000004
filingDate: 2026-03-18
reportDate: 2026-03-18
acceptanceDateTime: 2026-03-18T20:02:14.000Z
form: 8-K
items: 2.02,9.01
row 240:
accessionNumber: 0001104659-26-034174
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T12:26:22.000Z
form: 8-K
items: 8.01,9.01
row 241:
accessionNumber: 0000093410-26-000103
filingDate: 2026-03-25
reportDate: 2026-03-25
acceptanceDateTime: 2026-03-25T20:36:44.000Z
form: 8-K
items: 5.03,9.01
row 242:
accessionNumber: 0000104169-26-000067
filingDate: 2026-03-27
reportDate: 2026-03-27
acceptanceDateTime: 2026-03-27T20:10:53.000Z
form: 8-K
items: 8.01
row 243:
accessionNumber: 0001104659-26-038249
filingDate: 2026-04-01
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-01T12:33:36.000Z
form: 8-K
items: 8.01,9.01
row 244:
accessionNumber: 0001628280-26-022956
filingDate: 2026-04-02
reportDate: 2026-04-02
acceptanceDateTime: 2026-04-02T13:07:13.000Z
form: 8-K
items: 2.02,9.01
row 245:
accessionNumber: 0001652044-26-000031
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T20:18:28.000Z
form: 8-K
items: 5.02
row 246:
accessionNumber: 0001193125-26-140574
filingDate: 2026-04-02
reportDate: 2026-03-30
acceptanceDateTime: 2026-04-02T21:25:00.000Z
form: 8-K
items: 5.02
row 247:
accessionNumber: 0001551152-26-000011
filingDate: 2026-04-03
reportDate: 2026-04-03
acceptanceDateTime: 2026-04-03T20:05:55.000Z
form: 8-K
items: 2.02,9.01
row 248:
accessionNumber: 0001193125-26-142939
filingDate: 2026-04-06
reportDate: 2026-04-01
acceptanceDateTime: 2026-04-06T12:12:11.000Z
form: 8-K
items: 5.02,7.01,9.01
row 249:
accessionNumber: 0000858877-26-000048
filingDate: 2026-04-06
reportDate: 2026-03-31
acceptanceDateTime: 2026-04-06T20:29:18.000Z
form: 8-K
items: 5.02
row 250:
accessionNumber: 0001193125-26-144028
filingDate: 2026-04-06
reportDate: 2026-04-06
acceptanceDateTime: 2026-04-06T21:22:08.000Z
form: 8-K
items: 8.01
row 251:
accessionNumber: 0001104659-26-041034
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-08T22:02:20.000Z
form: 8-K
items: 7.01,9.01
row 252:
accessionNumber: 0000093410-26-000108
filingDate: 2026-04-09
reportDate: 2026-04-09
acceptanceDateTime: 2026-04-09T11:00:12.000Z
form: 8-K
items: 2.02
row 253:
accessionNumber: 0001652044-26-000034
filingDate: 2026-04-10
reportDate: 2026-04-07
acceptanceDateTime: 2026-04-10T20:16:53.000Z
form: 8-K
items: 5.02
row 254:
accessionNumber: 0001628280-26-024990
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T10:32:42.000Z
form: 8-K
items: 2.02,9.01
row 255:
accessionNumber: 0000200406-26-000076
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T11:35:25.000Z
form: 8-K
items: 2.02,8.01,9.01
row 256:
accessionNumber: 0001104659-26-042880
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T12:04:26.000Z
form: 8-K
items: 7.01,9.01
row 257:
accessionNumber: 0001628280-26-025013
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T14:05:26.000Z
form: 8-K
items: 7.01,9.01
row 258:
accessionNumber: 0000080424-26-000048
filingDate: 2026-04-14
reportDate: 2026-04-14
acceptanceDateTime: 2026-04-14T20:17:07.000Z
form: 8-K
items: 7.01,9.01
row 259:
accessionNumber: 0001628280-26-025108
filingDate: 2026-04-14
reportDate: 2026-04-08
acceptanceDateTime: 2026-04-14T21:01:31.000Z
form: 8-K
items: 5.02
row 260:
accessionNumber: 0000909832-26-000041
filingDate: 2026-04-15
reportDate: 2026-04-15
acceptanceDateTime: 2026-04-15T20:16:27.000Z
form: 8-K
items: 8.01,9.01
row 261:
accessionNumber: 0001193125-26-159326
filingDate: 2026-04-16
reportDate: 2026-04-16
acceptanceDateTime: 2026-04-16T21:15:36.000Z
form: 8-K
items: 8.01,9.01
row 262:
accessionNumber: 0001140361-26-015711
filingDate: 2026-04-20
reportDate: 2026-04-17
acceptanceDateTime: 2026-04-20T21:29:51.000Z
form: 8-K
items: 5.02
row 263:
accessionNumber: 0000731766-26-000121
filingDate: 2026-04-21
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-21T10:02:24.000Z
form: 8-K
items: 2.02,9.01
row 264:
accessionNumber: 0001730168-26-000039
filingDate: 2026-04-21
reportDate: 2026-04-20
acceptanceDateTime: 2026-04-21T20:37:02.000Z
form: 8-K
items: 5.07
row 265:
accessionNumber: 0001628280-26-026551
filingDate: 2026-04-22
reportDate: 2026-04-22
acceptanceDateTime: 2026-04-22T20:10:44.000Z
form: 8-K
items: 2.02,9.01
row 266:
accessionNumber: 0001193125-26-173739
filingDate: 2026-04-23
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-23T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 267:
accessionNumber: 0000080424-26-000056
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T11:01:47.000Z
form: 8-K
items: 2.02,9.01
row 268:
accessionNumber: 0000080424-26-000057
filingDate: 2026-04-24
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-24T14:02:12.000Z
form: 8-K
items: 7.01,9.01
row 269:
accessionNumber: 0000019617-26-000119
filingDate: 2026-04-24
reportDate: 2026-04-21
acceptanceDateTime: 2026-04-24T20:16:13.000Z
form: 8-K
items: 5.03
row 270:
accessionNumber: 0001045810-26-000026
filingDate: 2026-04-27
reportDate: 2026-04-24
acceptanceDateTime: 2026-04-27T20:10:30.000Z
form: 8-K
items: 5.02
row 271:
accessionNumber: 0000200406-26-000089
filingDate: 2026-04-28
reportDate: 2026-04-23
acceptanceDateTime: 2026-04-27T21:33:52.000Z
form: 8-K
items: 5.07,9.01
row 272:
accessionNumber: 0001628280-26-027723
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T11:00:30.000Z
form: 8-K
items: 2.02,9.01
row 273:
accessionNumber: 0001403161-26-000077
filingDate: 2026-04-28
reportDate: 2026-04-28
acceptanceDateTime: 2026-04-28T20:05:56.000Z
form: 8-K
items: 2.02,8.01,9.01
row 274:
accessionNumber: 0001551152-26-000013
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T11:50:28.000Z
form: 8-K
items: 2.02,9.01
row 275:
accessionNumber: 0001652044-26-000043
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:01:35.000Z
form: 8-K
items: 2.02,9.01
row 276:
accessionNumber: 0001193125-26-191457
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:03:31.000Z
form: 8-K
items: 2.02,9.01
row 277:
accessionNumber: 0001628280-26-028364
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:05:41.000Z
form: 8-K
items: 2.02,9.01
row 278:
accessionNumber: 0001018724-26-000012
filingDate: 2026-04-29
reportDate: 2026-04-29
acceptanceDateTime: 2026-04-29T20:18:55.000Z
form: 8-K
items: 2.02,9.01
row 279:
accessionNumber: 0001104659-26-052081
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T10:53:18.000Z
form: 8-K
items: 2.02,9.01
row 280:
accessionNumber: 0000059478-26-000043
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 281:
accessionNumber: 0001193125-26-194086
filingDate: 2026-04-30
reportDate: 2026-04-27
acceptanceDateTime: 2026-04-30T11:54:16.000Z
form: 8-K
items: 8.01,9.01
row 282:
accessionNumber: 0001141391-26-000029
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T12:03:33.000Z
form: 8-K
items: 2.02,9.01
row 283:
accessionNumber: 0000320193-26-000011
filingDate: 2026-04-30
reportDate: 2026-04-30
acceptanceDateTime: 2026-04-30T20:30:41.000Z
form: 8-K
items: 2.02,9.01
row 284:
accessionNumber: 0000093410-26-000110
filingDate: 2026-05-01
reportDate: 2026-05-01
acceptanceDateTime: 2026-05-01T10:16:43.000Z
form: 8-K
items: 2.02,9.01
row 285:
accessionNumber: 0001628280-26-029230
filingDate: 2026-05-01
reportDate: 2026-04-29
acceptanceDateTime: 2026-05-01T18:01:51.000Z
form: 8-K
items: 5.07
row 286:
accessionNumber: 0000858877-26-000057
filingDate: 2026-05-01
reportDate: 2026-04-27
acceptanceDateTime: 2026-05-01T20:05:06.000Z
form: 8-K
items: 5.02
row 287:
accessionNumber: 0001321655-26-000026
filingDate: 2026-05-04
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-04T20:06:32.000Z
form: 8-K
items: 2.02,7.01,9.01
row 288:
accessionNumber: 0001193125-26-204128
filingDate: 2026-05-04
reportDate: 2026-04-30
acceptanceDateTime: 2026-05-04T20:36:02.000Z
form: 8-K
items: 8.01,9.01
row 289:
accessionNumber: 0000002488-26-000072
filingDate: 2026-05-05
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-05T20:16:06.000Z
form: 8-K
items: 2.02,7.01,9.01
row 290:
accessionNumber: 0001193125-26-211978
filingDate: 2026-05-07
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-07T20:16:48.000Z
form: 8-K
items: 3.03,5.03,8.01,9.01
row 291:
accessionNumber: 0001141391-26-000034
filingDate: 2026-05-07
reportDate: 2026-05-05
acceptanceDateTime: 2026-05-07T20:17:31.000Z
form: 8-K
items: 5.02,9.01
row 292:
accessionNumber: 0001193125-26-212148
filingDate: 2026-05-07
reportDate: 2026-05-02
acceptanceDateTime: 2026-05-07T20:33:34.000Z
form: 8-K
items: 2.02,5.02,5.03,5.07,9.01
row 293:
accessionNumber: 0000059478-26-000048
filingDate: 2026-05-07
reportDate: 2026-05-04
acceptanceDateTime: 2026-05-07T20:41:48.000Z
form: 8-K
items: 5.07
row 294:
accessionNumber: 0001045810-26-000028
filingDate: 2026-05-08
reportDate: 2026-05-07
acceptanceDateTime: 2026-05-08T20:35:07.000Z
form: 8-K
items: 5.02
row 295:
accessionNumber: 0001193125-26-215875
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T13:10:25.000Z
form: 8-K
items: 7.01,9.01
row 296:
accessionNumber: 0001193125-26-216986
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T20:45:29.000Z
form: 8-K
items: 8.01,9.01
row 297:
accessionNumber: 0000731766-26-000129
filingDate: 2026-05-11
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-11T21:28:55.000Z
form: 8-K
items: 7.01
row 298:
accessionNumber: 0001193125-26-219432
filingDate: 2026-05-12
reportDate: 2026-05-11
acceptanceDateTime: 2026-05-12T20:11:02.000Z
form: 8-K
items: 1.01,8.01,9.01
row 299:
accessionNumber: 0001193125-26-219708
filingDate: 2026-05-12
reportDate: 2026-05-06
acceptanceDateTime: 2026-05-12T20:50:49.000Z
form: 8-K
items: 5.02,7.01,9.01
row 300:
accessionNumber: 0001104659-26-059484
filingDate: 2026-05-12
reportDate: 2026-05-08
acceptanceDateTime: 2026-05-12T21:01:51.000Z
form: 8-K
items: 5.07
row 301:
accessionNumber: 0000858877-26-000075
filingDate: 2026-05-13
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-13T20:06:53.000Z
form: 8-K
items: 2.02,2.05,9.01
row 302:
accessionNumber: 0001193125-26-224155
filingDate: 2026-05-14
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-14T20:28:48.000Z
form: 8-K
items: 5.02,9.01
row 303:
accessionNumber: 0001193125-26-226746
filingDate: 2026-05-15
reportDate: 2026-05-13
acceptanceDateTime: 2026-05-15T20:12:53.000Z
form: 8-K
items: 1.01,1.02,2.03,5.02,5.07,9.01
row 304:
accessionNumber: 0001045810-26-000051
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 305:
accessionNumber: 0001193125-26-232707
filingDate: 2026-05-20
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-20T20:30:32.000Z
form: 8-K
items: 8.01,9.01
row 306:
accessionNumber: 0000104169-26-000095
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T10:59:53.000Z
form: 8-K
items: 2.02,9.01
row 307:
accessionNumber: 0000019617-26-000228
filingDate: 2026-05-21
reportDate: 2026-05-19
acceptanceDateTime: 2026-05-21T20:15:13.000Z
form: 8-K
items: 5.07
row 308:
accessionNumber: 0001193125-26-234488
filingDate: 2026-05-21
reportDate: 2026-05-21
acceptanceDateTime: 2026-05-21T20:25:10.000Z
form: 8-K
items: 8.01,9.01
row 309:
accessionNumber: 0001104659-26-065717
filingDate: 2026-05-22
reportDate: 2026-05-20
acceptanceDateTime: 2026-05-22T20:12:53.000Z
form: 8-K
items: 5.07
row 310:
accessionNumber: 0001628280-26-037738
filingDate: 2026-05-22
reportDate: 2026-05-22
acceptanceDateTime: 2026-05-22T20:21:18.000Z
form: 8-K
items: 8.01,9.01
row 311:
accessionNumber: 0001193125-26-242018
filingDate: 2026-05-27
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-27T20:39:34.000Z
form: 8-K
items: 8.01,9.01
row 312:
accessionNumber: 0001104659-26-067509
filingDate: 2026-05-28
reportDate: 2026-05-26
acceptanceDateTime: 2026-05-28T20:15:25.000Z
form: 8-K
items: 5.07
row 313:
accessionNumber: 0000909832-26-000046
filingDate: 2026-05-28
reportDate: 2026-05-28
acceptanceDateTime: 2026-05-28T20:17:32.000Z
form: 8-K
items: 2.02,9.01
row 314:
accessionNumber: 0000093410-26-000123
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T13:13:55.000Z
form: 8-K
items: 5.02
row 315:
accessionNumber: 0000093410-26-000125
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T14:12:25.000Z
form: 8-K
items: 5.07
row 316:
accessionNumber: 0001628280-26-039193
filingDate: 2026-05-29
reportDate: 2026-05-27
acceptanceDateTime: 2026-05-29T20:16:13.000Z
form: 8-K
items: 5.07
row 317:
accessionNumber: 0001141391-26-000037
filingDate: 2026-06-02
reportDate: 2026-05-29
acceptanceDateTime: 2026-06-02T20:15:00.000Z
form: 8-K
items: 5.02,9.01
row 318:
accessionNumber: 0001193125-26-253533
filingDate: 2026-06-02
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-02T20:15:25.000Z
form: 8-K
items: 8.01,9.01
row 319:
accessionNumber: 0001730168-26-000051
filingDate: 2026-06-03
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-03T20:21:35.000Z
form: 8-K
items: 2.02,8.01,9.01
row 320:
accessionNumber: 0001193125-26-257724
filingDate: 2026-06-04
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-04T21:07:39.000Z
form: 8-K
items: 1.01,7.01,8.01,9.01
row 321:
accessionNumber: 0001193125-26-258667
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T14:36:56.000Z
form: 8-K
items: 5.02
row 322:
accessionNumber: 0000104169-26-000111
filingDate: 2026-06-05
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-05T20:07:36.000Z
form: 8-K
items: 5.03,5.07,9.01
row 323:
accessionNumber: 0000731766-26-000138
filingDate: 2026-06-05
reportDate: 2026-06-01
acceptanceDateTime: 2026-06-05T20:17:52.000Z
form: 8-K
items: 5.07
row 324:
accessionNumber: 0001652044-26-000059
filingDate: 2026-06-05
reportDate: 2026-06-02
acceptanceDateTime: 2026-06-05T20:40:20.000Z
form: 8-K
items: 5.02
row 325:
accessionNumber: 0001193125-26-259830
filingDate: 2026-06-05
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-05T20:52:38.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 326:
accessionNumber: 0001193125-26-261669
filingDate: 2026-06-08
reportDate: 2026-06-04
acceptanceDateTime: 2026-06-08T20:02:24.000Z
form: 8-K
items: 8.01,9.01
row 327:
accessionNumber: 0001321655-26-000033
filingDate: 2026-06-09
reportDate: 2026-06-03
acceptanceDateTime: 2026-06-09T20:05:18.000Z
form: 8-K
items: 5.07
row 328:
accessionNumber: 0001104659-26-071845
filingDate: 2026-06-09
reportDate: 2026-06-09
acceptanceDateTime: 2026-06-09T20:13:47.000Z
form: 8-K
items: 5.02,9.01
row 329:
accessionNumber: 0001104659-26-072140
filingDate: 2026-06-10
reportDate: 2026-06-08
acceptanceDateTime: 2026-06-10T13:00:19.000Z
form: 8-K
items: 1.01,2.03,9.01
row 330:
accessionNumber: 0001193125-26-265848
filingDate: 2026-06-10
reportDate: 2026-06-10
acceptanceDateTime: 2026-06-10T20:13:46.000Z
form: 8-K
items: 2.02,8.01,9.01
row 331:
accessionNumber: 0001193125-26-266777
filingDate: 2026-06-11
reportDate: 2026-06-11
acceptanceDateTime: 2026-06-11T13:07:29.000Z
form: 8-K
items: 8.01,9.01
row 332:
accessionNumber: 0001193125-26-267578
filingDate: 2026-06-11
reportDate: 2026-06-05
acceptanceDateTime: 2026-06-11T20:17:04.000Z
form: 8-K
items: 5.02,5.07,9.01
row 333:
accessionNumber: 0001104659-26-073562
filingDate: 2026-06-12
reportDate: 2026-06-12
acceptanceDateTime: 2026-06-12T21:00:28.000Z
form: 8-K
items: 8.01,9.01
row 334:
accessionNumber: 0001141391-26-000041
filingDate: 2026-06-17
reportDate: 2026-06-16
acceptanceDateTime: 2026-06-17T20:04:44.000Z
form: 8-K
items: 5.07
row 335:
accessionNumber: 0001193125-26-275077
filingDate: 2026-06-18
reportDate: 2026-06-17
acceptanceDateTime: 2026-06-18T13:00:28.000Z
form: 8-K
items: 8.01,9.01
row 336:
accessionNumber: 0001193125-26-275783
filingDate: 2026-06-18
reportDate: 2026-06-15
acceptanceDateTime: 2026-06-18T20:00:24.000Z
form: 8-K
items: 8.01,9.01
row 337:
accessionNumber: 0001104659-26-076067
filingDate: 2026-06-22
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-22T11:11:21.000Z
form: 8-K
items: 7.01,9.01
row 338:
accessionNumber: 0000723125-26-000013
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:02:01.000Z
form: 8-K
items: 2.02,9.01
row 339:
accessionNumber: 0001628280-26-045167
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:06:40.000Z
form: 8-K
items: 8.01,9.01
row 340:
accessionNumber: 0001628280-26-045169
filingDate: 2026-06-24
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-24T20:07:40.000Z
form: 8-K
items: 7.01,9.01
row 341:
accessionNumber: 0000019617-26-000241
filingDate: 2026-06-25
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-25T11:59:33.000Z
form: 8-K
items: 5.02
row 342:
accessionNumber: 0001552781-26-000366
filingDate: 2026-06-25
reportDate: 2026-06-18
acceptanceDateTime: 2026-06-25T20:19:25.000Z
form: 8-K
items: 5.02,9.01
row 343:
accessionNumber: 0001403161-26-000086
filingDate: 2026-06-26
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-26T20:07:23.000Z
form: 8-K
items: 8.01
row 344:
accessionNumber: 0001045810-26-000056
filingDate: 2026-06-30
reportDate: 2026-06-24
acceptanceDateTime: 2026-06-30T20:27:26.000Z
form: 8-K
items: 5.07
row 345:
accessionNumber: 0000002488-26-000115
filingDate: 2026-07-01
reportDate: 2026-06-26
acceptanceDateTime: 2026-07-01T20:27:26.000Z
form: 8-K
items: 5.02
row 346:
accessionNumber: 0001628280-26-046717
filingDate: 2026-07-02
reportDate: 2026-07-02
acceptanceDateTime: 2026-07-02T13:01:26.000Z
form: 8-K
items: 2.02,9.01
row 347:
accessionNumber: 0001045810-26-000060
filingDate: 2026-07-02
reportDate: 2026-06-28
acceptanceDateTime: 2026-07-02T13:23:16.000Z
form: 8-K
items: 5.02
row 348:
accessionNumber: 0001193125-26-295589
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T12:00:19.000Z
form: 8-K
items: 8.01
row 349:
accessionNumber: 0001551152-26-000021
filingDate: 2026-07-06
reportDate: 2026-07-06
acceptanceDateTime: 2026-07-06T20:12:09.000Z
form: 8-K
items: 2.02,9.01
row 350:
accessionNumber: 0002115436-26-000003
filingDate: 2026-07-07
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-07T20:19:57.000Z
form: 8-K
items: 7.01
row 351:
accessionNumber: 0000909832-26-000060
filingDate: 2026-07-08
reportDate: 2026-07-07
acceptanceDateTime: 2026-07-08T20:18:27.000Z
form: 8-K
items: 8.01,9.01
row 352:
accessionNumber: 0001104659-26-082293
filingDate: 2026-07-09
reportDate: 2026-07-09
acceptanceDateTime: 2026-07-09T20:46:08.000Z
form: 8-K
items: 8.01,9.01
row 353:
accessionNumber: 0001628280-26-048078
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 354:
accessionNumber: 0001628280-26-048086
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T13:52:21.000Z
form: 8-K
items: 7.01,9.01
row 355:
accessionNumber: 0000080424-26-000082
filingDate: 2026-07-14
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-14T20:19:08.000Z
form: 8-K
items: 7.01,9.01
row 356:
accessionNumber: 0000200406-26-000146
filingDate: 2026-07-15
reportDate: 2026-07-15
acceptanceDateTime: 2026-07-15T11:49:04.000Z
form: 8-K
items: 2.02,9.01
row 357:
accessionNumber: 0001403161-26-000096
filingDate: 2026-07-15
reportDate: 2026-07-14
acceptanceDateTime: 2026-07-15T20:23:24.000Z
form: 8-K
items: 5.03,9.01
row 358:
accessionNumber: 0000731766-26-000191
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T10:00:59.000Z
form: 8-K
items: 2.02,9.01
row 359:
accessionNumber: 0001628280-26-048466
filingDate: 2026-07-16
reportDate: 2026-07-16
acceptanceDateTime: 2026-07-16T20:20:56.000Z
form: 8-K
items: 8.01
row 360:
accessionNumber: 0001652044-26-000066
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:01:36.000Z
form: 8-K
items: 2.02,9.01
row 361:
accessionNumber: 0001628280-26-049213
filingDate: 2026-07-22
reportDate: 2026-07-22
acceptanceDateTime: 2026-07-22T20:35:52.000Z
form: 8-K
items: 2.02,9.01
row 362:
accessionNumber: 0000019617-26-000288
filingDate: 2026-07-23
reportDate: 2026-07-21
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 5.03
row 363:
accessionNumber: 0001193125-26-314128
filingDate: 2026-07-23
reportDate: 2026-07-23
acceptanceDateTime: 2026-07-23T20:15:21.000Z
form: 8-K
items: 8.01,9.01
row 364:
accessionNumber: 0000200406-26-000155
filingDate: 2026-07-28
reportDate: 2026-07-27
acceptanceDateTime: 2026-07-28T00:15:31.000Z
form: 8-K
items: 7.01,9.01
row 365:
accessionNumber: 0001628280-26-049922
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 366:
accessionNumber: 0001403161-26-000103
filingDate: 2026-07-28
reportDate: 2026-07-28
acceptanceDateTime: 2026-07-28T20:05:26.000Z
form: 8-K
items: 2.02,8.01,9.01
row 367:
accessionNumber: 0000080424-26-000093
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:03:12.000Z
form: 8-K
items: 2.02,9.01
row 368:
accessionNumber: 0000080424-26-000094
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T11:05:06.000Z
form: 8-K
items: 5.02,7.01,9.01
row 369:
accessionNumber: 0000080424-26-000097
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T14:38:23.000Z
form: 8-K
items: 7.01,9.01
row 370:
accessionNumber: 0001628280-26-050596
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:03:23.000Z
form: 8-K
items: 2.02,9.01
row 371:
accessionNumber: 0001193125-26-323632
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T20:04:53.000Z
form: 8-K
items: 2.02,9.01
row 372:
accessionNumber: 0000200406-26-000163
filingDate: 2026-07-29
reportDate: 2026-07-29
acceptanceDateTime: 2026-07-29T21:25:05.000Z
form: 8-K
items: 7.01,9.01
row 373:
accessionNumber: 0001141391-26-000081
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T12:07:03.000Z
form: 8-K
items: 2.02,9.01
row 374:
accessionNumber: 0001018724-26-000024
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:06:23.000Z
form: 8-K
items: 2.02,9.01
row 375:
accessionNumber: 0000320193-26-000018
filingDate: 2026-07-30
reportDate: 2026-07-30
acceptanceDateTime: 2026-07-30T20:30:28.000Z
form: 8-K
items: 2.02,9.01
row 376:
accessionNumber: 0000093410-26-000162
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:16:46.000Z
form: 8-K
items: 2.02,9.01
row 377:
accessionNumber: 0002115436-26-000006
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T10:31:39.000Z
form: 8-K
items: 2.02,7.01
row 378:
accessionNumber: 0001551152-26-000023
filingDate: 2026-07-31
reportDate: 2026-07-31
acceptanceDateTime: 2026-07-31T11:51:32.000Z
form: 8-K
items: 2.02,9.01
row 379:
accessionNumber: 0001321655-26-000039
filingDate: 2026-08-03
reportDate: 2026-08-03
acceptanceDateTime: 2026-08-03T20:06:14.000Z
form: 8-K
items: 2.02,7.01,9.01
row 380:
accessionNumber: 0001104659-26-090045
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T10:47:58.000Z
form: 8-K
items: 2.02,9.01
row 381:
accessionNumber: 0000200406-26-000167
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T12:48:52.000Z
form: 8-K
items: 5.02,9.01
row 382:
accessionNumber: 0000002488-26-000121
filingDate: 2026-08-04
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-04T20:16:24.000Z
form: 8-K
items: 2.02,7.01,9.01
row 383:
accessionNumber: 0000059478-26-000077
filingDate: 2026-08-05
reportDate: 2026-08-05
acceptanceDateTime: 2026-08-05T11:05:09.000Z
form: 8-K
items: 2.02,9.01
row 384:
accessionNumber: 0001104659-26-091269
filingDate: 2026-08-05
reportDate: 2026-08-04
acceptanceDateTime: 2026-08-05T21:17:20.000Z
form: 8-K
items: 8.01,9.01
row 385:
accessionNumber: 0001193125-26-342390
filingDate: 2026-08-10
reportDate: 2026-08-10
acceptanceDateTime: 2026-08-10T20:10:48.000Z
form: 8-K
items: 8.01,9.01
row 386:
accessionNumber: 0001193125-26-344495
filingDate: 2026-08-11
reportDate: 2026-08-08
acceptanceDateTime: 2026-08-11T19:52:27.000Z
form: 8-K
items: 2.02,9.01
row 387:
accessionNumber: 0000858877-26-000106
filingDate: 2026-08-12
reportDate: 2026-08-12
acceptanceDateTime: 2026-08-12T20:07:06.000Z
form: 8-K
items: 2.02,9.01
row 388:
accessionNumber: 0001045810-26-000069
filingDate: 2026-08-17
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-17T12:41:33.000Z
form: 8-K
items: 1.01,2.03,7.01
row 389:
accessionNumber: 0001193125-26-354029
filingDate: 2026-08-17
reportDate: 2026-08-13
acceptanceDateTime: 2026-08-17T20:05:40.000Z
form: 8-K
items: 1.01,2.03,9.01
row 390:
accessionNumber: 0001104659-26-098367
filingDate: 2026-08-18
reportDate: 2026-08-18
acceptanceDateTime: 2026-08-18T20:30:26.000Z
form: 8-K
items: 8.01,9.01
row 391:
accessionNumber: 0000002488-26-000163
filingDate: 2026-08-19
reportDate: 2026-08-17
acceptanceDateTime: 2026-08-19T20:16:56.000Z
form: 8-K
items: 5.02,9.01
row 392:
accessionNumber: 0000104169-26-000145
filingDate: 2026-08-20
reportDate: 2026-08-20
acceptanceDateTime: 2026-08-20T10:59:01.000Z
form: 8-K
items: 2.02,9.01
row 393:
accessionNumber: 0001104659-26-101067
filingDate: 2026-08-26
reportDate: 2026-08-24
acceptanceDateTime: 2026-08-26T12:06:55.000Z
form: 8-K
items: 5.02,9.01
row 394:
accessionNumber: 0001045810-26-000073
filingDate: 2026-08-26
reportDate: 2026-08-26
acceptanceDateTime: 2026-08-26T20:21:19.000Z
form: 8-K
items: 2.02,9.01
row 395:
accessionNumber: 0001193125-26-373026
filingDate: 2026-08-28
reportDate: 2026-08-28
acceptanceDateTime: 2026-08-28T15:26:26.000Z
form: 8-K
items: 8.01,9.01
row 396:
accessionNumber: 0001140361-26-035325
filingDate: 2026-09-01
reportDate: 2026-04-17
acceptanceDateTime: 2026-09-01T20:30:35.000Z
form: 8-K/A
items: 5.02
row 397:
accessionNumber: 0001730168-26-000076
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:26:04.000Z
form: 8-K
items: 2.02,8.01,9.01
row 398:
accessionNumber: 0001193125-26-380280
filingDate: 2026-09-02
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-02T20:30:24.000Z
form: 8-K
items: 7.01,9.01
row 399:
accessionNumber: 0001045810-26-000078
filingDate: 2026-09-03
reportDate: 2026-09-02
acceptanceDateTime: 2026-09-03T12:03:56.000Z
form: 8-K
items: 8.01
row 400:
accessionNumber: 0001104659-26-104940
filingDate: 2026-09-03
reportDate: 2026-09-03
acceptanceDateTime: 2026-09-03T12:47:46.000Z
form: 8-K
items: 7.01,9.01
row 401:
accessionNumber: 0000731766-26-000205
filingDate: 2026-09-08
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-08T20:04:56.000Z
form: 8-K
items: 7.01
row 402:
accessionNumber: 0001018724-26-000036
filingDate: 2026-09-09
reportDate: 2026-09-08
acceptanceDateTime: 2026-09-09T20:28:21.000Z
form: 8-K
items: 5.02
row 403:
accessionNumber: 0001193125-26-387905
filingDate: 2026-09-10
reportDate: 2026-09-10
acceptanceDateTime: 2026-09-10T20:16:50.000Z
form: 8-K
items: 2.02,8.01,9.01
row 404:
accessionNumber: 0001193125-26-389753
filingDate: 2026-09-14
reportDate: 2026-09-12
acceptanceDateTime: 2026-09-14T10:01:59.000Z
form: 8-K
items: 8.01,9.01
row 405:
accessionNumber: 0001104659-26-107526
filingDate: 2026-09-14
reportDate: 2026-09-14
acceptanceDateTime: 2026-09-14T20:45:41.000Z
form: 8-K
items: 8.01,9.01
row 406:
accessionNumber: 0001403161-26-000121
filingDate: 2026-09-23
reportDate: 2026-09-18
acceptanceDateTime: 2026-09-23T20:06:31.000Z
form: 8-K
items: 8.01
row 407:
accessionNumber: 0000909832-26-000084
filingDate: 2026-09-24
reportDate: 2026-09-24
acceptanceDateTime: 2026-09-24T20:17:37.000Z
form: 8-K
items: 2.02,9.01
row 408:
accessionNumber: 0001193125-26-402986
filingDate: 2026-09-25
reportDate: 2026-09-25
acceptanceDateTime: 2026-09-25T21:20:49.000Z
form: 8-K
items: 8.01,9.01
row 409:
accessionNumber: 0000002488-26-000182
filingDate: 2026-09-28
reportDate: 2026-09-26
acceptanceDateTime: 2026-09-28T20:16:47.000Z
form: 8-K
items: 3.02
row 410:
accessionNumber: 0001628280-26-063820
filingDate: 2026-09-29
reportDate: 2026-09-29
acceptanceDateTime: 2026-09-29T20:38:50.000Z
form: 8-K
items: 1.01,1.02,2.03,9.01
row 411:
accessionNumber: 0000723125-26-000018
filingDate: 2026-09-30
reportDate: 2026-09-30
acceptanceDateTime: 2026-09-30T20:02:22.000Z
form: 8-K
items: 2.02,9.01
row 412:
accessionNumber: 0001628280-26-064366
filingDate: 2026-10-02
reportDate: 2026-10-02
acceptanceDateTime: 2026-10-02T13:04:26.000Z
form: 8-K
items: 2.02,9.01
row 413:
accessionNumber: 0000093410-26-000188
filingDate: 2026-10-05
reportDate: 2026-09-30
acceptanceDateTime: 2026-10-05T13:01:20.000Z
form: 8-K
items: 5.02
row 414:
accessionNumber: 0001551152-26-000030
filingDate: 2026-10-05
reportDate: 2026-10-05
acceptanceDateTime: 2026-10-05T20:07:45.000Z
form: 8-K
items: 2.02,9.01
row 415:
accessionNumber: 0000093410-26-000192
filingDate: 2026-10-06
reportDate: 2026-10-06
acceptanceDateTime: 2026-10-06T21:16:59.000Z
form: 8-K
items: 7.01,8.01,9.01
row 416:
accessionNumber: 0000858877-26-000156
filingDate: 2026-10-09
reportDate: 2026-10-07
acceptanceDateTime: 2026-10-09T20:08:49.000Z
form: 8-K
items: 5.02
row 417:
accessionNumber: 0000731766-26-000255
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:14:45.000Z
form: 8-K
items: 2.02,9.01
row 418:
accessionNumber: 0001628280-26-065582
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T10:30:38.000Z
form: 8-K
items: 2.02,9.01
row 419:
accessionNumber: 0000200406-26-000189
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T12:12:35.000Z
form: 8-K
items: 2.02,9.01
row 420:
accessionNumber: 0001628280-26-065616
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T13:38:53.000Z
form: 8-K
items: 7.01,9.01
row 421:
accessionNumber: 0000080424-26-000214
filingDate: 2026-10-13
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-13T14:01:56.000Z
form: 8-K
items: 7.01,9.01
row 422:
accessionNumber: 0000310158-26-000237
filingDate: 2026-10-13
reportDate: 2026-10-09
acceptanceDateTime: 2026-10-13T16:36:57.000Z
form: 8-K
items: 5.02
row 423:
accessionNumber: 0000909832-26-000096
filingDate: 2026-10-14
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-14T20:16:05.000Z
form: 8-K
items: 8.01,9.01
row 424:
accessionNumber: 0001104659-26-116227
filingDate: 2026-10-15
reportDate: 2026-10-14
acceptanceDateTime: 2026-10-15T20:00:53.000Z
form: 8-K
items: 5.02
row 425:
accessionNumber: 0002115436-26-000013
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T12:02:58.000Z
form: 8-K
items: 7.01
row 426:
accessionNumber: 0000080424-26-000245
filingDate: 2026-10-16
reportDate: 2026-10-16
acceptanceDateTime: 2026-10-16T20:25:47.000Z
form: 8-K
items: 5.07
row 427:
accessionNumber: 0000909832-26-000100
filingDate: 2026-10-16
reportDate: 2026-10-13
acceptanceDateTime: 2026-10-16T20:52:57.000Z
form: 8-K
items: 5.02,9.01
row 428:
accessionNumber: 0001193125-26-426704
filingDate: 2026-10-20
reportDate: 2026-10-20
acceptanceDateTime: 2026-10-20T20:15:28.000Z
form: 8-K
items: 8.01,9.01
row 429:
accessionNumber: 0001628280-26-066700
filingDate: 2026-10-21
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-21T20:03:35.000Z
form: 8-K
items: 1.01,2.02,8.01,9.01
row 430:
accessionNumber: 0001628280-26-066738
filingDate: 2026-10-21
reportDate: 2026-10-21
acceptanceDateTime: 2026-10-21T20:41:42.000Z
form: 8-K
items: 2.02,9.01
row 431:
accessionNumber: 0000080424-26-000250
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T11:02:49.000Z
form: 8-K
items: 2.02,9.01
row 432:
accessionNumber: 0000080424-26-000252
filingDate: 2026-10-22
reportDate: 2026-10-22
acceptanceDateTime: 2026-10-22T14:29:34.000Z
form: 8-K
items: 7.01,9.01
row 433:
accessionNumber: 0001193125-26-429539
filingDate: 2026-10-23
reportDate: 2026-10-19
acceptanceDateTime: 2026-10-23T13:04:03.000Z
form: 8-K
items: 8.01,9.01
row 434:
accessionNumber: 0001628280-26-067403
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T10:58:13.000Z
form: 8-K
items: 2.02,9.01
row 435:
accessionNumber: 0001403161-26-000126
filingDate: 2026-10-27
reportDate: 2026-10-27
acceptanceDateTime: 2026-10-27T20:05:22.000Z
form: 8-K
items: 2.02,8.01,9.01
row 436:
accessionNumber: 0001193125-26-434271
filingDate: 2026-10-27
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-27T20:23:36.000Z
form: 8-K
items: 2.03
row 437:
accessionNumber: 0001193125-26-435853
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T18:24:44.000Z
form: 8-K
items: 7.01,9.01
row 438:
accessionNumber: 0001652044-26-000080
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:01:33.000Z
form: 8-K
items: 2.02,9.01
row 439:
accessionNumber: 0001193125-26-436122
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:04:44.000Z
form: 8-K
items: 2.02,9.01
row 440:
accessionNumber: 0001193125-26-436149
filingDate: 2026-10-28
reportDate: 2026-10-28
acceptanceDateTime: 2026-10-28T20:11:03.000Z
form: 8-K
items: 8.01,9.01
row 441:
accessionNumber: 0001104659-26-119825
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T10:43:01.000Z
form: 8-K
items: 2.02,9.01
row 442:
accessionNumber: 0000059478-26-000104
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T11:03:30.000Z
form: 8-K
items: 2.02,9.01
row 443:
accessionNumber: 0001141391-26-000122
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T12:04:22.000Z
form: 8-K
items: 2.02,9.01
row 444:
accessionNumber: 0001018724-26-000038
filingDate: 2026-10-29
reportDate: 2026-10-29
acceptanceDateTime: 2026-10-29T20:05:27.000Z
form: 8-K
items: 2.02,9.01
row 445:
accessionNumber: 0001193125-26-438017
filingDate: 2026-10-29
reportDate: 2026-10-26
acceptanceDateTime: 2026-10-29T21:08:00.000Z
form: 8-K
items: 1.01,3.03,5.03,9.01
row 446:
accessionNumber: 0000093410-26-000196
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:16:00.000Z
form: 8-K
items: 2.02,9.01
row 447:
accessionNumber: 0002115436-26-000018
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T10:32:50.000Z
form: 8-K
items: 2.02,7.01
row 448:
accessionNumber: 0001551152-26-000033
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T11:51:51.000Z
form: 8-K
items: 2.02,9.01
row 449:
accessionNumber: 0001628280-26-068591
filingDate: 2026-10-30
reportDate: 2026-10-30
acceptanceDateTime: 2026-10-30T20:23:07.000Z
form: 8-K
items: 8.01,9.01
row 450:
accessionNumber: 0001104659-26-121322
filingDate: 2026-11-02
reportDate: 2026-10-28
acceptanceDateTime: 2026-11-02T21:05:38.000Z
form: 8-K
items: 5.02
row 451:
accessionNumber: 0001321655-26-000045
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:06:48.000Z
form: 8-K
items: 2.02,7.01,9.01
row 452:
accessionNumber: 0000320193-26-000024
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:30:23.000Z
form: 8-K
items: 2.02,9.01
row 453:
accessionNumber: 0001628280-26-068909
filingDate: 2026-11-02
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-02T21:33:15.000Z
form: 8-K
items: 8.01,9.01
row 454:
accessionNumber: 0000002488-26-000188
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:16:27.000Z
form: 8-K
items: 2.02,7.01,9.01
row 455:
accessionNumber: 0001628280-26-069608
filingDate: 2026-11-03
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-03T21:42:13.000Z
form: 8-K
items: 8.01,9.01
row 456:
accessionNumber: 0001193125-26-447173
filingDate: 2026-11-04
reportDate: 2026-10-29
acceptanceDateTime: 2026-11-04T21:01:27.000Z
form: 8-K
items: 8.01,9.01
row 457:
accessionNumber: 0001193125-26-447507
filingDate: 2026-11-04
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-04T21:49:48.000Z
form: 8-K
items: 8.01,9.01
row 458:
accessionNumber: 0001193125-26-448357
filingDate: 2026-11-05
reportDate: 2026-11-04
acceptanceDateTime: 2026-11-05T11:01:52.000Z
form: 8-K
items: 5.02
row 459:
accessionNumber: 0001193125-26-449835
filingDate: 2026-11-05
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-05T21:10:44.000Z
form: 8-K
items: 8.01,9.01
row 460:
accessionNumber: 0001104659-26-123389
filingDate: 2026-11-05
reportDate: 2026-11-02
acceptanceDateTime: 2026-11-05T21:33:48.000Z
form: 8-K
items: 5.02,9.01
row 461:
accessionNumber: 0001193125-26-450074
filingDate: 2026-11-05
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-05T21:58:46.000Z
form: 8-K
items: 8.01,9.01
row 462:
accessionNumber: 0001193125-26-452530
filingDate: 2026-11-09
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-09T11:10:14.000Z
form: 8-K
items: 2.02,9.01
row 463:
accessionNumber: 0001140361-26-042798
filingDate: 2026-11-09
reportDate: 2026-11-05
acceptanceDateTime: 2026-11-09T21:30:40.000Z
form: 8-K
items: 8.01,9.01
row 464:
accessionNumber: 0000731766-26-000274
filingDate: 2026-11-09
reportDate: 2026-11-03
acceptanceDateTime: 2026-11-09T21:33:53.000Z
form: 8-K
items: 5.02
row 465:
accessionNumber: 0000909832-26-000134
filingDate: 2026-11-10
reportDate: 2026-11-07
acceptanceDateTime: 2026-11-10T21:16:20.000Z
form: 8-K
items: 5.02,8.01,9.01
row 466:
accessionNumber: 0001045810-26-000082
filingDate: 2026-11-12
reportDate: 2026-11-11
acceptanceDateTime: 2026-11-12T13:52:41.000Z
form: 8-K
items: 5.02,9.01
row 467:
accessionNumber: 0000858877-26-000170
filingDate: 2026-11-12
reportDate: 2026-11-12
acceptanceDateTime: 2026-11-12T21:06:24.000Z
form: 8-K
items: 2.02,9.01
row 468:
accessionNumber: 0001193125-26-458525
filingDate: 2026-11-12
reportDate: 2026-11-12
acceptanceDateTime: 2026-11-12T21:27:49.000Z
form: 8-K
items: 8.01,9.01

### Per reviewed filing — index and document excerpts

#### Filing 1 — COSTCO WHOLESALE CORP /NEW — accession 0000909832-26-000134

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 8.01: Other Events Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | cost-20261107.htm iXBRL | 8-K | 24303
Index items (from index page): 5.02, 8.01, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On November 7, 2026, Helena B. Foulkes notified the Board of Directors (the “Board”) of Costco Wholesale Corporation (the “Company”) of her decision to resign from the Board and all committees of the Board of which she is a member, effective November 7, 2026. She served on the Board since August 16, 2023 and was a member of the Audit Committee and the Nominating and Governance

Item 8.01 heading: Item 8.01. Other Events
Item 8.01 excerpt: On November 10, 2026, the Board of Directors declared a special cash dividend on the Company's common stock of $30 per share, payable December 4, 2026, to shareholders of record at the close of business on November 24, 2026. A copy of the press release is attached as Exhibit 99.1.

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. 99.1. Press release dated November 10, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

#### Filing 2 — UNITEDHEALTH GROUP INC — accession 0000731766-26-000274

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | unh-20261103.htm iXBRL | 8-K | 33659
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: Madeline Bell as independent director On November 9, 2026, UnitedHealth Group Incorporated (the “Company”) issued a press release announcing the appointment of Madeline Bell to serve as an independent director of the Company, effective November 3, 2026. Ms. Bell has not yet been appointed to any committees of the Company's Board of Directors. A copy of the press release 

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: Exhibit Description 99.1 Press release dated November 9, 2026 104 Cover Page Interactive Data File (formatted as Inline XBRL).

#### Filing 3 — MICRON TECHNOLOGY INC — accession 0001104659-26-123389

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2629062d1_8k.htm iXBRL | 8-K | 30829
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On November 2, 2026, Linnie M. Haynesworth notified the Governance and Sustainability Committee of the Board of Directors (the “Board”) of Micron Technology, Inc. (the “Company”) that she would retire from the Board and, accordingly, Ms. Haynesworth will not be nominated for re-election at the Company’s fiscal 2026 annual shareholders meeting (the “Annual Meeting”). Ms. Haynesworth will continue to serve as a director through the end of her term at the Annual Meeting.

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. Exhibit No. Description 99.1 Press Release issued on November 5, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 4 — MICROSOFT CORP — accession 0001193125-26-448357

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | d177209d8k.htm iXBRL | 8-K | 26217
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: (b) On November 4, 2026, Emma N. Walmsley, a member of the Board of Directors of Microsoft Corporation (the “Company”) since 2019, informed the Company of her decision not to stand for re-election at the Company’s 2026 annual shareholder meeting (the “Annual Meeting”). Ms. Walmsley will continue to serve as a director until the Annual Meeting. Her decision not to stand for re-election is not as a result of any disagreement with management on any matter relating to the Company’s operations, policies, or practices.

#### Filing 5 — AbbVie Inc. — accession 0001104659-26-121322

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2628215d1_8k.htm iXBRL | 8-K | 36234
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02 Departure of
Item 5.02 excerpt: On October 28, 2026, Jennifer L. Davis, a Class II director of AbbVie Inc. (“AbbVie”), notified the Company’s Board of Directors (the “Board”), of her intent to resign from the Board, effective November 2, 2026, in light of her recent appointment as Chief Executive Officer at Align Technology, Inc. Her resignation as a director is not the result of any dispute or disagreement with AbbVie on any matter relating to the operations, policies or practices of AbbVie.

#### Filing 6 — Meta Platforms, Inc. — accession 0001193125-26-438017

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 3.03: Material Modifications to Rights of Security Holders Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | d183592d8k.htm iXBRL | 8-K | 56328
Index items (from index page): 1.01, 3.03, 5.03, 9.01

Item 1.01 heading: Item 1.01. Entry into a Material Definitive Agreement
Item 1.01 excerpt: Mandatory Convertible Preferred Stock Offering On October 26, 2026, Meta Platforms, Inc. (the “Company”) entered into an underwriting agreement (the “Underwriting Agreement (Depositary Shares)”) with Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC as the representatives of the several underwriters named therein (the “Depositary Shares Underwriters”), pursuant to which the Company agreed to issue and sell 250,000,000 Series A depositary shares (the “Depositary Shares”), each representing a 1/20th interest in a share of 6.50% Series A Mandatory Convertible Preferred Stock, liquidation preference $1,000.00 per share, par value $0.000006 per share (the “Preferred Stock” and such offering, the “Depositary Shares Offering”). Pursuant to the Underwriting Agreement (Depositary Shares), the Company granted the Depositary Shares Underwriters an o

Item 3.03 heading: Item 3.03. Material Modification to Rights of Security Holders
Item 3.03 excerpt: On October 28, 2026, the Company filed the Certificates of Designations with the Secretary of State of the State of Delaware to establish the preferences, limitations, and relative rights of the Preferred Stock. The Original Certificate of Designations became effective upon filing, and the Restated Charter Certificate of Designat

Item 5.03 heading: Item 5.03. Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Item 5.03 excerpt: The information set forth under Item 3.03 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 5.03. Forward Looking Statements This Current Report on Form 8-K contains forward-looking statements within the meaning of the Private Securities Litigation Reform Act of 1995 (the “PSLRA”). All statements contained in this Current Report on Form 8-K that do not relate to matters of historical fact should be 

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits 1.1 Underwriting Agreement, dated as of October 26, 2026, by and among Meta Platforms, Inc. and Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as representatives of the several underwriters named therein, relating to the Depositary Shares. 1.2 Underwriting Agreement, dated as of October 26, 2026, by and among Meta Platforms, Inc., Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as representatives of the several underwriters named therein, Morgan Stanley Capital Services LLC and Goldman Sachs & Co. LLC, as forward purchasers, and Morgan Stanley & Co. LLC and Goldman Sachs & Co. LLC, as forward sellers, relating to the Class A Common Stock. 3.1 Original Certificate of Designations for the 6.50% Series A Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective October 28, 2026. 4.1 Form of Certificate for the 6

#### Filing 7 — Broadcom Inc. — accession 0001193125-26-434271

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 2.03: Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant
Documents table row (document whose Type is the form): 1 | 8-K | d148323d8k.htm iXBRL | 8-K | 22351
Index items (from index page): 2.03

Item 2.03 heading: Item 2.03 Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant
Item 2.03 excerpt: On October 26, 2026, Broadcom Inc. (the “Company”) arranged for financial partners to take on a portion of certain agreements to purchase AI racks based on custom AI accelerators designed by the Company and the related lease agreements with the Company’s customer that enable the deployment of compute capacity. In connection with this arrangement, the Company is providing residual value support to a newly formed special purpose 

#### Filing 8 — Meta Platforms, Inc. — accession 0001628280-26-066700

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 2.02: Results of Operations and Financial Condition Item 8.01: Other Events Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | meta-20261019.htm iXBRL | 8-K | 49903
Index items (from index page): 1.01, 2.02, 8.01, 9.01

Item 1.01 heading: Item 1.01. Entry into a Material Definitive Agreement
Item 1.01 excerpt: On October 19, 2026, the board of directors (the “Board”) of Meta Platforms, Inc. (the “Company” or “Meta”) approved and declared advisable, based on the unanimous recommendation of a special committee consisting of disinterested and independent directors established to review such transaction, and recommended to the Company’s shareholders, the amendment and restatement of the Company’s certificate of incorporation (as so amended and restated, the “Restated Charter”) to, among other things, adjust the Company’s capital structure by establishing a new class of non-voting Class C common stock, par value $0.000006 (the “Recapitalization”), which was subsequently approved by the requisite shareholders by written consent on October 20, 2026. The Company expects to file the Restated Charter with the Secretary of State of the State of Delaware on or about Octob

Item 2.02 heading: Item 2.02 Results of Operations and Financial Condition
Item 2.02 excerpt: On October 21, 2026, the Company issued a press release and will hold a conference call regarding its financial results for the quarter ended September 30, 2026. A copy of the press release is furnished as Exhibit 99.1 to this Current Report on Form 8-K. The information furnished 

Item 8.01 heading: Item 8.01 Other Events
Item 8.01 excerpt: As described above, also on October 19, 2026, the Board declared the Stock Dividend, contingent upon the effectiveness of the Restated Charter, with the record date and payment date for the Stock Dividend to be established by the Board by subsequent action. For more information on the non-voting Class C common stock, please refer to the Company’s Preliminary Information Stat

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit Number Exhibit Title or Description 10.1 Founder Alignment Agreement, dated October 20, 2026, by and between Mark Zuckerberg and Meta Platforms, Inc. 99.1 Press release dated October 21, 2026 104 Cover Page Interactive Data File (the cover page XBRL tags are embedded within the inline XBRL document)

#### Filing 9 — COSTCO WHOLESALE CORP /NEW — accession 0000909832-26-000100

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | cost-20261013.htm iXBRL | 8-K | 24574
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On October 13, 2026, the Compensation Committee of the Board of Directors approved the fiscal 2027 criteria for bonuses to executive officers, with the Nominating and Governance Committee of the Board also approving the environmental and social performance criteria. Executive officers other than the Chief Executive Officer are eligible to receive base bonuses of $400,000. The base amounts include $160,000 based on targets relating to sales and $160,000 based on targets relating to pre-tax income. The potential payment attributable to each goal may be from zero to up to 120% of the target amount, based on the level

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. 10.1. Fiscal 2027 Executive Bonus Plan. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

#### Filing 10 — PROCTER & GAMBLE Co — accession 0000080424-26-000245

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.07: Submission of Matters to a Vote of Security Holders
Documents table row (document whose Type is the form): 1 | 8-K | pg-20261016.htm iXBRL | 8-K | 83259
Index items (from index page): 5.07

Item 5.07 heading: Item 5.07. Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: On October 13, 2026, the Company held its 2026 Annual Meeting of Shareholders. Set forth below are the final voting results for each of the proposals submitted to a vote of the shareholders. Proposa

#### Filing 11 — AbbVie Inc. — accession 0001104659-26-116227

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2627361d1_8k.htm iXBRL | 8-K | 36699
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02 Departure of
Item 5.02 excerpt: On October 14, 2026, AbbVie Inc. (“AbbVie”) expanded the size of its Board of Directors (the “Board”) from twelve directors to thirteen directors and appointed Dr. John M. Carethers as a Class II director. Dr. Carethers currently serves as the Vice Chancellor for Health Sciences at the University of California San Diego and was previously a director of Avantor, Inc. Dr. Carethers has been appointed to the Public Policy and Sustainability Committee of AbbVie. The Board affirmatively determined that Dr. Carethers is an “independent director” under each of the standards set forth in section 303A.02 of the New York Stock Exchange Listed Company Manual and AbbVie’s Governance Guidelines and Director Independence Guidelines. Dr. Carethers will be entitled to compensation as an independent director as disclosed in Exhibit 10.5 to AbbVie’s Quar

#### Filing 12 — Merck & Co., Inc. — accession 0000310158-26-000237

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | mrk-20261009.htm iXBRL | 8-K | 34793
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: (d) Incorporated by reference is a press release issued by Merck & Co., Inc. (the “Company”) on October 13, 2026, attached as Exhibit 99.1, announcing the election of Paul J. Diaz to the Company’s Board of Directors (the “Board”), effective November 1, 2026. The Board appointed Mr. Diaz as a member of both the Audit Committee and the Research Committee of the Board. For his s

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit 99.1 Press release issued October 13, 2026 Exhibit 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 13 — CISCO SYSTEMS, INC. — accession 0000858877-26-000156

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | csco-20261007.htm iXBRL | 8-K | 28324
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: Director On October 7, 2026, the Board of Directors (“Board”) of Cisco Systems, Inc. (“Cisco”) appointed Girish D. Rishi, CEO of Cognite Holding B.V., as a member of the Board effective October 9, 2026. In connection with his appointment, the Board determined that Mr. Rishi is “independent” under the applicable listing s

#### Filing 14 — CHEVRON CORP — accession 0000093410-26-000188

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | cvx-20260930.htm iXBRL | 8-K | 28629
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: (b) On September 30, 2026, the Board of Directors (the “Board”) of Chevron Corporation (”Chevron”) approved certain officer elections. Mark A. Nelson, currently Chevron’s Vice Chairman and Executive Vice President of Oil, Products & Gas, will remain Vice Chairman with responsibility for Strategy and Business Development in addition to his corporate duties, and will no longer serve as Executive Vice President, Oil, Products & Gas, in each case, effective January 1, 2027. Further, Eimear P. Bonner, currently Chevron’s Chief Financial Officer, will become President, Oil, Products & Gas, and

#### Filing 15 — Tesla, Inc. — accession 0001628280-26-063820

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 1.02: Termination of a Material Definitive Agreement Item 2.03: Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | tsla-20260929.htm iXBRL | 8-K | 41336
Index items (from index page): 1.01, 1.02, 2.03, 9.01

Item 1.02 heading: Item 1.02 Termination of a Material Definitive Agreement
Item 1.02 excerpt: Revolving Credit Facility As previously reported, Tesla is a party to that certain Credit Agreement, dated as of January 20, 2023 (as further amended from time to time, the “Existing Revolving Credit Agreement”), with Citi, as administrative agent and the lenders and other agents party thereto. The Existing Revolving Credit Agreement had aggregate commitments of $5.0 billion and was set to mature on January 20, 

Item 2.03 heading: Item 2.03 Creation of a Direct Financial Obligation or an Obligation Under an Off-Balance Sheet Arrangement of a Registrant
Item 2.03 excerpt: The information set forth in Item 1.01 above is incorporated herein by reference. Item 9.01 Financial Statements and Exhibits. (d)Exhibits. Exhibit No. Description 104 Cover Page Interactive Data File 

Item 1.01 heading: Item 1.01 Entry Into a Material Definitive Agreement
Item 1.01 excerpt: On September 29, 2026, Tesla, Inc. (“Tesla”) entered into the following credit agreements: •$20.0 billion senior unsecured three-year delayed draw term loan facility (the “Term Loan Facility”) pursuant to a Delayed Draw Term Loan Credit Agreement, dated as of September 29, 2026 (the “DDTL Credit Agreement”), by and among Tesla, as borrower, Citibank, N.A. (“Citi”), as administrative agent, and the lenders and other agents party thereto. •$8.0 billion senior unsecured five-year revolving facility (the “Five-Year Revolving Facility”) pursuant to a Five-Year Revolving Credit Agreement, dated as of September 29, 2026 (the “Five-Year Revolving Credit Agreement”), by and among Tesla, as borrower, Wells Fargo Bank, National Association (“WF Bank”), as administrative agent, and the lenders, issuing banks and other agents party thereto. •$2.0 billion senior unsecured 364-day revolving credit faci

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d)Exhibits. Exhibit No. Description 104 Cover Page Interactive Data File (embedded within the Inline XBRL document).

#### Filing 16 — ADVANCED MICRO DEVICES INC — accession 0000002488-26-000182

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 3.02: Unregistered Sales of Equity Securities
Documents table row (document whose Type is the form): 1 | 8-K | amd-20260926.htm iXBRL | 8-K | 25721
Index items (from index page): 3.02

Item 3.02 heading: Item 3.02 Unregistered Sales of Equity Securities
Item 3.02 excerpt: On September 26, 2026, Advanced Micro Devices, Inc. (the “Company”) entered into an Agreement and Plan of Merger (the “Merger Agreement”) to acquire all of the equity interests in World Labs Technologies, Inc. (“World Labs”) (the “Acquisition”) for a total purchase price of approximately $8.2 billion to be paid in shares of the Company’s common stock, par value $0.01 per share (“Common Stock”), to stockholders of World Labs, subject to customary adjustments. At this time, the number of shares to be issued in connection with the Acquisition is not known and will be calculated 

#### Filing 17 — AMAZON COM INC — accession 0001018724-26-000036

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | amzn-20260908.htm iXBRL | 8-K | 42816
Index items (from index page): 5.02

Item 5.02 heading: ITEM 5.02. DEPARTURE OF DIRECTORS OR CERTAIN OFFICERS; ELECTION OF DIRECTORS; APPOINTMENT OF CERTAIN OFFICERS; COMPENSATORY ARRANGEMENTS OF CERTAIN OFFICERS
Item 5.02 excerpt: On September 8, 2026, the Board of Directors of Amazon.com, Inc. (the “Company”) elected Kevin R. Mandia as a director of the Company and also appointed him to the Audit Committee and Security Committee of the Board. Mr. Mandia has served as Chief Executive Officer of Armadin, Inc., a cybersecurity company he founded, since September 2025. Mr. Mandia has also served as General Partner of Ballistic Ventures, a venture capital firm he co-founded, since June 2024 and previously served as Strategic Partner from December 2021 to June 2024. He served as Chief Executive Officer of Mandiant, Inc., a cybersecurity firm acquired by Google LLC in September 2022, 

#### Filing 18 — Apple Inc. — accession 0001140361-26-035325

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K/A | ef20081427_8ka.htm iXBRL | 8-K/A | 39807
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: Apple Inc. (“Apple”) previously announced its Chief Executive Officer transition plan in its Current Report on Form 8-K filed on April 20, 2026 (the “Original Form 8-K”). This Amendment to the Original Form 8-K (the “Form 8-K/A”) is being filed to disclose John Ternus’ new compensation arrangement in connection with his appointment to the role of CEO, and Tim Cook’s new compensation arrangement in connection with his appointment to the role of Executive Chair of Apple’s Board of Directors (the “Board”), in each case effective as of September 1, 2026 (the “Transition Date”). Other than as set forth in this Form 8-K/A, all information in the Original Form 8-K remains unchanged. Mr. Ternus’ ann

#### Filing 19 — MICRON TECHNOLOGY INC — accession 0001104659-26-101067

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2624017d1_8k.htm iXBRL | 8-K | 33038
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On August 26, 2026, Micron Technology, Inc. ("Micron" or the “Company”) announced that Manish Bhatia, 54, the Company’s current Executive Vice President, Global Operations, has been appointed as President and Chief Operating Officer of the Company and that Dr. Scott DeBoer, 60, the Company’s current Executive Vice President, Chief Technology and Products Officer, has been appointed President and Chief Technology and Products Officer of the Company, effective immediately. Mr. Bhatia has led the Company’s global operations since joining Micron in 2017, overseeing manufacturing and factory c

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. Exhibit No. Description 99.1 Press Release dated August 26, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 20 — ADVANCED MICRO DEVICES INC — accession 0000002488-26-000163

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | amd-20260817.htm iXBRL | 8-K | 31546
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: Director Retirement On August 17, 2026, Mr. Joe Householder provided Advanced Micro Devices, Inc. (the “Company”) with notice of his intention to retire from the Company’s Board of Directors (the “Board”) effective as of August 19, 2026. Mr. Householder has served as a director since 2014. Mr. Householder’s retirement is not the result of any disagreement

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit No. Description 99.1 Press Release dated August 19, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 21 — ADVANCED MICRO DEVICES INC — accession 0001193125-26-354029

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 2.03: Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | d142696d8k.htm iXBRL | 8-K | 44357
Index items (from index page): 1.01, 2.03, 9.01

Item 2.03 heading: Item 2.03 Creation of
Item 2.03 excerpt: The information set forth under “Item 1.01. Entry into a Material Definitive Agreement” is incorporated herein by reference.

Item 1.01 heading: Item 1.01 Entry into a Material Definitive Agreement
Item 1.01 excerpt: On August 17, 2026 (the “Closing Date”), Advanced Micro Devices, Inc. (the “Company”) closed its public offering (the “Offering”) of $4.75 billion aggregate principal amount of senior notes, consisting of $1.25 billion aggregate principal amount of its 4.600% Senior Notes due 2029 (the “2029 Notes”), $1.50 billion aggregate principal amount of its 5.000% Senior Notes due 2031 (the “2031 Notes”), $1.00 billion aggregate principal amount of its 5.250% Senior Notes due 2033 (the “2033 Notes”) and $1.00 billion aggregate principal amount of its 5.500% Senior Notes due 2036 (the “2036 Notes,” and together with the 2029 Notes, the 2031 Notes and the 2033 Notes, the “Notes”). The terms of the Notes are governed by an Indenture, dated June 9, 2022 (the “Base Indenture”), by and between the Comp

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit Number Description 1.1 Underwriting Agreement, dated as of August 13, 2026, by and among Advanced Micro Devices, Inc. and Barclays Capital Inc., BofA Securities, Inc., Citigroup Global Markets Inc., J.P. Morgan Securities LLC, Morgan Stanley & Co. LLC and Wells Fargo Securities, LLC, as representatives of the several underwriters named therein 4.1 Third Supplemental Indenture, dated as of August 17, 2026, by and between the Company and U.S. Bank Trust Company, National Association, as trustee 4.2 Form of 2029 Note (included in Exhibit 4.1) 4.3 Form of 2031 Note (included in Exhibit 4.1) 4.4 Form of 2033 Note (included in Exhibit 4.1) 4.5 Form of 2036 Note (included in Exhibit 4.1) 5.1 Opinion of Latham & Watkins LLP 23.1 Consent of Latham & Watkins (included in Exhibit 5.1) 104 Cover Page Interactive Data File (the Cover Page XBRL ta

#### Filing 22 — NVIDIA CORP — accession 0001045810-26-000069

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 2.03: Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant Item 7.01: Regulation FD Disclosure
Documents table row (document whose Type is the form): 1 | 8-K | nvda-20260817.htm iXBRL | 8-K | 31418
Index items (from index page): 1.01, 2.03, 7.01

Item 1.01 heading: Item 1.01. Entry into a Material Definitive Agreement
Item 1.01 excerpt: On August 17, 2026, NVIDIA Corporation (“NVIDIA”) announced a multi-year partnership with SB Energy Corp. (collectively with its affiliates, “SB Energy”) to advance the development of the PORTS Technology Campus, a large-scale AI data center campus in Pike County, Ohio (the “Portsmouth Site”). Through the partnership and the credit support described below, NVIDIA has secured land, power, and shell capacity at the Portsmouth Site to host NVIDIA AI compute infrastructure. An affiliate of OpenAI Group PBC (such affiliate, “OpenAI”) will be the tenant. Residual Value Guaranties On August 17, 2026, NVIDIA entered into multiple residual value guaranties (collectively, the

Item 2.03 heading: Item 2.03. Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant
Item 2.03 excerpt: The information set forth in Item 1.01 above is hereby incorporated by reference into this Item 2.03.

Item 7.01 heading: Item 7.01
Item 7.01 excerpt: On August 17, 2026, NVIDIA issued a press release announcing the partnership with SB Energy. The press release is attached as Exhibit 99.1 hereto and is incorporated herein by reference. The press release is furn

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit Description 99.1 Press release, issued August 17, 2026 104 The cover page of this Current Report on Form 8-K, formatted in inline XBRL (included as Exhibit 101)

#### Filing 23 — JOHNSON & JOHNSON — accession 0000200406-26-000167

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | jnj-20260804.htm iXBRL | 8-K | 43919
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On August 4, 2026, the Company announced that Jennifer Taubert will retire from her position as Executive Vice President, Worldwide Chairman, Innovative Medicine and member of the Executive Committee effective September 1, 2026. The Company’s related press release is attached to this Report as Exhibit 99.1.

Item 9.01 heading: Item 9.01 Financial statements and exhibits
Item 9.01 excerpt: (d) Exhibits. Exhibit No. Description of Exhibit 99.1 Press Release dated August 4, 2026. 104 The cover page from this Current Report on Form 8-K, formatted in Inline XBRL. Signatures Pursuant to the requireme

#### Filing 24 — PROCTER & GAMBLE Co — accession 0000080424-26-000094

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 7.01: Regulation FD Disclosure Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | pg-20260729.htm iXBRL | 8-K | 55792
Index items (from index page): 5.02, 7.01, 9.01

Item 5.02 heading: ITEM 5.02 DEPARTURE OF DIRECTORS OR CERTAIN OFFICERS; ELECTION OF DIRECTORS; APPOINTMENT OF CERTAIN OFFICERS; COMPENSATORY ARRANGEMENTS OF CERTAIN OFFICERS
Item 5.02 excerpt: On July 29, 2026, The Procter & Gamble Company (the "Company") announced that Jon R. Moeller, Executive Chairman of the Board, will retire from his position as Executive Chairman and as a member of the Board of Directors (“the Board”), effective July 31, 2026. Mr. Moeller will remain with the Company through August 14, 2026, when he will retire from the Company. The Company als

Item 7.01 heading: ITEM 7.01 REGULATION FD DISCLOSURE
Item 7.01 excerpt: The Company issued a news release on July 29, 2026, announcing Mr. Moeller’s retirement and Mr. Jejurikar’s appointment. A copy of this news release is furnished as Exhibit 99.1 The Company is furnishing the information under this item, inc

Item 9.01 heading: ITEM 9.01 - FINANCIAL STATEMENTS AND EXHIBITS
Item 9.01 excerpt: Exhibit No. Description 99.1 Dividend News Release by The Procter & Gamble Company dated July 29, 2026. 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 25 — JPMORGAN CHASE & CO — accession 0000019617-26-000288

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Documents table row (document whose Type is the form): 1 | 8-K | jpm-20260721.htm iXBRL | 8-K | 42482
Index items (from index page): 5.03

Item 5.03 heading: Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Item 5.03 excerpt: The Board of Directors (the “Board”) of JPMorgan Chase & Co. (the “Corporation”) has adopted an amendment to Section 2.03 of the Corporation’s By-laws, effective July 21, 2026 (as so amended, the "By-laws"), to provide that a Lead Independent Director, if any, shall be appointed by the non-management directors. The foregoing description of the amendments to the By-laws does not purport to be a complete summary and is qualified i

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibit Exhibit No. Description of Exhibit 3.2 By-laws of JPMorgan Chase & Co., as amended, effective July 21, 2026 101 Pursuant to Rule 406 of Regulation S-T, the cover page is formatted in Inline XBRL (Inline eXtensible Business Reporting Language). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document and included in Exhibit 101).

#### Filing 26 — VISA INC. — accession 0001403161-26-000096

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | v-20260714.htm iXBRL | 8-K | 42402
Index items (from index page): 5.03, 9.01

Item 5.03 heading: Item 5.03 Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Item 5.03 excerpt: The Board of Directors of Visa Inc. (the “Company”) amended the Company’s Amended and Restated Bylaws (as amended, the “Bylaws”), effective July 14, 2026. The amendments designate (i) the Court of Chancery of the State of Delaware or, if such court lacks subject matter juri

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits Exhibit Number Description 3.2 Amended and Restated Bylaws of Visa Inc. 104 Cover Page Interactive Data File (formatted as Inline XBRL)

#### Filing 27 — NVIDIA CORP — accession 0001045810-26-000060

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | nvda-20260628.htm iXBRL | 8-K | 22172
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: (b) On June 28, 2026, Ajay K. Puri, Executive Vice President, Worldwide Field Operations of NVIDIA Corporation, or the Company, notified the Company of his intention to retire from his role effective upon the employment commencement date of his successor. Mr. Puri, a 21-year executive at NVIDIA, is expected to remain with the Company in a senior advisory role to ensure a s

#### Filing 28 — ADVANCED MICRO DEVICES INC — accession 0000002488-26-000115

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | amd-20260626.htm iXBRL | 8-K | 44715
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On June 26, 2026, the Board of Directors (the “Board”) of Advanced Micro Devices, Inc. (the “Company”) and the Compensation and Leadership Resources Committee of the Board (the “Committee”), as applicable, approved the following changes to the compensation of certain members of the Company’s executive team: Base Salary Increases Effective July 1, 2026, the annual base salaries for the below-listed members of the Company’s executive team will increase as follows: Name and Title Annual Base Salary as of June 30, 2026 Annual Base Salary Effective July 1, 2026 Lisa T. Su, Chair, President and Chief Executive Officer $1,323,000 $1,375,000 Jean Hu, Executive Vice President, Chief Financial Officer and Treasurer $800,000 $850,000 Mark Papermaster, Executive Vice President and Chief Technology Officer $870,000 $900,000 Darren Grasby, Executive Vice President, Chief Sales Officer and President EM

#### Filing 29 — NVIDIA CORP — accession 0001045810-26-000056

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.07: Submission of Matters to a Vote of Security Holders
Documents table row (document whose Type is the form): 1 | 8-K | nvda-20260624.htm iXBRL | 8-K | 61847
Index items (from index page): 5.07

Item 5.07 heading: Item 5.07. Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: On June 24, 2026, at the 2026 Annual Meeting of Stockholders of NVIDIA Corporation, or the 2026 Annual Meeting, the following proposals were adopted or rejected by the margin indicated. 1. Stockholders approved the election of each of our ten (10) director nominees to hold office until the 2027 Annual Me

#### Filing 30 — COCA COLA CO — accession 0001552781-26-000366

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 |  | e26287_ko-8k.htm iXBRL | 8-K | 74143
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On June 25, 2026, The Coca-Cola Company (the “Company”) announced that Jennifer Mann, Executive Vice President and President, North America Operating Unit, will be departing the Company. Effective July 31, 2026, Ms. Mann will step down from her current positions. Beginning on August 1, 2026, she will continue with the Company as a senior advisor until April 30, 2027. Effective Aug

Item 9.01 heading: Item 9.01(d). Financial Statements and Exhibits
Item 9.01 excerpt: EXHIBIT INDEX Exhibit No. Description Exhibit 10.1 Separation Agreement and Full and Complete Release and Agreement on Trade Secrets and Confidentiality between The Coca-Cola Company and Jennifer Mann, dated June 25, 2026. Exhibit 99.1 Press Release of The Coca-Cola Company, dated June 25, 2026. Exhibit 104 Cover Page Interactive Data File (the cover page XBRL tags are embedded within the iXBRL document).

#### Filing 31 — JPMORGAN CHASE & CO — accession 0000019617-26-000241

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | jpm-20260624.htm iXBRL | 8-K | 48933
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02 Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On June 25, 2026, JPMorgan Chase & Co. ("JPMorganChase" or the “Firm”) announced that Doug Petno, 61, and Troy Rohrbaugh, 56, Co-CEOs of the Commercial & Investment Bank ("CIB"), have been elected Co-Presidents of the Firm, effective immediately.1 In addition to their new roles, Mr. Petno will become sole CEO of the CIB, and Mr. Rohrbaugh will become CEO of Consumer & Community Banking ("CCB"). The promotions of Messrs. Petno and Rohrbaugh to Co-Presidents and sole CEOs of the Firm’s two largest businesses are p

Item 9.01 heading: Item 9.01 Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibit Exhibit No. Description of Exhibit 99.1 JPMorgan Chase & Co. Press Release dated June 25, 2026 101 Pursuant to Rule 406 of Regulation S-T, the cover page is formatted in Inline XBRL (Inline eXtensible Business Reporting Language). 104 Cover Page Interactive Data File (embedded within the Inline XBRL document and included in Exhibit 101).

#### Filing 32 — Mastercard Inc — accession 0001141391-26-000041

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.07: Submission of Matters to a Vote of Security Holders
Documents table row (document whose Type is the form): 1 | 8-K | ma-20260616.htm iXBRL | 8-K | 63046
Index items (from index page): 5.07

Item 5.07 heading: Item 5.07 Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: On June 16, 2026, Mastercard Incorporated ("Mastercard") held its annual meeting of stockholders (the "Annual Meeting"). Holders of Class A common stock at the close of business on April 21, 2026 were entitled to vote at the Annual Meeting.

#### Filing 33 — Alphabet Inc. — accession 0001193125-26-267578

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 5.07: Submission of Matters to a Vote of Security Holders Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | d57679d8k.htm iXBRL | 8-K | 119785
Index items (from index page): 5.02, 5.07, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: Amended and Restated Alphabet Inc. 2021 Stock Plan At the Annual Meeting of Shareholders of Alphabet Inc. (“Alphabet”) held on June 5, 2026 (the “2026 Annual Meeting”), Alphabet’s shareholders approved the amendment and restatement of the Alphabet Inc. Amended and Restated 2021 Stock Plan (the “2021 Stock Plan”) to increase the share reserve by 200,000,000 shares of Class C capital stock. A description of the 2021 Stock Plan and related matters was set forth in Alphabet’s definitive proxy statement on Form 14A filed with the U.S. Securities and Exchange Commission on April 24, 2026 (the “2026 Proxy Statement”) and is qualified in its entirety by reference to the full text of the 2021 Stock Plan, a copy of which is being filed as Exhibit 10.01 to this Form 8-K.

Item 5.07 heading: Item 5.07. Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: At the 2026 Annual Meeting, Alphabet’s shareholders voted on fourteen proposals as set forth below, all of which are described in detail in the 2026 Proxy Statement. Holders of the shares of Class A common stock were entitled to one vote per share held as of the close of business on A

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. Exhibit No. Description 10.01 Alphabet Inc. Amended and Restated 2021 Stock Plan 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 34 — AMAZON COM INC — accession 0001104659-26-072140

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 2.03: Creation of a Direct Financial Obligation or an Obligation under an Off-Balance Sheet Arrangement of a Registrant Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2613616d4_8k.htm iXBRL | 8-K | 54467
Index items (from index page): 1.01, 2.03, 9.01

Item 1.01 heading: ITEM 1.01 ENTRY INTO A MATERIAL DEFINITIVE AGREEMENT
Item 1.01 excerpt: On June 8, 2026, Amazon.com, Inc. (the “Company”), Citibank N.A., as administrative agent, and the lenders party thereto entered into a term loan agreement (the “DDTL Credit Agreement”). The DDTL Credit Agreement provides the Company with a $17.5 billion senior unsecured delayed draw term loan credit facility (the “DDTL Facility”). Commitments to provide the DDTL Facility will expire on September 30, 2026 unless fully borrowed prior to such date. Th

Item 2.03 heading: ITEM 2.03 CREATION OF A DIRECT FINANCIAL OBLIGATION OR AN OBLIGATION UNDER AN OFF-BALANCE SHEET ARRANGEMENT OF A REGISTRANT
Item 2.03 excerpt: The information set forth in Item 1.01 of this Current Report on Form 8-K is hereby incorporated by reference into this Item 2.03.

Item 9.01 heading: ITEM 9.01. FINANCIAL STATEMENTS AND EXHIBITS
Item 9.01 excerpt: (d) Exhibits. Exhibit Number Description 10.1 Term Loan Agreement, dated as of June 8 2026, among Amazon.com, Inc., Citibank N.A., as administrative agent, and the lenders party thereto. 104 The cover page from this Current Report on Form 8-K, formatted in Inline XBRL (included as Exhibit 101). 3

#### Filing 35 — MICRON TECHNOLOGY INC — accession 0001104659-26-071845

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | FORM 8-K | tm2617112d1_8k.htm iXBRL | 8-K | 31825
Index items (from index page): 5.02, 9.01

Item 5.02 heading: Item 5.02. Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers; Compensatory Arrangements of Certain Officers
Item 5.02 excerpt: On June 9, 2026, the Board of Directors (“Board”) of Micron Technology, Inc. (the “Company”) appointed Alexis Black Björlin as a member of the Board. The Board has determined that Dr. Björlin is an independent director under the applicable rules of the Nasdaq Stock Market LLC (the “Independence Rules”). Following the appointment of Dr. Björlin, the Board will have a total of nine directors, of which eight are determined to be independent under the Independence Rules. Dr. Björlin has also been appointed to the Governance and Sustainability Committee of the Board. Dr. Björlin will parti

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits. Exhibit No. Description 99.1 Press Release dated June 9, 2026 104 Cover Page Interactive Data File (embedded within the Inline XBRL document)

#### Filing 36 — Palantir Technologies Inc. — accession 0001321655-26-000033

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.07: Submission of Matters to a Vote of Security Holders
Documents table row (document whose Type is the form): 1 | 8-K | pltr-20260603.htm iXBRL | 8-K | 50995
Index items (from index page): 5.07

Item 5.07 heading: Item 5.07 - Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: On June 3, 2026, Palantir Technologies Inc. (the “Company”) held its 2026 annual meeting of stockholders (the “Annual Meeting”). Holders of the Company’s Class A common stock, par value $0.001 per share, were entitled to one vote on each proposal f

#### Filing 37 — Alphabet Inc. — accession 0001193125-26-259830

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 1.01: Entry into a Material Definitive Agreement Item 3.03: Material Modifications to Rights of Security Holders Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | d36818d8k.htm iXBRL | 8-K | 88964
Index items (from index page): 1.01, 3.03, 5.03, 9.01

Item 1.01 heading: Item 1.01. Entry into a Material Definitive Agreement
Item 1.01 excerpt: Mandatory Convertible Preferred Stock Offering On June 2, 2026, Alphabet Inc. (“Alphabet” or the “Company”) entered into an underwriting agreement (the “Underwriting Agreement”) with Goldman Sachs & Co. LLC, J.P. Morgan Securities LLC, and Morgan Stanley & Co. LLC as the representatives of the respective underwriters under such agreement, pursuant to which Alphabet agreed to issue and sell (1) 167,500,000 series A depositary shares (the “Series A Depositary Shares”), each representing a 1/20th interest in a share of 6.25% Series A Mandatory Convertible Preferred Stock, liquidation preference $1,000.00 per share, par value $0.001 per share (the “Series A Preferred Stock” and such offering, the “Series A Depositary Shares Offering”) and (2) 167,500,000 series B depositary shares (the “Series B Depositary Shares” and together with the Series A Depositary Shares, the “Depositary Shares”), ea

Item 3.03 heading: Item 3.03. Material Modification to Rights of Security Holders
Item 3.03 excerpt: On June 4, 2026, the Company filed the Certificates of Designations with the Secretary of State of the State of Delaware to establish the preferences, limitations and relative rights of the respective series of Preferred Stock. The Certificates of Designations became effective upon filing. Subject to certain exceptions, under the terms of each s

Item 5.03 heading: Item 5.03. Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Item 5.03 excerpt: The information set forth under Item 3.03 of this Current Report on Form 8-K is hereby incorporated by reference in this Item 5.03.

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d)Exhibits Exhibit No. Description 1.1 Form of Underwriting Agreement (Preferred Stock) (incorporated by reference to Exhibit 1.3 to Alphabet Inc’s Registration statement on Form S-3; File No: 333-296395) 3.1 Certificate of Designations for the 6.25% Series A Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective June 4, 2026 3.2 Certificate of Designations for the 6.25% Series B Mandatory Convertible Preferred Stock, filed with the Secretary of State of the State of Delaware and effective June 4, 2026 4.1 Form of Certificate for the 6.25% Series A Mandatory Convertible Preferred Stock (included as Exhibit A to Exhibit 3.1) 4.2 Form of Certificate for the 6.25% Series B Mandatory Convertible Preferred Stock (included as Exhibit A to Exhibit 3.2) 4.3 Deposit Agreement for the Series A Mandatory Convertible Preferred Stock, dated as

#### Filing 38 — Alphabet Inc. — accession 0001652044-26-000059

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.02: Departure of Directors or Certain Officers; Election of Directors; Appointment of Certain Officers: Compensatory Arrangements of Certain Officers
Documents table row (document whose Type is the form): 1 | 8-K | goog-20260602.htm iXBRL | 8-K | 60985
Index items (from index page): 5.02

Item 5.02 heading: Item 5.02
Item 5.02 excerpt: (c) Appointment of Principal Officer On June 5, 2026, Alphabet Inc. (“Alphabet”) announced the appointment of Marsida Saraci, Vice President and Controller, as its Principal Accounting Officer, effective immediately. Marsida Saraci, age 47, has worked for Alphabet since April 2011, most recently as Vice President, Finance - Deputy Con

#### Filing 39 — UNITEDHEALTH GROUP INC — accession 0000731766-26-000138

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.07: Submission of Matters to a Vote of Security Holders
Documents table row (document whose Type is the form): 1 | 8-K | unh-20260601.htm iXBRL | 8-K | 54329
Index items (from index page): 5.07

Item 5.07 heading: Item 5.07. Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: On June 1, 2026, the Company held its 2026 Annual Meeting of Shareholders (the “Annual Meeting”). There were 768,066,717 shares of common stock represented at the Annual Meeting. The shareholders of the Company voted 

#### Filing 40 — Walmart Inc. — accession 0000104169-26-000111

index_status: 200
doc_status: 200
Index Items excerpt: Items Item 5.03: Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year Item 5.07: Submission of Matters to a Vote of Security Holders Item 9.01: Financial Statements and Exhibits
Documents table row (document whose Type is the form): 1 | 8-K | wmt-20260604.htm iXBRL | 8-K | 74901
Index items (from index page): 5.03, 5.07, 9.01

Item 5.03 heading: Item 5.03. Amendments to Articles of Incorporation or Bylaws; Change in Fiscal Year
Item 5.03 excerpt: On June 4, 2026, Walmart Inc. (the "Company") held its Annual Shareholders' Meeting (the "Meeting"). At the Meeting, the Company's shareholders approved an amendment (the "Charter Amendment") to the Company's Restated Ce

Item 5.07 heading: Item 5.07. Submission of Matters to a Vote of Security Holders
Item 5.07 excerpt: As of close of business on April 10, 2026, the record date for the Meeting, there were 7,970,990,515 shares of the Company's common stock outstanding, with each share entitled to one vote. The holders of 7,164,547,083 shares of the Company's common stock were present in person or represented by proxy during

Item 9.01 heading: Item 9.01. Financial Statements and Exhibits
Item 9.01 excerpt: (d) Exhibits 3.1 Certificate of Amendment of Restated Certificate of Incorporation of Walmart Inc., effective June 4, 2026 3.2 Restated Certificate of Incorporation of Walmart Inc., effective June 4, 2026 Exhibit 104 Cover Page Interactive Data File (embedded within the Inline XBRL)

```synmerco-data
a488df1534dc386644dfa9c6f30dfda2473f7015b1de93cf13a6a3efbf063aba 8k-30-filers-pull1.csv
52791f46eaab79f3613a6e6b8d571477175a6d9f4e840bc35b4f1a9ec1592c2b 8k-30-filers-pull2.csv
8c9ce3ac56b81b1de5db61a80b763583b9dc94b8f02ab1eb977f771df3a1d3ca 8k-30-filers-pull3.csv
```
