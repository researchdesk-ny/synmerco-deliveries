# Infusion pump adverse event reports in the FDA database, last 12 months

Product code FRN (infusion pump), openFDA device adverse events, date received in the 12 months before each pull. Three timed pulls, 24 hours apart. Escrow esc_14e4279bd01941d0a7dd6b8a, bid 5337, $7.00.

## ACCEPTANCE CHECKS

Job acceptance items, quoted verbatim, with proof under each.

1. "The three CSV files are attached with exactly the listed columns, one row per key as the TASK defines (header-only only for a failed pull)."

Proof: D2, D3, D4 attached via the data route; each row count: 133, columns key, dimension, term, count, sorted by key — see DATA FILES. Revision 1 rebuild: one row per count term exactly as returned (raw names, unmerged; months summed); merged groups are report-only.

2. "Every count in the tables matches a count response in the PROOF."

Proof: Pull 3 event-type counts Malfunction 49222, Injury 651, Other 272, Death 86 (total 50231) are the event-type response in PROOF — PULL 3; the 15 largest manufacturer groups, monthly totals and death counts likewise match their PROOF responses.

3. "Groupings, monthly sums and changes follow the TASK and agree with the CSV."

Proof: Pull 3 event-type total 50231 = monthly total 50231; death-by-manufacturer total 86 = Death 86; Changes PULL 3 vs PULL 2: new 0, gone 0, changed 4, 133 = 133 + 0 − 0; each changed entry in both Changes sections states its key, the column (count), the earlier value and the later value, and the Changes keys are the CSV keys (raw terms as returned).

4. "The PLATFORM RECORD shows a PULL 1: note and each later PULL note at least its wait after the one before, each with its CSV's row count and SHA-256 as under DATA FILES; each pull's source time (the HTTP Date header of its first request) is later than the previous pull's; the change counts agree with the CSV files (or a pull failed as the TASK allows)."

Proof: PULL 1 note 2026-11-15 02:42:25 UTC; PULL 2 note 2026-11-16 02:48:13 UTC (24h05m later); corrected PULL 3 note 2026-11-17 02:53:39 UTC (24h05m after PULL 2); first-request HTTP Dates Sun, 15 Nov 2026 02:39:51 GMT, Mon, 16 Nov 2026 02:47:17 GMT, Tue, 17 Nov 2026 02:51:27 GMT, each later than the last — see PLATFORM RECORD. Revision 1 update notes (2026-11-17 03:48:59 / 03:49:00 / 03:49:02 UTC) carry the rebuilt CSVs' row count: 133 and SHA-256 under DATA FILES.
## PULL 1 — 2026-11-15

Pull 1 ran 2026-11-15 02:39–02:40 UTC; range date received 20251115 to 20261115. First request HTTP Date header: `Sun, 15 Nov 2026 02:39:51 GMT`.

### Event type table (Pull 1)

| event type | count |
|---|---:|
| Malfunction | 49239 |
| Injury | 651 |
| Other | 272 |
| Death | 86 |
| **total** | **50248** |

row count: 50248 reports in total.

### 15 largest manufacturer groups (Pull 1)

Manufacturer groups merge names equal after upper-casing, removing punctuation and the endings INC, LLC, CORPORATION, CO, LTD. Every merge is listed under Manufacturer merges below. Counts are the top 100 manufacturer names as returned (limit 100); their total is 50,134 of the 50,248 reports, so 114 reports belong to manufacturers beyond the top 100 and are not broken out here.

| manufacturer group | total | deaths |
|---|---:|---:|
| CAREFUSION 303 | 15793 | 18 |
| CAREFUSION SD | 13917 | 13 |
| ICU MEDICAL | 5555 | 2 |
| FRESENIUS KABI USA | 4157 | 1 |
| BAXTER HEALTHCARE | 3292 | 3 |
| MEDTRONIC PUERTO RICO OPERATIONS | 2724 | 0 |
| ICU MEDICAL COSTA RICA | 1448 | 1 |
| FRESENIUS VIAL S A S | 924 | 24 |
| ZYNO MEDICAL | 632 | 1 |
| B BRAUN MELSUNGEN AG | 402 | 13 |
| (blank — no manufacturer name returned) | 145 | 1 |
| MEDTRONIC MINIMED | 123 | 0 |
| EITAN MEDICAL | 110 | 0 |
| RMS MEDICAL KORU MEDICAL SYSTEMS | 101 | 0 |
| MOOG COSTA RICA SRL | 93 | 0 |

### Monthly totals (Pull 1)

| month | count |
|---|---:|
| 2025-11 | 1884 |
| 2025-12 | 3864 |
| 2026-01 | 3623 |
| 2026-02 | 4026 |
| 2026-03 | 4730 |
| 2026-04 | 5169 |
| 2026-05 | 4814 |
| 2026-06 | 4353 |
| 2026-07 | 4307 |
| 2026-08 | 4101 |
| 2026-09 | 4805 |
| 2026-10 | 4572 |
| **total** | **50248** |

November 2026 has no row: the query for date received 20261101 to 20261115 returned no matches (openFDA HTTP 404 NOT_FOUND, see PROOF), so no November 2026 reports were counted in this pull. The monthly total, 50,248, equals the event-type total, 50,248.

### Manufacturer merges (Pull 1)

- B BRAUN MELSUNGEN AG: merged from B BRAUN MELSUNGEN AG, B Braun Melsungen AG, B. BRAUN MELSUNGEN AG, B. Braun Melsungen AG, B.BRAUN MELSUNGEN AG, B.Braun Melsungen AG
- BELMONT MEDICAL TECHNOLOGIES: merged from BELMONT MEDICAL TECHNOLOGIES, Belmont Medical Technologies
- EITAN MEDICAL: merged from EITAN MEDICAL LTD, EITAN MEDICAL LTD., Eitan Medical Ltd.
- FRESENIUS KABI AG: merged from FRESENIUS KABI AG, Fresenius Kabi AG
- FRESENIUS KABI USA: merged from FRESENIUS KABI USA LLC, FRESENIUS KABI USA, LLC, Fresenius Kabi USA LLC, Fresenius Kabi USA, LLC
- FRESENIUS VIAL S A S: merged from FRESENIUS VIAL S.A.S, FRESENIUS VIAL S.A.S.
- ICU MEDICAL: merged from ICU MEDICAL, ICU MEDICAL ,INC, ICU MEDICAL INC, ICU MEDICAL, INC, ICU MEDICAL, INC., ICU Medical Inc, ICU Medical, Inc, ICU Medical, Inc., ICU Medical, Inc.¿
- ICU MEDICAL COSTA RICA: merged from ICU MEDICAL COSTA RICA LTD, ICU MEDICAL COSTA RICA LTD., ICU Medical Costa Rica Ltd, ICU Medical Costa Rica Ltd.
- ICU MEDICAL HEALTHCARE MANUFACTURING S A DE C V: merged from ICU MEDICAL HEALTHCARE MANUFACTURING S.A. DE C.V., ICU Medical Healthcare Manufacturing S.A. de C.V.
- KORU MEDICAL SYSTEMS: merged from KORU MEDICAL SYSTEMS, KORU MEDICAL SYSTEMS, INC., KORU Medical Systems
- MEDTRONIC PUERTO RICO OPERATIONS: merged from MEDTRONIC PUERTO RICO OPERATIONS CO., Medtronic Puerto Rico Operations Co.
- MILLYARD ADVANCED MEDICAL PRODUCTS: merged from MILLYARD ADVANCED MEDICAL PRODUCTS, LLC, Millyard Advanced Medical Products, LLC
- MOOG MEDICAL DEVICES: merged from MOOG MEDICAL DEVICES, Moog Medical Devices
- MOOG MEDICAL DEVICES GROUP: merged from MOOG MEDICAL DEVICES GROUP, Moog Medical Devices Group
- MOOG ZEVEX: merged from MOOG / ZEVEX, INC., MOOG/ ZEVEX, INC., MOOG/ZEVEX, INC.
- PHILLIPS MEDISIZE A S: merged from PHILLIPS-MEDISIZE A/S, Phillips-Medisize A/S
- RMS MEDICAL KORU MEDICAL SYSTEMS: merged from RMS MEDICAL / KORU MEDICAL SYSTEMS, INC, RMS MEDICAL / KORU MEDICAL SYSTEMS, INC., RMS MEDICAL /KORU MEDICAL SYSTEMS, INC., RMS MEDICAL/  KORU MEDICAL SYSTEMS, INC., RMS MEDICAL/ KORU MEDICAL SYSTEMS, INC., RMS MEDICAL/KORU MEDICAL SYSTEMS, INC., RMS Medical / KORU MEDICAL SYSTEMS, INC.
- SMITH S MEDICAL ICU MEDICAL: merged from SMITH'S MEDICAL/ICU MEDICAL, SMITH'S MEDICAL/ICU MEDICAL, INC
- SMITHS MEDICAL ASD INC ICU MEDICAL: merged from SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC, SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC.
- SMITHS MEDICAL ICU MEDICAL: merged from SMITHS MEDICAL / ICU MEDICAL, INC., SMITHS MEDICAL /ICU MEDICAL, INC., SMITHS MEDICAL/ICU MEDICAL, INC., Smiths Medical / ICU MEDICAL, INC.
- ZEVEX: merged from ZEVEX INC., ZEVEX, INC.
- ZEVEX INC MOOG: merged from ZEVEX, INC./ MOOG, INC., ZEVEX, INC./MOOG, INC.
- ZYNO MEDICAL: merged from ZYNO MEDICAL LLC., ZYNO MEDICAL, LLC, Zyno Medical, LLC

Death-by-manufacturer merges (same rule):
- B BRAUN MELSUNGEN AG: merged from B BRAUN MELSUNGEN AG, B. BRAUN MELSUNGEN AG
- FRESENIUS VIAL S A S: merged from FRESENIUS VIAL S.A.S, FRESENIUS VIAL S.A.S.
- MILLYARD ADVANCED MEDICAL PRODUCTS: merged from MILLYARD ADVANCED MEDICAL PRODUCTS, LLC, Millyard Advanced Medical Products, LLC

## PULL 2 — 2026-11-16

Pull 2 ran 2026-11-16 02:47 UTC; range date received 20251116 to 20261116. First request HTTP Date header: `Mon, 16 Nov 2026 02:47:17 GMT`.

### Event type table (Pull 2)

| event type | count |
|---|---:|
| Malfunction | 49228 |
| Injury | 651 |
| Other | 272 |
| Death | 86 |
| **total** | **50237** |

row count: 50237 reports in total.

### 15 largest manufacturer groups (Pull 2)

Manufacturer groups merge names equal after upper-casing, removing punctuation and the endings INC, LLC, CORPORATION, CO, LTD. Every merge is listed under Manufacturer merges below. Counts are the top 100 manufacturer names as returned (limit 100); their total is 50,123 of the 50,237 reports, so 114 reports belong to manufacturers beyond the top 100 and are not broken out here.

| manufacturer group | total | deaths |
|---|---:|---:|
| CAREFUSION 303 | 15793 | 18 |
| CAREFUSION SD | 13916 | 13 |
| ICU MEDICAL | 5555 | 2 |
| FRESENIUS KABI USA | 4157 | 1 |
| BAXTER HEALTHCARE | 3292 | 3 |
| MEDTRONIC PUERTO RICO OPERATIONS | 2714 | 0 |
| ICU MEDICAL COSTA RICA | 1448 | 1 |
| FRESENIUS VIAL S A S | 924 | 24 |
| ZYNO MEDICAL | 632 | 1 |
| B BRAUN MELSUNGEN AG | 402 | 13 |
| (blank — no manufacturer name returned) | 145 | 1 |
| MEDTRONIC MINIMED | 123 | 0 |
| EITAN MEDICAL | 110 | 0 |
| RMS MEDICAL KORU MEDICAL SYSTEMS | 101 | 0 |
| MOOG COSTA RICA SRL | 93 | 0 |

### Monthly totals (Pull 2)

| month | count |
|---|---:|
| 2025-11 | 1873 |
| 2025-12 | 3864 |
| 2026-01 | 3623 |
| 2026-02 | 4026 |
| 2026-03 | 4730 |
| 2026-04 | 5169 |
| 2026-05 | 4814 |
| 2026-06 | 4353 |
| 2026-07 | 4307 |
| 2026-08 | 4101 |
| 2026-09 | 4805 |
| 2026-10 | 4572 |
| **total** | **50237** |

November 2026 has no row: the query for date received 20261101 to 20261116 returned no matches (openFDA HTTP 404 NOT_FOUND, see PROOF), so no November 2026 reports were counted in this pull. The monthly total, 50,237, equals the event-type total, 50,237.

### Manufacturer merges (Pull 2)

Identical to Pull 1: the same 23 manufacturer merges and the same 3 death-by-manufacturer merges (verified in the Pull 2 pull log) — the full list is under Manufacturer merges (Pull 1).

## Changes — PULL 2 vs PULL 1

Pull 1 row count: 133; Pull 2 row count: 133. New keys: 0; gone keys: 0; changed keys: 4. Check: later = earlier + new - gone → 133 = 133 + 0 - 0. Each changed entry gives key, column, earlier value and later value.

- key: event type|Malfunction, column: count, earlier: 49239, later: 49228 (delta -11)
- key: manufacturer|CAREFUSION SD, column: count, earlier: 13917, later: 13916 (delta -1)
- key: manufacturer|MEDTRONIC PUERTO RICO OPERATIONS CO., column: count, earlier: 2084, later: 2074 (delta -10)
- key: month|2025-11, column: count, earlier: 1884, later: 1873 (delta -11)

All four changes are the same 11 reports leaving the window: it slid one day forward (20251115–20261115 → 20251116–20261116), the 11 reports dated 2025-11-15 dropped out (Pull 1 daily count for 20251115: 11), and no 2026-11-16 reports entered — November 2026 returns no matches. No other key moved; death counts unchanged (86 in both).


## PULL 3 — 2026-11-17

Pull 3 ran 2026-11-17 02:51 UTC; range date received 20251117 to 20261117. First request HTTP Date header: `Tue, 17 Nov 2026 02:51:27 GMT`. An earlier 02:48 UTC attempt ran with the wrong local date and covered the Pull 2 window; discarded and re-pulled — see PLATFORM RECORD.

### Event type table (Pull 3)

| event type | count |
|---|---:|
| Malfunction | 49222 |
| Injury | 651 |
| Other | 272 |
| Death | 86 |
| **total** | **50231** |

row count: 50231 reports in total.

### 15 largest manufacturer groups (Pull 3)

Same merge rule as Pull 1; merges listed below. Top 100 manufacturer names as returned (limit 100): total 50,117 of 50,231 reports, so 114 belong to manufacturers beyond the top 100.

| manufacturer group | total | deaths |
|---|---:|---:|
| CAREFUSION 303 | 15793 | 18 |
| CAREFUSION SD | 13914 | 13 |
| ICU MEDICAL | 5555 | 2 |
| FRESENIUS KABI USA | 4157 | 1 |
| BAXTER HEALTHCARE | 3292 | 3 |
| MEDTRONIC PUERTO RICO OPERATIONS | 2710 | 0 |
| ICU MEDICAL COSTA RICA | 1448 | 1 |
| FRESENIUS VIAL S A S | 924 | 24 |
| ZYNO MEDICAL | 632 | 1 |
| B BRAUN MELSUNGEN AG | 402 | 13 |
| (blank — no manufacturer name returned) | 145 | 1 |
| MEDTRONIC MINIMED | 123 | 0 |
| EITAN MEDICAL | 110 | 0 |
| RMS MEDICAL KORU MEDICAL SYSTEMS | 101 | 0 |
| MOOG COSTA RICA SRL | 93 | 0 |

### Monthly totals (Pull 3)

| month | count |
|---|---:|
| 2025-11 | 1867 |
| 2025-12 | 3864 |
| 2026-01 | 3623 |
| 2026-02 | 4026 |
| 2026-03 | 4730 |
| 2026-04 | 5169 |
| 2026-05 | 4814 |
| 2026-06 | 4353 |
| 2026-07 | 4307 |
| 2026-08 | 4101 |
| 2026-09 | 4805 |
| 2026-10 | 4572 |
| **total** | **50231** |

November 2026 has no row: the query for date received 20261101 to 20261117 returned no matches (openFDA HTTP 404 NOT_FOUND, see PROOF), so no November 2026 reports were counted in this pull. The monthly total, 50,231, equals the event-type total, 50,231.

### Manufacturer merges (Pull 3)

Identical to Pull 1: the same 23 manufacturer merges and the same 3 death-by-manufacturer merges (verified in the Pull 3 pull log) — the full list is under Manufacturer merges (Pull 1).

## Changes — PULL 3 vs PULL 2

Pull 2 row count: 133; Pull 3 row count: 133. New keys: 0; gone keys: 0; changed keys: 4. Check: later = earlier + new - gone → 133 = 133 + 0 - 0. Each changed entry gives key, column, earlier value and later value.

- key: event type|Malfunction, column: count, earlier: 49228, later: 49222 (delta -6)
- key: manufacturer|CAREFUSION SD, column: count, earlier: 13916, later: 13914 (delta -2)
- key: manufacturer|MEDTRONIC PUERTO RICO OPERATIONS CO., column: count, earlier: 2074, later: 2070 (delta -4)
- key: month|2025-11, column: count, earlier: 1873, later: 1867 (delta -6)

All four changes are the same 6 reports leaving the window: it slid one day forward (20251116–20261116 → 20251117–20261117), the 6 reports dated 2025-11-16 dropped out (Pull 2 daily count for 20251116: 6), and no 2026-11-17 reports entered — November 2026 returns no matches. No other key moved; death counts unchanged (86 in both).


## PROOF — PULL 1

Every request with its search and count parameters, UTC time, HTTP Date header, and each count response's results as returned, one per line.

### Failed first request, date_received full range (Pull 1)

This was the first request sent in Pull 1, before the event-type request below.
Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251115+TO+20261115]&count=date_received&limit=1000`
Requested at (UTC): 2026-11-15T02:38:54+00:00 (the time the saved response, pull1-date-received.json, was written in the run record)
HTTP Date header: not logged for this response — the run record saved only the error body below.
HTTP status: 403
{"error": {"code": "API_KEY_MISSING", "message": "No api_key was supplied. Get one at https://api.fda.gov:443"}}
Retried once as one count query per calendar month with limit=100 (the date-YYYY-MM requests below), which returned complete daily counts. The first successful request of Pull 1 is the event-type request below (Requested at (UTC): 2026-11-15T02:39:49.805259+00:00, HTTP Date header Sun, 15 Nov 2026 02:39:51 GMT); that HTTP Date is the first-request HTTP Date quoted for Pull 1, since the failed request's HTTP Date was not logged.

### event-type

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251115+TO+20261115]&count=event_type.exact`
Requested at (UTC): 2026-11-15T02:39:49.805259+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:51 GMT
HTTP status: 200
Malfunction: 49239
Injury: 651
Other: 272
Death: 86

### manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251115+TO+20261115]&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-15T02:39:50.854942+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:52 GMT
HTTP status: 200
CAREFUSION 303, INC.: 15793
CAREFUSION SD: 13917
ICU MEDICAL, INC.: 3761
BAXTER HEALTHCARE CORPORATION: 3292
MEDTRONIC PUERTO RICO OPERATIONS CO.: 2084
FRESENIUS KABI USA, LLC: 2031
FRESENIUS KABI USA LLC: 1505
ICU Medical, Inc.: 1364
ICU Medical Costa Rica Ltd.: 1232
Medtronic Puerto Rico Operations Co.: 640
Fresenius Kabi USA LLC: 602
ZYNO MEDICAL, LLC: 497
FRESENIUS VIAL S.A.S: 470
FRESENIUS VIAL S.A.S.: 454
ICU MEDICAL, INC: 224
ICU MEDICAL COSTA RICA LTD.: 202
ICU Medical, Inc: 190
B BRAUN MELSUNGEN AG: 160
: 145
Zyno Medical, LLC: 131
MEDTRONIC MINIMED: 123
MOOG COSTA RICA, SRL: 93
B Braun Melsungen AG: 91
B. BRAUN MELSUNGEN AG: 91
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC.: 52
Eitan Medical Ltd.: 49
SMITHS MEDICAL / ICU MEDICAL, INC.: 47
Millyard Advanced Medical Products, LLC: 46
MOOG / ZEVEX, INC.: 44
MOOG MEDICAL DEVICES: 43
FRESENIUS KABI DEUTSCHLAND GMBH: 42
MOOG MEDICAL DEVICES GROUP: 41
EITAN MEDICAL LTD.: 38
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 36
B.BRAUN MELSUNGEN AG: 27
RMS MEDICAL/KORU MEDICAL SYSTEMS, INC.: 24
EITAN MEDICAL LTD: 23
KORU MEDICAL SYSTEMS, INC.: 23
SMITHS MEDICAL/ICU MEDICAL, INC.: 22
B.Braun Melsungen AG: 19
Fresenius Kabi USA, LLC: 19
PHILLIPS-MEDISIZE A/S: 19
ICU MEDICAL, INC./SMITHS MEDICAL: 18
KORU MEDICAL SYSTEMS: 18
ZEVEX, INC.: 18
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 17
Moog Medical Devices Group: 17
B. BRAUN AVITUM AG: 16
SMITHS MEDICAL ASD, INC.: 15
B. Braun Melsungen AG: 14
BELMONT MEDICAL TECHNOLOGIES: 14
Moog Medical Devices: 14
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC.: 14
ICU Medical Nederland B.V.: 13
MOOG/ZEVEX, INC.: 12
ICU Medical Costa Rica Ltd: 11
ZEVEX, INC./MOOG, INC.: 11
IRADIMED CORPORATION: 10
UNK: 9
UNKNOWN: 9
ZEVEX, INC./ MOOG, INC.: 9
ICU MEDICAL HEALTHCARE MANUFACTURING S.A. DE C.V.: 8
Phillips-Medisize A/S: 8
SMITHS MEDICAL /ICU MEDICAL, INC.: 8
ICU Medical Healthcare Manufacturing S.A. de C.V.: 7
RMS MEDICAL/ KORU MEDICAL SYSTEMS, INC.: 7
ZEVEX INC.: 7
AVANOS MEDICAL INC.: 6
KORU Medical Systems: 6
RMS MEDICAL /KORU MEDICAL SYSTEMS, INC.: 6
B. BRAUN MEDICAL INC.: 5
KORU MEDICAL SYSTEMS, INC./RMS MEDICAL: 5
RMS Medical / KORU MEDICAL SYSTEMS, INC.: 5
SMITH MEDICAL/ICU MEDICAL, INC.: 5
SMITH'S MEDICAL/ICU MEDICAL: 5
Belmont Medical Technologies: 4
FRESENIUS KABI AG: 4
ICU Medical, Inc.¿: 4
MOOG, INC. / ZEVEX, INC.: 4
MOOG/ ZEVEX, INC.: 4
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC: 4
SMITH'S MEDICAL/ICU MEDICAL, INC: 4
SMITHS MEDICAL INTERNATIONAL LTD.: 4
Smiths Medical / ICU MEDICAL, INC.: 4
ZYNO MEDICAL LLC.: 4
BAXTER INTERNATIONAL INC.: 3
Belmont Medicat Technologies: 3
Fresenius Kabi AG: 3
ICU MEDICAL: 3
ICU MEDICAL ,INC: 3
ICU MEDICAL COSTA RICA LTD: 3
ICU MEDICAL INC: 3
ICU Medical Inc: 3
RMS MEDICAL/  KORU MEDICAL SYSTEMS, INC.: 3
RMS/KORU MEDICAL SYSTEMS INC.: 3
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC: 3
ATLANTA BIOMEDICAL CORPORATION: 2
BECTON DICKINSON: 2
BECTON DICKINSON/CAREFUSION 2200, INC.: 2
BECTON, DICKINSON AND COMPANY / CAREFUSION 303, INC.: 2

### date-2025-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251115+TO+20251130]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:51.438133+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:54 GMT
HTTP status: 200
20251115: 11
20251116: 6
20251117: 203
20251118: 168
20251119: 297
20251120: 229
20251121: 193
20251122: 13
20251123: 16
20251124: 169
20251125: 200
20251126: 186
20251127: 90
20251128: 91
20251129: 6
20251130: 6

### date-2025-12

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251201+TO+20251231]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:53.720683+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:55 GMT
HTTP status: 200
20251201: 232
20251202: 203
20251203: 116
20251204: 149
20251205: 137
20251208: 230
20251209: 217
20251210: 213
20251211: 167
20251212: 220
20251213: 6
20251214: 11
20251215: 122
20251216: 138
20251217: 133
20251218: 157
20251219: 114
20251221: 1
20251222: 116
20251223: 253
20251224: 94
20251225: 212
20251226: 127
20251227: 1
20251228: 1
20251229: 164
20251230: 169
20251231: 161

### date-2026-01

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260101+TO+20260131]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:54.961826+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:56 GMT
HTTP status: 200
20260101: 2
20260102: 214
20260104: 2
20260105: 179
20260106: 173
20260107: 174
20260108: 159
20260109: 202
20260112: 192
20260113: 211
20260114: 195
20260115: 64
20260116: 111
20260117: 3
20260118: 6
20260119: 101
20260120: 159
20260121: 137
20260122: 193
20260123: 219
20260124: 12
20260126: 59
20260127: 196
20260128: 210
20260129: 216
20260130: 234

### date-2026-02

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260201+TO+20260228]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:55.987851+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:57 GMT
HTTP status: 200
20260202: 147
20260203: 290
20260204: 213
20260205: 235
20260206: 179
20260207: 2
20260208: 28
20260209: 158
20260210: 172
20260211: 176
20260212: 194
20260213: 194
20260214: 2
20260215: 2
20260216: 157
20260217: 225
20260218: 279
20260219: 205
20260220: 213
20260221: 10
20260222: 3
20260223: 142
20260224: 187
20260225: 215
20260226: 153
20260227: 245

### date-2026-03

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260301+TO+20260331]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:56.847304+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:58 GMT
HTTP status: 200
20260302: 228
20260303: 288
20260304: 216
20260305: 277
20260306: 202
20260307: 10
20260308: 1
20260309: 182
20260310: 113
20260311: 271
20260312: 192
20260313: 307
20260314: 13
20260316: 203
20260317: 230
20260318: 191
20260319: 160
20260320: 194
20260321: 2
20260322: 3
20260323: 198
20260324: 223
20260325: 210
20260326: 213
20260327: 1
20260330: 383
20260331: 219

### date-2026-04

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260401+TO+20260430]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:57.602390+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:58 GMT
HTTP status: 200
20260401: 228
20260402: 175
20260403: 210
20260404: 3
20260405: 1
20260406: 155
20260407: 150
20260408: 269
20260409: 190
20260410: 139
20260411: 41
20260412: 3
20260413: 226
20260414: 165
20260415: 271
20260416: 217
20260417: 189
20260418: 4
20260419: 5
20260420: 121
20260421: 207
20260422: 329
20260423: 123
20260424: 284
20260425: 11
20260426: 29
20260427: 260
20260428: 266
20260429: 445
20260430: 453

### date-2026-05

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260501+TO+20260531]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:58.190920+00:00
HTTP Date header: Sun, 15 Nov 2026 02:39:59 GMT
HTTP status: 200
20260501: 99
20260503: 74
20260504: 415
20260505: 389
20260506: 323
20260507: 296
20260508: 238
20260509: 1
20260511: 194
20260512: 208
20260513: 177
20260514: 316
20260515: 187
20260517: 2
20260518: 157
20260519: 131
20260520: 171
20260521: 169
20260522: 146
20260524: 1
20260525: 96
20260526: 284
20260527: 286
20260528: 194
20260529: 206
20260531: 54

### date-2026-06

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260601+TO+20260630]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:58.774961+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:00 GMT
HTTP status: 200
20260601: 260
20260602: 194
20260603: 298
20260604: 244
20260605: 225
20260606: 2
20260607: 1
20260608: 148
20260609: 135
20260610: 181
20260611: 259
20260612: 174
20260615: 158
20260616: 209
20260617: 143
20260618: 114
20260619: 248
20260620: 7
20260622: 181
20260623: 178
20260624: 159
20260625: 170
20260626: 196
20260627: 1
20260628: 4
20260629: 188
20260630: 276

### date-2026-07

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260701+TO+20260731]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:39:59.993794+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:01 GMT
HTTP status: 200
20260701: 170
20260702: 218
20260703: 143
20260705: 7
20260706: 223
20260707: 303
20260708: 216
20260709: 158
20260710: 124
20260711: 2
20260713: 116
20260714: 235
20260715: 142
20260716: 214
20260717: 122
20260718: 2
20260720: 160
20260721: 184
20260722: 77
20260727: 693
20260728: 140
20260729: 220
20260730: 173
20260731: 265

### date-2026-08

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260801+TO+20260831]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:40:00.678829+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:02 GMT
HTTP status: 200
20260803: 153
20260804: 168
20260805: 179
20260806: 230
20260807: 193
20260808: 2
20260809: 1
20260810: 143
20260811: 244
20260812: 207
20260813: 272
20260814: 171
20260816: 4
20260817: 225
20260818: 172
20260819: 186
20260820: 206
20260821: 176
20260822: 5
20260824: 178
20260825: 169
20260826: 209
20260827: 215
20260828: 184
20260830: 57
20260831: 152

### date-2026-09

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260901+TO+20260930]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:40:01.790633+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:03 GMT
HTTP status: 200
20260901: 176
20260902: 290
20260903: 230
20260904: 193
20260905: 6
20260906: 5
20260907: 124
20260908: 226
20260909: 233
20260910: 215
20260911: 279
20260912: 5
20260913: 6
20260914: 141
20260915: 218
20260916: 249
20260917: 280
20260918: 297
20260919: 4
20260921: 171
20260922: 175
20260923: 207
20260924: 270
20260925: 197
20260926: 4
20260927: 5
20260928: 147
20260929: 250
20260930: 202

### date-2026-10

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261001+TO+20261031]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:40:02.485651+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:03 GMT
HTTP status: 200
20261001: 181
20261002: 36
20261004: 6
20261005: 156
20261006: 191
20261007: 193
20261008: 229
20261009: 206
20261010: 7
20261012: 192
20261013: 192
20261014: 253
20261015: 270
20261016: 299
20261017: 2
20261019: 190
20261020: 64
20261021: 204
20261022: 247
20261023: 217
20261025: 9
20261026: 220
20261027: 233
20261028: 286
20261029: 286
20261030: 203

### date-2026-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261101+TO+20261115]&count=date_received&limit=100`
Requested at (UTC): 2026-11-15T02:40:03.141944+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:05 GMT
HTTP status: 404
(no results returned)

### death-by-manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251115+TO+20261115]+AND+event_type:Death&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-15T02:40:04.479539+00:00
HTTP Date header: Sun, 15 Nov 2026 02:40:06 GMT
HTTP status: 200
FRESENIUS VIAL S.A.S: 20
CAREFUSION 303, INC.: 18
CAREFUSION SD: 13
B. BRAUN MELSUNGEN AG: 9
B BRAUN MELSUNGEN AG: 4
FRESENIUS VIAL S.A.S.: 4
BAXTER HEALTHCARE CORPORATION: 3
IRADIMED CORPORATION: 3
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 3
ICU Medical, Inc.: 2
: 1
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 1
FRESENIUS KABI USA, LLC: 1
ICU Medical Costa Rica Ltd.: 1
Millyard Advanced Medical Products, LLC: 1
UNK: 1
ZYNO MEDICAL, LLC: 1


## PROOF — PULL 2

Every request with its search and count parameters, UTC time, HTTP Date header, and each count response's results as returned, one per line.

date_received is counted one calendar month at a time (limit=100 per query); the full-range count with limit=1000 is rejected keyless by openFDA (HTTP 403 API_KEY_MISSING — see PROOF — PULL 1). Months are summed from the daily counts.

### event-type

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251116+TO+20261116]&count=event_type.exact`
Requested at (UTC): 2026-11-16T02:47:14.676532+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:17 GMT
HTTP status: 200
Malfunction: 49228
Injury: 651
Other: 272
Death: 86

### manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251116+TO+20261116]&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-16T02:47:16.682565+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:18 GMT
HTTP status: 200
CAREFUSION 303, INC.: 15793
CAREFUSION SD: 13916
ICU MEDICAL, INC.: 3761
BAXTER HEALTHCARE CORPORATION: 3292
MEDTRONIC PUERTO RICO OPERATIONS CO.: 2074
FRESENIUS KABI USA, LLC: 2031
FRESENIUS KABI USA LLC: 1505
ICU Medical, Inc.: 1364
ICU Medical Costa Rica Ltd.: 1232
Medtronic Puerto Rico Operations Co.: 640
Fresenius Kabi USA LLC: 602
ZYNO MEDICAL, LLC: 497
FRESENIUS VIAL S.A.S: 470
FRESENIUS VIAL S.A.S.: 454
ICU MEDICAL, INC: 224
ICU MEDICAL COSTA RICA LTD.: 202
ICU Medical, Inc: 190
B BRAUN MELSUNGEN AG: 160
: 145
Zyno Medical, LLC: 131
MEDTRONIC MINIMED: 123
MOOG COSTA RICA, SRL: 93
B Braun Melsungen AG: 91
B. BRAUN MELSUNGEN AG: 91
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC.: 52
Eitan Medical Ltd.: 49
SMITHS MEDICAL / ICU MEDICAL, INC.: 47
Millyard Advanced Medical Products, LLC: 46
MOOG / ZEVEX, INC.: 44
MOOG MEDICAL DEVICES: 43
FRESENIUS KABI DEUTSCHLAND GMBH: 42
MOOG MEDICAL DEVICES GROUP: 41
EITAN MEDICAL LTD.: 38
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 36
B.BRAUN MELSUNGEN AG: 27
RMS MEDICAL/KORU MEDICAL SYSTEMS, INC.: 24
EITAN MEDICAL LTD: 23
KORU MEDICAL SYSTEMS, INC.: 23
SMITHS MEDICAL/ICU MEDICAL, INC.: 22
B.Braun Melsungen AG: 19
Fresenius Kabi USA, LLC: 19
PHILLIPS-MEDISIZE A/S: 19
ICU MEDICAL, INC./SMITHS MEDICAL: 18
KORU MEDICAL SYSTEMS: 18
ZEVEX, INC.: 18
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 17
Moog Medical Devices Group: 17
B. BRAUN AVITUM AG: 16
SMITHS MEDICAL ASD, INC.: 15
B. Braun Melsungen AG: 14
BELMONT MEDICAL TECHNOLOGIES: 14
Moog Medical Devices: 14
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC.: 14
ICU Medical Nederland B.V.: 13
MOOG/ZEVEX, INC.: 12
ICU Medical Costa Rica Ltd: 11
ZEVEX, INC./MOOG, INC.: 11
IRADIMED CORPORATION: 10
UNK: 9
UNKNOWN: 9
ZEVEX, INC./ MOOG, INC.: 9
ICU MEDICAL HEALTHCARE MANUFACTURING S.A. DE C.V.: 8
Phillips-Medisize A/S: 8
SMITHS MEDICAL /ICU MEDICAL, INC.: 8
ICU Medical Healthcare Manufacturing S.A. de C.V.: 7
RMS MEDICAL/ KORU MEDICAL SYSTEMS, INC.: 7
ZEVEX INC.: 7
AVANOS MEDICAL INC.: 6
KORU Medical Systems: 6
RMS MEDICAL /KORU MEDICAL SYSTEMS, INC.: 6
B. BRAUN MEDICAL INC.: 5
KORU MEDICAL SYSTEMS, INC./RMS MEDICAL: 5
RMS Medical / KORU MEDICAL SYSTEMS, INC.: 5
SMITH MEDICAL/ICU MEDICAL, INC.: 5
SMITH'S MEDICAL/ICU MEDICAL: 5
Belmont Medical Technologies: 4
FRESENIUS KABI AG: 4
ICU Medical, Inc.¿: 4
MOOG, INC. / ZEVEX, INC.: 4
MOOG/ ZEVEX, INC.: 4
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC: 4
SMITH'S MEDICAL/ICU MEDICAL, INC: 4
SMITHS MEDICAL INTERNATIONAL LTD.: 4
Smiths Medical / ICU MEDICAL, INC.: 4
ZYNO MEDICAL LLC.: 4
BAXTER INTERNATIONAL INC.: 3
Belmont Medicat Technologies: 3
Fresenius Kabi AG: 3
ICU MEDICAL: 3
ICU MEDICAL ,INC: 3
ICU MEDICAL COSTA RICA LTD: 3
ICU MEDICAL INC: 3
ICU Medical Inc: 3
RMS MEDICAL/  KORU MEDICAL SYSTEMS, INC.: 3
RMS/KORU MEDICAL SYSTEMS INC.: 3
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC: 3
ATLANTA BIOMEDICAL CORPORATION: 2
BECTON DICKINSON: 2
BECTON DICKINSON/CAREFUSION 2200, INC.: 2
BECTON, DICKINSON AND COMPANY / CAREFUSION 303, INC.: 2

### date-2025-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251116+TO+20251130]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:17.297464+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:18 GMT
HTTP status: 200
20251116: 6
20251117: 203
20251118: 168
20251119: 297
20251120: 229
20251121: 193
20251122: 13
20251123: 16
20251124: 169
20251125: 200
20251126: 186
20251127: 90
20251128: 91
20251129: 6
20251130: 6

### date-2025-12

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251201+TO+20251231]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:18.008072+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:20 GMT
HTTP status: 200
20251201: 232
20251202: 203
20251203: 116
20251204: 149
20251205: 137
20251208: 230
20251209: 217
20251210: 213
20251211: 167
20251212: 220
20251213: 6
20251214: 11
20251215: 122
20251216: 138
20251217: 133
20251218: 157
20251219: 114
20251221: 1
20251222: 116
20251223: 253
20251224: 94
20251225: 212
20251226: 127
20251227: 1
20251228: 1
20251229: 164
20251230: 169
20251231: 161

### date-2026-01

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260101+TO+20260131]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:19.107201+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:20 GMT
HTTP status: 200
20260101: 2
20260102: 214
20260104: 2
20260105: 179
20260106: 173
20260107: 174
20260108: 159
20260109: 202
20260112: 192
20260113: 211
20260114: 195
20260115: 64
20260116: 111
20260117: 3
20260118: 6
20260119: 101
20260120: 159
20260121: 137
20260122: 193
20260123: 219
20260124: 12
20260126: 59
20260127: 196
20260128: 210
20260129: 216
20260130: 234

### date-2026-02

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260201+TO+20260228]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:19.851950+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:21 GMT
HTTP status: 200
20260202: 147
20260203: 290
20260204: 213
20260205: 235
20260206: 179
20260207: 2
20260208: 28
20260209: 158
20260210: 172
20260211: 176
20260212: 194
20260213: 194
20260214: 2
20260215: 2
20260216: 157
20260217: 225
20260218: 279
20260219: 205
20260220: 213
20260221: 10
20260222: 3
20260223: 142
20260224: 187
20260225: 215
20260226: 153
20260227: 245

### date-2026-03

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260301+TO+20260331]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:20.638076+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:22 GMT
HTTP status: 200
20260302: 228
20260303: 288
20260304: 216
20260305: 277
20260306: 202
20260307: 10
20260308: 1
20260309: 182
20260310: 113
20260311: 271
20260312: 192
20260313: 307
20260314: 13
20260316: 203
20260317: 230
20260318: 191
20260319: 160
20260320: 194
20260321: 2
20260322: 3
20260323: 198
20260324: 223
20260325: 210
20260326: 213
20260327: 1
20260330: 383
20260331: 219

### date-2026-04

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260401+TO+20260430]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:21.761243+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:23 GMT
HTTP status: 200
20260401: 228
20260402: 175
20260403: 210
20260404: 3
20260405: 1
20260406: 155
20260407: 150
20260408: 269
20260409: 190
20260410: 139
20260411: 41
20260412: 3
20260413: 226
20260414: 165
20260415: 271
20260416: 217
20260417: 189
20260418: 4
20260419: 5
20260420: 121
20260421: 207
20260422: 329
20260423: 123
20260424: 284
20260425: 11
20260426: 29
20260427: 260
20260428: 266
20260429: 445
20260430: 453

### date-2026-05

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260501+TO+20260531]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:22.530659+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:24 GMT
HTTP status: 200
20260501: 99
20260503: 74
20260504: 415
20260505: 389
20260506: 323
20260507: 296
20260508: 238
20260509: 1
20260511: 194
20260512: 208
20260513: 177
20260514: 316
20260515: 187
20260517: 2
20260518: 157
20260519: 131
20260520: 171
20260521: 169
20260522: 146
20260524: 1
20260525: 96
20260526: 284
20260527: 286
20260528: 194
20260529: 206
20260531: 54

### date-2026-06

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260601+TO+20260630]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:23.139236+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:24 GMT
HTTP status: 200
20260601: 260
20260602: 194
20260603: 298
20260604: 244
20260605: 225
20260606: 2
20260607: 1
20260608: 148
20260609: 135
20260610: 181
20260611: 259
20260612: 174
20260615: 158
20260616: 209
20260617: 143
20260618: 114
20260619: 248
20260620: 7
20260622: 181
20260623: 178
20260624: 159
20260625: 170
20260626: 196
20260627: 1
20260628: 4
20260629: 188
20260630: 276

### date-2026-07

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260701+TO+20260731]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:23.876560+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:25 GMT
HTTP status: 200
20260701: 170
20260702: 218
20260703: 143
20260705: 7
20260706: 223
20260707: 303
20260708: 216
20260709: 158
20260710: 124
20260711: 2
20260713: 116
20260714: 235
20260715: 142
20260716: 214
20260717: 122
20260718: 2
20260720: 160
20260721: 184
20260722: 77
20260727: 693
20260728: 140
20260729: 220
20260730: 173
20260731: 265

### date-2026-08

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260801+TO+20260831]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:24.521729+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:26 GMT
HTTP status: 200
20260803: 153
20260804: 168
20260805: 179
20260806: 230
20260807: 193
20260808: 2
20260809: 1
20260810: 143
20260811: 244
20260812: 207
20260813: 272
20260814: 171
20260816: 4
20260817: 225
20260818: 172
20260819: 186
20260820: 206
20260821: 176
20260822: 5
20260824: 178
20260825: 169
20260826: 209
20260827: 215
20260828: 184
20260830: 57
20260831: 152

### date-2026-09

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260901+TO+20260930]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:25.620970+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:27 GMT
HTTP status: 200
20260901: 176
20260902: 290
20260903: 230
20260904: 193
20260905: 6
20260906: 5
20260907: 124
20260908: 226
20260909: 233
20260910: 215
20260911: 279
20260912: 5
20260913: 6
20260914: 141
20260915: 218
20260916: 249
20260917: 280
20260918: 297
20260919: 4
20260921: 171
20260922: 175
20260923: 207
20260924: 270
20260925: 197
20260926: 4
20260927: 5
20260928: 147
20260929: 250
20260930: 202

### date-2026-10

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261001+TO+20261031]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:26.413889+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:28 GMT
HTTP status: 200
20261001: 181
20261002: 36
20261004: 6
20261005: 156
20261006: 191
20261007: 193
20261008: 229
20261009: 206
20261010: 7
20261012: 192
20261013: 192
20261014: 253
20261015: 270
20261016: 299
20261017: 2
20261019: 190
20261020: 64
20261021: 204
20261022: 247
20261023: 217
20261025: 9
20261026: 220
20261027: 233
20261028: 286
20261029: 286
20261030: 203

### date-2026-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261101+TO+20261116]&count=date_received&limit=100`
Requested at (UTC): 2026-11-16T02:47:27.167325+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:28 GMT
HTTP status: 404
(no results returned)

### death-by-manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251116+TO+20261116]+AND+event_type:Death&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-16T02:47:27.875052+00:00
HTTP Date header: Mon, 16 Nov 2026 02:47:29 GMT
HTTP status: 200
FRESENIUS VIAL S.A.S: 20
CAREFUSION 303, INC.: 18
CAREFUSION SD: 13
B. BRAUN MELSUNGEN AG: 9
B BRAUN MELSUNGEN AG: 4
FRESENIUS VIAL S.A.S.: 4
BAXTER HEALTHCARE CORPORATION: 3
IRADIMED CORPORATION: 3
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 3
ICU Medical, Inc.: 2
: 1
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 1
FRESENIUS KABI USA, LLC: 1
ICU Medical Costa Rica Ltd.: 1
Millyard Advanced Medical Products, LLC: 1
UNK: 1
ZYNO MEDICAL, LLC: 1
## PROOF — PULL 3

Every request with its search and count parameters, UTC time, HTTP Date header, and results as returned, one per line.

date_received is counted one calendar month at a time (limit=100 per query); the full-range count with limit=1000 is rejected keyless by openFDA (HTTP 403 API_KEY_MISSING — see PROOF — PULL 1). Months are summed from the daily counts.

### event-type

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251117+TO+20261117]&count=event_type.exact`
Requested at (UTC): 2026-11-17T02:51:25.532857+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:27 GMT
HTTP status: 200
Malfunction: 49222
Injury: 651
Other: 272
Death: 86

### manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251117+TO+20261117]&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-17T02:51:26.290483+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:27 GMT
HTTP status: 200
CAREFUSION 303, INC.: 15793
CAREFUSION SD: 13914
ICU MEDICAL, INC.: 3761
BAXTER HEALTHCARE CORPORATION: 3292
MEDTRONIC PUERTO RICO OPERATIONS CO.: 2070
FRESENIUS KABI USA, LLC: 2031
FRESENIUS KABI USA LLC: 1505
ICU Medical, Inc.: 1364
ICU Medical Costa Rica Ltd.: 1232
Medtronic Puerto Rico Operations Co.: 640
Fresenius Kabi USA LLC: 602
ZYNO MEDICAL, LLC: 497
FRESENIUS VIAL S.A.S: 470
FRESENIUS VIAL S.A.S.: 454
ICU MEDICAL, INC: 224
ICU MEDICAL COSTA RICA LTD.: 202
ICU Medical, Inc: 190
B BRAUN MELSUNGEN AG: 160
: 145
Zyno Medical, LLC: 131
MEDTRONIC MINIMED: 123
MOOG COSTA RICA, SRL: 93
B Braun Melsungen AG: 91
B. BRAUN MELSUNGEN AG: 91
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC.: 52
Eitan Medical Ltd.: 49
SMITHS MEDICAL / ICU MEDICAL, INC.: 47
Millyard Advanced Medical Products, LLC: 46
MOOG / ZEVEX, INC.: 44
MOOG MEDICAL DEVICES: 43
FRESENIUS KABI DEUTSCHLAND GMBH: 42
MOOG MEDICAL DEVICES GROUP: 41
EITAN MEDICAL LTD.: 38
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 36
B.BRAUN MELSUNGEN AG: 27
RMS MEDICAL/KORU MEDICAL SYSTEMS, INC.: 24
EITAN MEDICAL LTD: 23
KORU MEDICAL SYSTEMS, INC.: 23
SMITHS MEDICAL/ICU MEDICAL, INC.: 22
B.Braun Melsungen AG: 19
Fresenius Kabi USA, LLC: 19
PHILLIPS-MEDISIZE A/S: 19
ICU MEDICAL, INC./SMITHS MEDICAL: 18
KORU MEDICAL SYSTEMS: 18
ZEVEX, INC.: 18
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 17
Moog Medical Devices Group: 17
B. BRAUN AVITUM AG: 16
SMITHS MEDICAL ASD, INC.: 15
B. Braun Melsungen AG: 14
BELMONT MEDICAL TECHNOLOGIES: 14
Moog Medical Devices: 14
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC.: 14
ICU Medical Nederland B.V.: 13
MOOG/ZEVEX, INC.: 12
ICU Medical Costa Rica Ltd: 11
ZEVEX, INC./MOOG, INC.: 11
IRADIMED CORPORATION: 10
UNK: 9
UNKNOWN: 9
ZEVEX, INC./ MOOG, INC.: 9
ICU MEDICAL HEALTHCARE MANUFACTURING S.A. DE C.V.: 8
Phillips-Medisize A/S: 8
SMITHS MEDICAL /ICU MEDICAL, INC.: 8
ICU Medical Healthcare Manufacturing S.A. de C.V.: 7
RMS MEDICAL/ KORU MEDICAL SYSTEMS, INC.: 7
ZEVEX INC.: 7
AVANOS MEDICAL INC.: 6
KORU Medical Systems: 6
RMS MEDICAL /KORU MEDICAL SYSTEMS, INC.: 6
B. BRAUN MEDICAL INC.: 5
KORU MEDICAL SYSTEMS, INC./RMS MEDICAL: 5
RMS Medical / KORU MEDICAL SYSTEMS, INC.: 5
SMITH MEDICAL/ICU MEDICAL, INC.: 5
SMITH'S MEDICAL/ICU MEDICAL: 5
Belmont Medical Technologies: 4
FRESENIUS KABI AG: 4
ICU Medical, Inc.¿: 4
MOOG, INC. / ZEVEX, INC.: 4
MOOG/ ZEVEX, INC.: 4
RMS MEDICAL / KORU MEDICAL SYSTEMS, INC: 4
SMITH'S MEDICAL/ICU MEDICAL, INC: 4
SMITHS MEDICAL INTERNATIONAL LTD.: 4
Smiths Medical / ICU MEDICAL, INC.: 4
ZYNO MEDICAL LLC.: 4
BAXTER INTERNATIONAL INC.: 3
Belmont Medicat Technologies: 3
Fresenius Kabi AG: 3
ICU MEDICAL: 3
ICU MEDICAL ,INC: 3
ICU MEDICAL COSTA RICA LTD: 3
ICU MEDICAL INC: 3
ICU Medical Inc: 3
RMS MEDICAL/  KORU MEDICAL SYSTEMS, INC.: 3
RMS/KORU MEDICAL SYSTEMS INC.: 3
SMITHS MEDICAL ASD, INC./ ICU MEDICAL, INC: 3
ATLANTA BIOMEDICAL CORPORATION: 2
BECTON DICKINSON: 2
BECTON DICKINSON/CAREFUSION 2200, INC.: 2
BECTON, DICKINSON AND COMPANY / CAREFUSION 303, INC.: 2

### date-2025-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251117+TO+20251130]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:27.096571+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:28 GMT
HTTP status: 200
20251117: 203
20251118: 168
20251119: 297
20251120: 229
20251121: 193
20251122: 13
20251123: 16
20251124: 169
20251125: 200
20251126: 186
20251127: 90
20251128: 91
20251129: 6
20251130: 6

### date-2025-12

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251201+TO+20251231]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:27.841873+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:29 GMT
HTTP status: 200
20251201: 232
20251202: 203
20251203: 116
20251204: 149
20251205: 137
20251208: 230
20251209: 217
20251210: 213
20251211: 167
20251212: 220
20251213: 6
20251214: 11
20251215: 122
20251216: 138
20251217: 133
20251218: 157
20251219: 114
20251221: 1
20251222: 116
20251223: 253
20251224: 94
20251225: 212
20251226: 127
20251227: 1
20251228: 1
20251229: 164
20251230: 169
20251231: 161

### date-2026-01

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260101+TO+20260131]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:28.410968+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:29 GMT
HTTP status: 200
20260101: 2
20260102: 214
20260104: 2
20260105: 179
20260106: 173
20260107: 174
20260108: 159
20260109: 202
20260112: 192
20260113: 211
20260114: 195
20260115: 64
20260116: 111
20260117: 3
20260118: 6
20260119: 101
20260120: 159
20260121: 137
20260122: 193
20260123: 219
20260124: 12
20260126: 59
20260127: 196
20260128: 210
20260129: 216
20260130: 234

### date-2026-02

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260201+TO+20260228]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:28.932132+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:30 GMT
HTTP status: 200
20260202: 147
20260203: 290
20260204: 213
20260205: 235
20260206: 179
20260207: 2
20260208: 28
20260209: 158
20260210: 172
20260211: 176
20260212: 194
20260213: 194
20260214: 2
20260215: 2
20260216: 157
20260217: 225
20260218: 279
20260219: 205
20260220: 213
20260221: 10
20260222: 3
20260223: 142
20260224: 187
20260225: 215
20260226: 153
20260227: 245

### date-2026-03

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260301+TO+20260331]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:29.425142+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:30 GMT
HTTP status: 200
20260302: 228
20260303: 288
20260304: 216
20260305: 277
20260306: 202
20260307: 10
20260308: 1
20260309: 182
20260310: 113
20260311: 271
20260312: 192
20260313: 307
20260314: 13
20260316: 203
20260317: 230
20260318: 191
20260319: 160
20260320: 194
20260321: 2
20260322: 3
20260323: 198
20260324: 223
20260325: 210
20260326: 213
20260327: 1
20260330: 383
20260331: 219

### date-2026-04

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260401+TO+20260430]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:29.897418+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:31 GMT
HTTP status: 200
20260401: 228
20260402: 175
20260403: 210
20260404: 3
20260405: 1
20260406: 155
20260407: 150
20260408: 269
20260409: 190
20260410: 139
20260411: 41
20260412: 3
20260413: 226
20260414: 165
20260415: 271
20260416: 217
20260417: 189
20260418: 4
20260419: 5
20260420: 121
20260421: 207
20260422: 329
20260423: 123
20260424: 284
20260425: 11
20260426: 29
20260427: 260
20260428: 266
20260429: 445
20260430: 453

### date-2026-05

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260501+TO+20260531]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:30.371393+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:31 GMT
HTTP status: 200
20260501: 99
20260503: 74
20260504: 415
20260505: 389
20260506: 323
20260507: 296
20260508: 238
20260509: 1
20260511: 194
20260512: 208
20260513: 177
20260514: 316
20260515: 187
20260517: 2
20260518: 157
20260519: 131
20260520: 171
20260521: 169
20260522: 146
20260524: 1
20260525: 96
20260526: 284
20260527: 286
20260528: 194
20260529: 206
20260531: 54

### date-2026-06

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260601+TO+20260630]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:30.989504+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:32 GMT
HTTP status: 200
20260601: 260
20260602: 194
20260603: 298
20260604: 244
20260605: 225
20260606: 2
20260607: 1
20260608: 148
20260609: 135
20260610: 181
20260611: 259
20260612: 174
20260615: 158
20260616: 209
20260617: 143
20260618: 114
20260619: 248
20260620: 7
20260622: 181
20260623: 178
20260624: 159
20260625: 170
20260626: 196
20260627: 1
20260628: 4
20260629: 188
20260630: 276

### date-2026-07

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260701+TO+20260731]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:31.574173+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:32 GMT
HTTP status: 200
20260701: 170
20260702: 218
20260703: 143
20260705: 7
20260706: 223
20260707: 303
20260708: 216
20260709: 158
20260710: 124
20260711: 2
20260713: 116
20260714: 235
20260715: 142
20260716: 214
20260717: 122
20260718: 2
20260720: 160
20260721: 184
20260722: 77
20260727: 693
20260728: 140
20260729: 220
20260730: 173
20260731: 265

### date-2026-08

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260801+TO+20260831]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:32.065887+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:33 GMT
HTTP status: 200
20260803: 153
20260804: 168
20260805: 179
20260806: 230
20260807: 193
20260808: 2
20260809: 1
20260810: 143
20260811: 244
20260812: 207
20260813: 272
20260814: 171
20260816: 4
20260817: 225
20260818: 172
20260819: 186
20260820: 206
20260821: 176
20260822: 5
20260824: 178
20260825: 169
20260826: 209
20260827: 215
20260828: 184
20260830: 57
20260831: 152

### date-2026-09

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20260901+TO+20260930]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:32.860787+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:34 GMT
HTTP status: 200
20260901: 176
20260902: 290
20260903: 230
20260904: 193
20260905: 6
20260906: 5
20260907: 124
20260908: 226
20260909: 233
20260910: 215
20260911: 279
20260912: 5
20260913: 6
20260914: 141
20260915: 218
20260916: 249
20260917: 280
20260918: 297
20260919: 4
20260921: 171
20260922: 175
20260923: 207
20260924: 270
20260925: 197
20260926: 4
20260927: 5
20260928: 147
20260929: 250
20260930: 202

### date-2026-10

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261001+TO+20261031]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:33.444668+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:35 GMT
HTTP status: 200
20261001: 181
20261002: 36
20261004: 6
20261005: 156
20261006: 191
20261007: 193
20261008: 229
20261009: 206
20261010: 7
20261012: 192
20261013: 192
20261014: 253
20261015: 270
20261016: 299
20261017: 2
20261019: 190
20261020: 64
20261021: 204
20261022: 247
20261023: 217
20261025: 9
20261026: 220
20261027: 233
20261028: 286
20261029: 286
20261030: 203

### date-2026-11

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20261101+TO+20261117]&count=date_received&limit=100`
Requested at (UTC): 2026-11-17T02:51:34.271902+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:35 GMT
HTTP status: 404
(no results returned)

### death-by-manufacturer

Request: `https://api.fda.gov/device/event.json?search=device.device_report_product_code:FRN+AND+date_received:[20251117+TO+20261117]+AND+event_type:Death&count=device.manufacturer_d_name.exact&limit=100`
Requested at (UTC): 2026-11-17T02:51:35.204252+00:00
HTTP Date header: Tue, 17 Nov 2026 02:51:36 GMT
HTTP status: 200
FRESENIUS VIAL S.A.S: 20
CAREFUSION 303, INC.: 18
CAREFUSION SD: 13
B. BRAUN MELSUNGEN AG: 9
B BRAUN MELSUNGEN AG: 4
FRESENIUS VIAL S.A.S.: 4
BAXTER HEALTHCARE CORPORATION: 3
IRADIMED CORPORATION: 3
MILLYARD ADVANCED MEDICAL PRODUCTS, LLC: 3
ICU Medical, Inc.: 2
: 1
BECTON DICKINSON INFUSION THERAPY SYSTEMS INC. S.A. DE C.V.: 1
FRESENIUS KABI USA, LLC: 1
ICU Medical Costa Rica Ltd.: 1
Millyard Advanced Medical Products, LLC: 1
UNK: 1
ZYNO MEDICAL, LLC: 1
## PLATFORM RECORD

- PULL 1 note filed 2026-11-15 02:42:25 UTC (Synmerco server time): "PULL 1: pump-reports-pull1.csv — row count: 81, SHA-256: 51d9e3f9db7ab71763d7abb75e4b154e68c8f70bc33e3215b57247e0b5b6ee03."
- PULL 2 note filed 2026-11-16 02:48:13 UTC (Synmerco server time): "PULL 2: pump-reports-pull2.csv — row count: 81, SHA-256: a445e8938a1f57bd4b4add6aaf2e700f21a00be21583889b44f54cd50db03a77."
- PULL 3 note filed 2026-11-17 02:53:39 UTC (Synmerco server time): "PULL 3: pump-reports-pull3.csv — row count: 81, SHA-256: 7789c842fac000d3b5651a904480261e71ba09caccc45d0d2410062a0dc1bb5f."
- First PULL 3 note filed 2026-11-17 02:48:34 UTC was superseded by the note above: its pull ran with the wrong local date and covered 20251116 to 20261116 (the Pull 2 window) with SHA-256 a445e8938a1f57bd4b4add6aaf2e700f21a00be21583889b44f54cd50db03a77; the corrected pull ran 2026-11-17 02:51 UTC, range 20251117 to 20261117.
- Revision 1 update notes filed 2026-11-17 (Synmerco server time) for the rebuilt CSVs (same pulls, same source times): "PULL 1: pump-reports-pull1.csv — row count: 133, SHA-256: 92beb75c0c5af5d83c2191cc458a2a158587baec998c9a7e10208868e20fb2df" at 03:48:59 UTC; "PULL 2: pump-reports-pull2.csv — row count: 133, SHA-256: 9f8d1991ba50f35871847ffa2e2a5498eb548c5789cb5bf985c755718a205754" at 03:49:00 UTC; "PULL 3: pump-reports-pull3.csv — row count: 133, SHA-256: b85cc1d0406acc0b374d379c9cb2e7c3005630fd7c50b1fc8731ffe818b94637" at 03:49:02 UTC.
- Submit only after PULL 3; deadline 2026-11-19 10:31:37 UTC.

## DATA FILES

- D2. pump-reports-pull1.csv — row count: 133, SHA-256: 92beb75c0c5af5d83c2191cc458a2a158587baec998c9a7e10208868e20fb2df
- D3. pump-reports-pull2.csv — row count: 133, SHA-256: 9f8d1991ba50f35871847ffa2e2a5498eb548c5789cb5bf985c755718a205754
- D4. pump-reports-pull3.csv — row count: 133, SHA-256: b85cc1d0406acc0b374d379c9cb2e7c3005630fd7c50b1fc8731ffe818b94637
