---
name: stock-assessment
description: "Use when evaluating a stock by ticker symbol or company name. Investigates growth trajectory, profitability, institutional ownership, business model, financials (income statement, balance sheet, cash flow), capital allocation, strategy, management behaviour, and red flags. Produces a scored report with section ratings out of 5 and an overall investment verdict. Triggers: 'assess stock', 'research stock', 'stock analysis', 'evaluate ticker', 'investment research'."
argument-hint: "Ticker symbol or company name (e.g. AAPL, Microsoft, TSLA)"
---

# Stock Assessment

A comprehensive, structured framework for evaluating any publicly traded company. Given a ticker or company name, produce a full investment research report across eight steps, five of which are scored out of 5.

## When to Use

- User provides a ticker symbol (e.g. `AAPL`, `TSLA`, `NVDA`) or company name
- User asks for a stock breakdown, investment research, or equity analysis
- User wants to understand a business before investing

## Procedure

Work through each section in order. Use web search, SEC EDGAR, and the company's Investor Relations page as primary sources. Score each section **out of 5** (5 = excellent, 3 = average, 1 = poor) and record a brief justification.

## Process Rules

Apply these rules throughout every assessment:

- **Cite every figure.** For each data point (revenue, margins, ROIC, insider %, etc.) state the source and the filing/period it came from (e.g. "FY2024 10-K", "Q1 2025 13F"). Prefer primary filings over aggregators.
- **Never fabricate data.** If a figure cannot be found or verified, write `data unavailable — not verified` and reflect the gap in the section score and justification. Do not estimate or infer numbers and present them as fact.
- **Date everything.** Record the assessment date and the as-of date of the price and figures used; financial data goes stale quickly.
- **Separate fact from judgement.** Keep reported numbers distinct from your interpretation of them.

---

### Step 1 — Identify the Company

1. Confirm the full legal company name, primary exchange, and ticker.
2. Identify the sector and industry classification (GICS).
3. Note the current market capitalisation and the current share price (record the as-of date).
4. **Size context** (not a disqualifier): classify by market cap — small-cap < $2B, mid-cap $2–10B, large-cap > $10B. Flag small/mid-caps for higher risk and thinner institutional coverage. See [./references/screening-criteria.md](./references/screening-criteria.md).

---

### Step 2 — Initial Screening

Follow the criteria in [./references/screening-criteria.md](./references/screening-criteria.md).

Key checks:
- 10-year revenue growth trend (positive / accelerating / decelerating / negative)
- Current profitability (net income positive last 3 years)
- Market cap size context (large / mid / small — context, not a hard disqualifier)
- Net debt / EBITDA ratio (target < 3×)
- Institutional and notable investor ownership — who is buying or considering?

**Score this section /5.**

---

### Step 3 — Business Model & Competitive Position

Follow the guidance in [./references/screening-criteria.md](./references/screening-criteria.md) (Part B — Business Model Analysis).

Key checks:
- Revenue segments and their relative contribution
- Revenue characteristics (recurring vs. transactional, contracted vs. spot)
- Geographic diversification and concentration risk
- Key Performance Indicators specific to the industry
- Sources: company 10-K/20-F, Investor Day presentations, IR page

**Score this section /5.**

---

### Step 4 — Financial Analysis

Follow the full framework in [./references/financial-analysis.md](./references/financial-analysis.md).

Key checks:
- Income Statement: revenue, gross margin, EBITDA margin, net margin trends (5–10 yr)
- Balance Sheet: debt levels, cash position, goodwill / intangibles as % of assets
- Cash Flow: free cash flow conversion, capex intensity
- CAGR: 3yr, 5yr, 10yr revenue and EPS CAGR
- Capital allocation: R&D spend, dividend / buyback history, acquisition activity

**Score this section /5.**

---

### Step 5 — Strategy Evaluation

Follow the framework in [./references/strategy-evaluation.md](./references/strategy-evaluation.md).

Key checks:
- 5/10/15-year averages for ROCE, ROIC, ROE
- Capital allocation priorities (growth investment vs. debt paydown vs. buybacks vs. dividends)
- Competitive moat indicators (pricing power, switching costs, network effects)
- Customer satisfaction signals (NPS data, app store reviews, Trustpilot, Reddit sentiment)

**Score this section /5.**

---

### Step 6 — Red Flags

Follow the checklist in [./references/red-flags.md](./references/red-flags.md).

Key checks:
- Management compensation structure and alignment with shareholders
- Insider buying vs. selling (% of holdings traded, net direction over 12 months)
- Conflicts of interest on the board
- Active litigation or regulatory investigations
- Recent press releases and news cycle sentiment
- Congressional & Presidential trading (STOCK Act disclosures, committee relevance, executive branch holdings — see [./references/red-flags.md](./references/red-flags.md) Section 6 and [./references/data-sources.md](./references/data-sources.md) Congressional Trading section)

**Score this section /5** (5 = clean, no flags; 1 = multiple serious red flags). The Red Flags score is an average of six sub-areas: Compensation, Insider Trading, Conflicts, Litigation, News, and Congressional & Presidential Trading.

---

### Step 7 — SWOT Summary

Produce a concise SWOT table:

| Strengths | Weaknesses |
|-----------|------------|
| ...       | ...        |

| Opportunities | Threats |
|---------------|---------|
| ...           | ...     |

---

### Step 8 — Overall Verdict

Compile the scored report into a **Quality Score**, apply a **valuation overlay**, then produce a final verdict.

**Quality Score Table**

| Section | Score /5 | Key Finding |
|---------|----------|-------------|
| Initial Screening | | |
| Business Model | | |
| Financial Analysis | | |
| Strategy & Returns | | |
| Red Flags | | |
| **Quality Total** | **/25** | |

**Quality Rating** (Total / 25):
- 21–25 → Excellent business quality
- 16–20 → Good quality
- 11–15 → Average quality
- 6–10 → Below-average quality
- 1–5 → Poor quality

**Valuation Overlay**

The Quality Score measures business *quality only* — not price. A great business at the wrong price is not a buy. Classify the current valuation against the company's own history and close peers using at least two of:
- P/E (vs. 5-year median and peers)
- EV/EBITDA (vs. 5-year median and peers)
- P/FCF or FCF yield (vs. 5-year median and peers)

Classify valuation as **Cheap / Fair / Expensive** and state the multiples and references used. See [./references/data-sources.md](./references/data-sources.md) (Valuation Context).

**Final Verdict** — combine quality and valuation:

| Quality | Valuation | Verdict |
|---------|-----------|---------|
| High (16+) | Cheap / Fair | Buy candidate |
| High (16+) | Expensive | Watchlist — buy on weakness |
| Average (11–15) | Cheap | Speculative — monitor |
| Average (11–15) | Fair / Expensive | Neutral — monitor |
| Low (≤10) | Any | Avoid |

Conclude with:
1. **Bull case** (2–3 sentences)
2. **Bear case** (2–3 sentences)
3. **Suggested next steps** (e.g. dig into Q-earnings, await catalyst, review again at next earnings)

---

## Data Sources

See [./references/data-sources.md](./references/data-sources.md) for the full list of primary sources for each section (EDGAR, IR pages, news aggregators, ownership databases).

## Output Format

Always produce the full report in structured Markdown with:
- A header line: `**{Company} ({Exchange}: {Ticker})** — assessed {date}, share price {price} {currency}`
- Section headers matching the eight steps above
- Score callout for each scored section (e.g. `**Score: 4/5**`), with a one-line justification and cited sources
- SWOT table
- Quality Score table, valuation overlay, and final verdict
- A closing disclaimer: *This is educational research only, not financial advice. Verify all figures against primary filings before making any investment decision.*
