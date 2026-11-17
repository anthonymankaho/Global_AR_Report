# Global AR Report — Meyer Group

Monthly **third-party accounts receivable ageing** pack for the Meyer group, published for the
MyVault OS **Report** register (same pattern as the MTC Performance Report).

## September 2026 edition

| Item | Value |
|---|---|
| Position | 30-Sep-2026 |
| Prepared | 17-Nov-2026 |
| Reporting currency | USD |
| Entities | MHK · MTC · MMC · MTL (Myrex Thailand) · MUS · MIN (new) |
| Missing entities | **MUK, MCA, TVS, MJP not provided** — not a full-group position |
| Net third-party AR | USD 44,906,050.48 |
| Gross book | USD 462,487,509.42 (intercompany / related / consignment eliminated: USD 417,581,458.94) |
| Current | 77.3% |
| Reconciliation controls | 23 / 23 PASS |

## Files

- `Global_AR_Ageing_Report_2026-09.html` — dynamic exhibit pack (aging, entity drill, gross→net
  bridge, top-10 exposures, risk flags, filterable customer explorer, CSV export, FX & controls).
  Browser login: first-use administrator **GLOBALAR / GLOBALAR**. The login is a **workflow gate
  only** — customer data is embedded in the file and readable by anyone with file/URL access.
- `Global_AR_Ageing_Report_2026-09.xlsx` — companion workbook: Summary, Combined Aging (USD),
  per-entity sheets, IC & Exclusions bridge, FX Rates, Controls.
- `index.html` — redirect to the latest edition.

## Basis

- FX: `STANDARD EXCHANGE RATE-2026-09.xls`, HK DOLLAR standard column (= Market Rate), USD/HKD 7.8.
- INR (MIN): absent from the standard file — Sep-2026 average PACIFIC USD/INR **95.5022**
  (20 daily quotes 01–29 Sep, `FIN_Ex Rate_PSBUILD_20261115.xlsx`, Data sheet). Reference rate,
  not a finance-approved standard rate.
- Eliminations cross-checked against the group entity registry (Aug workbook `Inter-companies`):
  incl. TVS SPA (T.V.S. s.p.a.), HESTAN SMART COOKING INC (HSC), RUFFONI SRL (treated as
  Ruffoini S.r.l. RFN — **name variant, owner to confirm**). MTL 17 “-CS” consignment customers
  excluded per Aug policy. MTL ≤30→Current mapping is an Aug assumption — confirm.
- Build pipeline (working folder, not published here):
  `Desktop\Global AR Report\2026-09\_build\build_sept_report.py` → `inject_html.py`.
  Source workbooks are deliberately **not** committed (see `PROCESSING.md` in the working folder).

## Privacy

INTERNAL USE ONLY. Customer-level data is embedded. `noindex,nofollow,noarchive` is set on all
pages, but this is a public GitHub Pages site — treat the URL as access-controlled by obscurity
plus the workflow gate only. Do not circulate externally.
