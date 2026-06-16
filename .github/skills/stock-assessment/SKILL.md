---
name: stock-assessment
description: "Use when evaluating a stock by ticker symbol or company name. Investigates growth trajectory, profitability, institutional ownership, business model, financials (income statement, balance sheet, cash flow), capital allocation, strategy, management behaviour, and red flags. Produces a scored report with section ratings out of 5 and an overall investment verdict. Triggers: 'assess stock', 'research stock', 'stock analysis', 'evaluate ticker', 'investment research'."
argument-hint: "Ticker symbol or company name (e.g. AAPL, Microsoft, TSLA)"
---

# Stock Assessment

A comprehensive, structured framework for evaluating any publicly traded company. Given a ticker or company name, produce a full investment research report across eight scored dimensions.

## When to Use

- User provides a ticker symbol (e.g. `AAPL`, `TSLA`, `NVDA`) or company name
- User asks for a stock breakdown, investment research, or equity analysis
- User wants to understand a business before investing

## Procedure

Work through each section in order. Use web search, SEC EDGAR, and the company's Investor Relations page as primary sources. Score each section **out of 5** (5 = excellent, 3 = average, 1 = poor) and record a brief justification.

---

### Step 1 — Identify the Company

1. Confirm the full legal company name, primary exchange, and ticker.
2. Identify the sector and industry classification (GICS).
3. Note the current market capitalisation.
4. **Gate check**: If market cap < $10B, flag as small-cap and note higher risk profile.

---

### Step 2 — Initial Screening

Follow the criteria in [./references/screening-criteria.md](./references/screening-criteria.md).

Key checks:
- 10-year revenue growth trend (positive / accelerating / decelerating / negative)
- Current profitability (net income positive last 3 years)
- Market cap > $10B (investable universe gate)
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

**Score this section /5** (5 = clean, no flags; 1 = multiple serious red flags).

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

Compile the scored report and produce a final verdict.

**Scoring Table**

| Section | Score /5 | Key Finding |
|---------|----------|-------------|
| Initial Screening | | |
| Business Model | | |
| Financial Analysis | | |
| Strategy & Returns | | |
| Red Flags | | |
| **Total** | **/25** | |

**Overall Rating** (Total / 25):
- 21–25 → Strong Buy candidate — high conviction
- 16–20 → Watchlist / Buy on weakness
- 11–15 → Neutral — needs monitoring
- 6–10 → Caution — significant concerns
- 1–5 → Avoid — multiple red flags

Conclude with:
1. **Bull case** (2–3 sentences)
2. **Bear case** (2–3 sentences)
3. **Suggested next steps** (e.g. dig into Q-earnings, await catalyst, review again at next earnings)

---

## Data Sources

See [./references/data-sources.md](./references/data-sources.md) for the full list of primary sources for each section (EDGAR, IR pages, news aggregators, ownership databases).

## Output Format

Always produce the full report in structured Markdown with:
- Section headers matching the eight steps above
- Score callout for each section (e.g. `**Score: 4/5**`)
- SWOT table
- Final scoring table and verdict
