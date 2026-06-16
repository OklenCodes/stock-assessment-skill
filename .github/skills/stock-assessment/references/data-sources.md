# Data Sources Reference

A curated list of primary and secondary sources for each section of the stock assessment.

---

## Regulatory Filings

### United States — SEC EDGAR

URL: https://www.sec.gov/cgi-bin/browse-edgar

| Filing | Contains | Use For |
|--------|----------|---------|
| 10-K (Annual Report) | Full financials, risk factors, business overview, legal proceedings, executive comp | Financials, Red Flags, Business Model |
| 10-Q (Quarterly Report) | Interim financials, MD&A | Tracking quarterly trend |
| DEF 14A (Proxy) | Executive compensation, board composition, related-party transactions | Red Flags: Compensation, Conflicts |
| Form 4 | Insider buy/sell transactions (filed within 2 days) | Red Flags: Insider Trading |
| 13F (Institutional Holdings) | Institutional ownership snapshot (filed quarterly, 45-day lag) | Screening: Institutional Ownership |
| 8-K (Material Events) | Earnings releases, leadership changes, M&A announcements | Red Flags: News |
| S-1 / S-3 | Registration statements — useful for recent IPOs or capital raises | Business Model |

**Search tips:**
- Use "Full-Text Search" on EDGAR for specific topics inside filings
- Set Filing Type to `10-K` and Date Range for historical comparisons

---

### United Kingdom — Companies House & LSE

| Source | URL | Use For |
|--------|-----|---------|
| Companies House | https://find-and-update.company-information.service.gov.uk | Annual reports, confirmation statements |
| London Stock Exchange | https://www.londonstockexchange.com/live-markets/market-data-and-news | Regulatory news service (RNS) |
| FCA Register | https://register.fca.org.uk | Regulatory status, enforcement actions |

### Europe / Rest of World

- Always check the company's own **Investor Relations** page (usually at `ir.<company>.com` or `investors.<company>.com`)
- Annual reports filed with the local exchange or regulator
- SEDAR (Canada): https://www.sedar.com
- ASIC (Australia): https://www.asic.gov.au

---

## Financial Data & Charting

| Tool | URL | Best For |
|------|-----|---------|
| Macrotrends | https://www.macrotrends.net | 10–20 year historical financials; free |
| Stock Analysis | https://stockanalysis.com | Clean financials, quick CAGR snapshots |
| TIKR Terminal | https://tikr.com | Institutional-quality multi-year data; free tier available |
| Wisesheets | https://wisesheets.io | Excel/Sheets integration with EDGAR data |
| Simplywall.st | https://simplywall.st | Visualised fundamentals, analyst consensus |
| Koyfin | https://koyfin.com | Advanced charting, peer comparisons |
| GuruFocus | https://www.gurufocus.com | ROIC/ROCE/ROE history, intrinsic value estimates |

---

## Institutional Ownership & Superinvestor Tracking

| Tool | URL | Best For |
|------|-----|---------|
| WhaleWisdom | https://whalewisdom.com | 13F aggregation; hedge fund heatmaps |
| Dataroma | https://www.dataroma.com | Superinvestor portfolios (Buffett, Ackman, Munger, etc.) |
| Finviz | https://finviz.com | Institutional ownership %, short interest |
| OpenInsider | https://openinsider.com | Form 4 insider transactions with filters |
| SEC 13F search | https://efts.sec.gov/LATEST/search-index?q=%22ticker%22&dateRange=custom&startdt=2024-01-01&forms=13F-HR | Direct 13F search |

---

## News & Sentiment

| Source | URL | Best For |
|--------|-----|---------|
| Seeking Alpha | https://seekingalpha.com | Analyst opinions, earnings call transcripts |
| Reuters | https://www.reuters.com | Breaking institutional-quality news |
| Bloomberg | https://www.bloomberg.com | Premium financial news |
| Financial Times | https://www.ft.com | Global business reporting |
| CNBC | https://www.cnbc.com | US market news, executive interviews |
| Google News | https://news.google.com | Aggregated news; search `"{Company}" site:reuters.com OR site:wsj.com` |

---

## Customer & Brand Sentiment

| Source | URL | Best For |
|--------|-----|---------|
| Trustpilot | https://www.trustpilot.com | Consumer reviews; trend over time |
| Apple App Store | https://apps.apple.com | Mobile app quality and customer satisfaction |
| Google Play Store | https://play.google.com | Android app reviews |
| Glassdoor | https://www.glassdoor.com | Employee sentiment; management approval rating |
| Reddit | https://www.reddit.com | Subreddits for the company/product; r/investing |
| G2 / Capterra | https://www.g2.com | B2B software product reviews |

---

## Litigation & Regulatory

| Source | URL | Best For |
|--------|-----|---------|
| PACER | https://pacer.uscourts.gov | US federal court filings |
| SEC Enforcement | https://www.sec.gov/litigation/litreleases | SEC enforcement actions and press releases |
| DOJ Press Releases | https://www.justice.gov/news | DOJ corporate investigations |
| FTC Actions | https://www.ftc.gov/news-events/news/press-releases | Antitrust and consumer protection |
| 10-K Item 3 | SEC EDGAR | "Legal Proceedings" section in annual report |

---

## Valuation Context (Optional Add-On)

These sources help contextualise whether the stock is cheap or expensive relative to its quality score:

| Tool | URL | Notes |
|------|-----|-------|
| GuruFocus GF Value | https://www.gurufocus.com | Intrinsic value estimate with grade |
| Morningstar Fair Value | https://www.morningstar.com | Analyst fair value with moat rating |
| DCF calculators | Various | Build your own in Excel using FCF projections |
| P/E, EV/EBITDA, P/FCF | Koyfin / TIKR | Peer comparison multiples |
