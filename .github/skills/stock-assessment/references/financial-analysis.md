# Financial Analysis Reference

Primary sources for all data below:
- SEC EDGAR (10-K, 10-Q): https://www.sec.gov/cgi-bin/browse-edgar
- Company Investor Relations page (annual reports, earnings supplements)
- Macrotrends: https://www.macrotrends.net
- Stock Analysis: https://stockanalysis.com
- TIKR Terminal: https://tikr.com

---

## 1. Income Statement Analysis

### What to Pull (5–10 year history)

| Line Item | What to Look For |
|-----------|-----------------|
| Revenue | Growth trend — accelerating, stable, decelerating |
| Gross Profit & Margin | Is pricing power holding? Is margin stable or expanding? |
| Operating Income (EBIT) | Operating leverage — does margin expand faster than revenue? |
| EBITDA & EBITDA Margin | Cash earnings proxy; compare to peers |
| Net Income | Accounting-clean earnings; check for large one-offs |
| EPS (diluted) | Growing? Share count dilution eating into EPS? |
| R&D as % of Revenue | Investment level vs. peers; is it growing or being cut? |

### Red Lines

- Gross margin declining 3+ years in a row → pricing pressure or cost creep
- Revenue growing but net income flat or falling → margin erosion
- Heavy reliance on one-time gains for profitability

### Scoring Guide — Income Statement

- 5 — Revenue + EPS both growing double-digits; expanding margins; clean earnings
- 4 — Solid revenue growth; stable/improving margins; minor one-offs
- 3 — Moderate growth; flat margins; some non-recurring items
- 2 — Slow growth or stagnant earnings; compressing margins
- 1 — Revenue declining or losses; margin deterioration; heavy adjustments

---

## 2. Balance Sheet Analysis

### What to Pull (last 3–5 years)

| Item | What to Look For |
|------|-----------------|
| Cash & Equivalents | Trend — building or depleting? |
| Total Debt (short + long-term) | Absolute level and trend |
| Net Debt | Total Debt − Cash (negative = net cash = fortress) |
| Shareholders' Equity | Growing? Or being eroded by buybacks / losses? |
| Goodwill & Intangibles | As % of total assets — inflated goodwill signals overpaying for acquisitions |
| Current Ratio | Current Assets / Current Liabilities (>1.5 preferred) |
| Debt/Equity Ratio | Higher = more leveraged |

### Goodwill Watch

- Goodwill > 30% of total assets: scrutinise acquisition history
- Any impairment charges in the last 3 years: management overpaid

### Scoring Guide — Balance Sheet

- 5 — Net cash position; low debt; clean book; goodwill < 20% of assets
- 4 — Low net debt (< 1× EBITDA); healthy equity; minimal goodwill risk
- 3 — Moderate net debt; some goodwill; current ratio adequate
- 2 — High leverage (> 3× EBITDA); deteriorating equity or large goodwill
- 1 — Over-leveraged; equity declining; goodwill impairments or going-concern risk

---

## 3. Cash Flow Statement Analysis

### What to Pull (5–10 year history)

| Item | What to Look For |
|------|-----------------|
| Operating Cash Flow (OCF) | Should track closely to net income; divergence = quality issue |
| Capital Expenditure (Capex) | Maintenance vs. growth capex — ideally stated by management |
| Free Cash Flow (FCF) | OCF − Capex; the lifeblood of shareholder value |
| FCF Margin | FCF / Revenue (> 10% is healthy; > 20% is exceptional) |
| FCF Conversion | FCF / Net Income (> 90% preferred) |

### Cash Allocation Waterfall

Trace where FCF goes each year:
1. **Organic reinvestment** — R&D, capex, working capital
2. **Acquisitions** — M&A activity
3. **Debt repayment** — deleveraging
4. **Dividends** — income to shareholders
5. **Buybacks** — returning capital by reducing share count

A company consistently buying back shares at reasonable valuations = strong signal.
A company buying back shares while taking on debt = red flag.

### Scoring Guide — Cash Flow

- 5 — Strong, growing FCF; FCF margin > 15%; high conversion; disciplined capital allocation
- 4 — Consistent FCF; good conversion; sensible allocation mix
- 3 — Positive but lumpy FCF; moderate conversion; some capex-heavy years
- 2 — Weak or negative FCF in recent years; poor conversion; heavy M&A
- 1 — Persistently negative FCF; cash burn; unclear path to FCF generation

---

## 4. Cumulative Average Growth Rate (CAGR)

Calculate and record for **Revenue**, **EPS**, and **FCF**:

| Period | Formula |
|--------|---------|
| 3-year CAGR | (Value_now / Value_3yr_ago)^(1/3) − 1 |
| 5-year CAGR | (Value_now / Value_5yr_ago)^(1/5) − 1 |
| 10-year CAGR | (Value_now / Value_10yr_ago)^(1/10) − 1 |

**Benchmarks:**
- Revenue CAGR > 10% over 10 years → strong compounder
- EPS CAGR should match or exceed Revenue CAGR (margin expansion)
- FCF CAGR > Revenue CAGR → improving capital efficiency

**Scoring Guide — CAGRs**

- 5 — Revenue 10-yr CAGR > 12%; EPS CAGR > Revenue CAGR; FCF CAGR > 10%
- 4 — Revenue CAGR 8–12%; EPS growing faster than revenue
- 3 — Revenue CAGR 4–7%; EPS broadly in line
- 2 — Revenue CAGR 1–3%; EPS lagging revenue
- 1 — Negative or near-zero revenue CAGR; EPS declining

---

## Combined Financial Score

Average the sub-scores from Income Statement, Balance Sheet, Cash Flow, and CAGR to arrive at the single **Financial Analysis score out of 5** reported in the main assessment.

**Cap rule:** If any sub-area scores **1** (e.g., going-concern risk on the balance sheet, or persistently negative FCF with no clear path to profitability), cap the combined Financial Analysis score at **2**, regardless of how the other sub-areas score.

---

## Sector-Specific Adaptations

Standard EBITDA / leverage / FCF metrics do not translate cleanly across all industries. Apply the adaptations below before scoring Steps 2 and 4.

---

### Banking & Financial Institutions

Replace or supplement standard metrics with banking-specific equivalents:

| Standard Metric | Banking Equivalent | Source |
|---|---|---|
| Revenue growth | Net Interest Income (NII) + Fee income growth | 10-K / earnings release |
| Operating / EBITDA margin | Return on Tangible Equity (RoTE) and Cost-to-Income ratio | 10-K |
| Net Debt / EBITDA | CET1 Capital Ratio (regulatory comfort ≥ 12%) | Basel III Pillar 3 disclosure |
| Gross margin | Net Interest Margin (NIM) | Earnings supplement |
| FCF yield | Dividend payout from distributable earnings; Loan-to-Deposit Ratio (LDR) | 10-K |

Additional KPIs to track: Non-Performing Loan (NPL) ratio, Loan Loss Provision trend, Tangible Book Value per share.

> **Do not** apply Net Debt / EBITDA to banks — their balance sheet structure (customer deposits counted as liabilities) makes this metric meaningless. Use regulatory capital ratios instead.

---

### Exchange Operators & Financial Market Infrastructure

| Issue | Adaptation |
|---|---|
| Gross vs. net revenue | Exchanges pass through transaction-based fees (e.g. payments to liquidity providers, regulatory fees). Always use **net revenues** (after transaction-based expenses) as the meaningful revenue metric. These typically equal the "Gross Profit" line in standardised financial data aggregators. |
| Clearing house assets | Central counterparty clearing (CCP) balance sheets include member performance bonds that are not the exchange's own capital. For example, CME Group reported ~$165B in "Other Current Assets" that are matched dollar-for-dollar by equivalent current liabilities. **Exclude these clearing house items** from leverage, asset turnover, and working capital calculations. Use only operational debt vs. operational EBITDA for leverage ratios. |
| KPIs | Average Daily Volume (ADV), Rate Per Contract (RPC), Annual Recurring Revenue (ARR) for data/software segments, Remaining Performance Obligations (RPO), open interest |

---

### Pre-Profitability Growth Companies

When GAAP net income is consistently negative (early-stage hardware, growth SaaS in scaling phase, pre-revenue biotech):

- Do **not** apply a score of 1 to the FCF sub-area solely because FCF is negative, if the company has adequate cash runway (> 18 months) and a credible path to profitability
- Prioritise: **gross margin trajectory** (is gross margin expanding toward a sustainable model?), **revenue growth rate**, and **cash runway** (months until next required capital raise)
- **Cap the FCF sub-score at 3** (not 1) during a deliberate investment phase — but reduce further if the burn rate is accelerating without revenue progress
- State the pre-profitability status explicitly in Steps 2 and 4, and note estimated months of runway

---

### Cyclical Industrials with Captive Finance Subsidiaries

Companies such as Caterpillar, John Deere, and CNH Industrial operate a captive finance arm (e.g., Cat Financial) that provides customer financing for equipment purchases. This inflates consolidated leverage artificially.

- Separate **industrial segment** operating metrics from the **financial products segment** leverage when calculating Net Debt / EBITDA
- Use **industrial-only net debt / EBITDA** as the primary leverage metric, and note total consolidated leverage separately
- The finance subsidiary debt is self-funding (backed by equipment-loan receivables); treat it analogously to a bank's deposit-funded loan book — high gross leverage that is not operationally risky
- Source segment-level balance sheet data from the 10-K segment footnotes

---

### ADRs and Foreign Primary Listings

When a company's primary listing is outside the US but trades as an American Depositary Receipt (ADR) or American Depositary Share (ADS):

- Always confirm the **ADR ratio** before using any per-share metrics (e.g. AstraZeneca: 1 ADS = 2 ordinary shares; HSBC: 1 ADS = 4 ordinary shares; GSK: 1 ADS = 2 ordinary shares)
- Source the ratio from the company's ADR programme page or the depositary bank (BNY Mellon, Citibank, JPMorgan)
- Convert all per-share figures — EPS, DPS, Book Value per share — to **per-ADS basis** before comparing against the ADS market price
- Dividend yields should use the USD-denominated ADS dividend (which may differ from the local-currency ordinary share dividend due to FX conversion and timing)
- Note the primary listing exchange and currency, and state both the ADS price and the implied ordinary share price
