# Stock Assessment — GitHub Copilot Skill

A structured investment research skill for GitHub Copilot. Give it a ticker or company name and it produces a full, scored stock assessment report across eight dimensions.

## Usage

In any workspace that contains this skill, type `/stock-assessment` in GitHub Copilot Chat followed by a ticker or company name:

```
/stock-assessment AAPL
/stock-assessment Microsoft
/stock-assessment NVDA
```

Copilot will work through all eight research steps and return a scored Markdown report.

---

## What It Researches

The skill investigates and scores the following areas, each rated **out of 5**:

| # | Section | What it covers |
|---|---------|---------------|
| 1 | **Initial Screening** | 10-year revenue growth, profitability, market cap gate (>$10B), net debt, institutional & superinvestor ownership |
| 2 | **Business Model** | Revenue segments, revenue quality (recurring vs transactional), geographic diversification, industry KPIs |
| 3 | **Financial Analysis** | Income statement trends, balance sheet health, cash flow & FCF conversion, 3/5/10-year CAGRs |
| 4 | **Strategy & Returns** | 5/10/15-year ROCE, ROIC, ROE averages; capital allocation (R&D, buybacks, dividends, M&A); competitive moat; customer sentiment |
| 5 | **Red Flags** | Management compensation alignment, insider buying vs selling (%), conflicts of interest, active litigation, news cycle sentiment |

### Scoring Scale

| Score | Meaning |
|-------|---------|
| 5 | Excellent |
| 4 | Good |
| 3 | Average |
| 2 | Below average |
| 1 | Poor / serious concern |

### Overall Verdict (out of 25)

| Total | Rating |
|-------|--------|
| 21–25 | Strong Buy candidate |
| 16–20 | Watchlist / Buy on weakness |
| 11–15 | Neutral — monitor |
| 6–10 | Caution |
| 1–5 | Avoid |

---

## Report Structure

Every assessment returns:

1. Company identification (exchange, sector, market cap)
2. Initial screening with gate checks
3. Business model breakdown (segments, revenue quality, geography, KPIs)
4. Financial analysis (income statement, balance sheet, cash flow, CAGRs)
5. Strategy evaluation (returns, capital allocation, moat, customer sentiment)
6. Red flags checklist (compensation, insider trading, conflicts, litigation, news)
7. SWOT table
8. Scored summary table + bull case / bear case / next steps

---

## Skill Structure

```
.github/skills/stock-assessment/
├── SKILL.md                        ← Main skill entry point
└── references/
    ├── screening-criteria.md       ← Revenue growth, debt, institutional ownership + business model guide
    ├── financial-analysis.md       ← Income statement, balance sheet, cash flow, CAGR framework
    ├── strategy-evaluation.md      ← ROCE/ROIC/ROE, capital allocation, moat, customer sentiment
    ├── red-flags.md                ← Compensation, insider trading, conflicts, litigation, news
    └── data-sources.md             ← Curated primary sources (EDGAR, Macrotrends, TIKR, OpenInsider, etc.)
```

---

## Primary Data Sources Used

- **SEC EDGAR** — 10-K, 10-Q, DEF 14A (proxy), Form 4 (insider trades), 13F (institutional holdings)
- **Company Investor Relations pages** — Annual reports, Investor Day decks, earnings supplements
- **Macrotrends / Stock Analysis / TIKR** — Multi-year financial history
- **WhaleWisdom / Dataroma** — Institutional and superinvestor ownership
- **OpenInsider** — Insider buy/sell transaction tracking
- **Trustpilot / App Store / Glassdoor** — Customer and employee sentiment
- **Reuters / FT / WSJ / Seeking Alpha** — News cycle and analyst commentary

---

## Example Output

See the [TSLA assessment example](./examples/TSLA-2026-06-15.md) *(add your saved reports here)*.

---

## Requirements

- GitHub Copilot with Agent mode enabled
- VS Code with the GitHub Copilot extension

## Disclaimer

This skill produces educational research outputs only. Nothing here constitutes financial advice. Always verify data against primary filings and consult a qualified financial adviser before making investment decisions.
