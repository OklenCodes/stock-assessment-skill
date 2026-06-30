# Red Flags Reference

A clean bill of health here scores 5. Each flag found reduces the score. Multiple serious flags = score of 1–2.

---

## 1. Management Compensation

Sources: Proxy statement (DEF 14A) filed annually with the SEC, or the Remuneration Report in UK/Australian annual reports.

### What to Check

| Item | Green Flag | Red Flag |
|------|------------|----------|
| CEO pay ratio | Reasonable vs. median employee; < 100:1 preferred | > 500:1 with no performance justification |
| Pay-for-performance alignment | Compensation tied to ROIC, FCF, multi-year TSR | Compensation tied to revenue or adjusted EBITDA only (can be gamed) |
| Long-term incentive vesting | 3–5 year cliff or ramp vesting | Short vesting periods (< 2 years) or immediate cash bonuses |
| Clawback provisions | Yes — bonuses recoverable on restatement | No clawback provisions |
| Equity dilution | Low annual dilution (< 1% of shares) | > 2% annual dilution from stock-based compensation |

**Scoring guide:**
- 5 — Long-term aligned compensation; meaningful clawback; low dilution
- 4 — Broadly aligned; minor concerns on metrics chosen
- 3 — Adequate but heavy cash bonuses or marginal metrics
- 2 — Generous pay with weak performance linkage; dilution > 1.5%
- 1 — Excessive pay; no performance linkage; high dilution; no clawback

---

## 2. Insider Buying vs. Selling

Sources:
- SEC Form 4 (US) filings: https://www.sec.gov/cgi-bin/browse-edgar (Form Type: 4)
- OpenInsider: https://openinsider.com
- Finviz insider tracker: https://finviz.com (Insider Trading section)
- UK: PDMR disclosures on the company's RNS/LSE page
- Non-US issuers / ADRs: Form 4 does not apply. Use local insider/PDMR disclosure regimes (UK RNS, EU MAR, etc.); for many ADRs and foreign filers US insider data is unavailable — note this gap rather than inferring.

### Framework

For each executive and director, calculate over the trailing 12 months:
- Total shares acquired (open market purchases, not options exercises)
- Total shares sold
- Net direction: net buyer or net seller?
- % of personal holding bought or sold

| Signal | Interpretation |
|--------|---------------|
| CEO/CFO buying on the open market | Strong conviction — they believe shares are undervalued |
| Multiple directors buying in same period | Cluster buy signal — high conviction |
| Routine diversification selling (< 10% of holding) | Normal; no concern |
| Selling > 25% of personal holding in 12 months | Potential concern — note if it coincides with high valuation |
| Selling after poor quarters | Major red flag — lack of confidence in turnaround |
| 10b5-1 plan sales | Pre-planned; less meaningful than discretionary sales |

**Scoring guide:**
- 5 — Net insiders buying; cluster buy signals; < 5% of holdings sold
- 4 — Broadly neutral; minor diversification selling; no concerning patterns
- 3 — Mixed; some notable selling but balanced by routine purchases
- 2 — Net insider selling > 15% of holdings; multiple executives selling
- 1 — Heavy insider selling; executives departing; CEO/CFO selling large blocks

---

## 3. Conflicts of Interest

Sources: Proxy statement (DEF 14A) — Related Party Transactions section.

### What to Check

- Board independence: are the majority of directors truly independent?
- Related-party transactions: is the company paying above-market rates to entities connected to directors or executives?
- Dual-class share structures: do founders retain disproportionate voting control with minimal economic skin?
- Audit committee quality: are members financially literate and independent?
- Revolving door: do management frequently move between the company and key customers/suppliers?

**Scoring guide:**
- 5 — Majority independent board; no material related-party transactions; aligned capital structure
- 4 — Mostly independent; minor related-party activity below $1M; single-class shares
- 3 — Some conflicts disclosed; dual-class shares but founder still operationally active
- 2 — Material related-party transactions; low board independence; dual-class with no governance roadmap
- 1 — Egregious conflicts; self-dealing; board captured by insiders; zero accountability mechanisms

---

## 4. Active Litigation & Regulatory Risk

Sources:
- 10-K — "Legal Proceedings" section (Item 3) and "Risk Factors" (Item 1A)
- PACER (US federal court filings): https://pacer.uscourts.gov
- SEC enforcement actions: https://www.sec.gov/litigation/litreleases
- News searches: "{Company} lawsuit", "{Company} SEC investigation", "{Company} DOJ"

### What to Classify

| Type | Severity |
|------|---------|
| Routine commercial disputes (< $10M) | Low |
| Patent / IP litigation | Medium — monitor outcome |
| Customer / product liability class action | High — damages + reputational |
| SEC / DOJ / FTC investigation | Very High — existential risk |
| Antitrust investigation | Very High |
| Data breach / GDPR action | High — fines + brand damage |
| Accounting restatements | Critical — destroys trust in financials |

**Scoring guide:**
- 5 — No material litigation; no regulatory investigations
- 4 — Routine disputes only; no SEC/DOJ involvement
- 3 — One active case of moderate severity; company well-resourced to defend
- 2 — Multiple cases; one significant class action or regulatory probe
- 1 — SEC/DOJ investigation; accounting restatement; class action with material damages risk

---

## 5. Press Releases & News Cycle Sentiment

Scan last 3–6 months of news:
- Reuters, Bloomberg, FT, WSJ — institutional quality reporting
- Seeking Alpha — analyst community sentiment
- Company press releases — tone and frequency of profit warnings

### Warning Patterns

| Pattern | Concern Level |
|---------|--------------|
| Repeated guidance downgrades | High — management credibility issue |
| Sudden CFO or CEO departure | High — investigate cause |
| Auditor change | Medium-High — ask why |
| Unusual acquisition or divestiture | Medium — strategic pivot or desperation? |
| Product recall or safety issue | Medium-High — liability and brand damage |
| Positive press releases but deteriorating financials | High — financial PR spin |
| Analyst coverage being dropped | Medium — loss of institutional interest |

**Scoring guide:**
- 5 — Positive or neutral news; management beat and raise; stable leadership team
- 4 — Minor negative news; well-managed communications; no leadership instability
- 3 — Some guidance cuts; mixed press; one leadership change with clear succession
- 2 — Repeated profit warnings; management credibility questioned; negative press cycle
- 1 — Crisis communications; leadership vacuum; major negative media exposure

---

## 6. Congressional & Presidential Trading

Politicians subject to the STOCK Act (US) must disclose trades within **30–45 days**. These disclosures can be green or red signals depending on context — especially when the trading member sits on a committee with oversight of the company's sector.

Sources:
- **Capitol Trades**: https://www.capitoltrades.com — search by ticker; shows individual legislator trades, committee memberships, party
- **Quiver Quantitative — Congress Trading**: https://www.quiverquant.com/congresstrading/ — aggregated congressional trade data by stock
- **House Financial Disclosures**: https://disclosures.house.gov — official STOCK Act filings (House members)
- **Senate Financial Disclosures**: https://efts.senate.gov/LATEST/search-index — official STOCK Act filings (Senate members)
- **Office of Government Ethics (OGE)**: https://www.oge.gov/web/oge.nsf/Presidential+Financial+Disclosure — presidential and executive branch disclosures
- **White House ethics pledges / annual financial disclosures** — listed on OGE and White House official releases

### What to Check

**Step 1 — Congressional activity**
1. Search Capitol Trades and Quiver Quant for the ticker. Record:
   - Number of distinct legislators who have traded the stock in the last 24 months
   - Net direction: more buyers than sellers, or vice versa?
   - Committee relevance: do any trading members sit on committees with direct oversight of the company's sector (e.g. Senate Banking, House Energy & Commerce, Senate Armed Services)?
2. Classify each significant trade:

| Signal | Interpretation |
|--------|---------------|
| Multiple legislators buying — especially those on relevant oversight committees | Positive signal — informed conviction; potential policy tailwind |
| Bipartisan cluster buying | Stronger positive signal — cross-aisle confidence |
| Cluster selling before a regulatory announcement or negative news | Red flag — potential information asymmetry or insider access |
| Single legislator buying/selling (routine portfolio management) | Neutral — note but do not overweight |
| Legislator sells entire position shortly before bad news | High concern — potential misuse of non-public information |

**Step 2 — Presidential / executive branch activity**
1. Check OGE annual financial disclosure for the sitting president and immediate family members.
2. Note any holdings, purchases, or disposals in the stock or closely related entities.
3. Check for executive orders, White House policy announcements, or regulatory actions that could directly benefit or harm the company — and whether these correlate with any executive branch trading.

| Signal | Interpretation |
|--------|---------------|
| President or senior official holds a significant position | Note as context — may indicate policy alignment or conflict of interest |
| Recent purchase before a positive policy announcement | Flag as potential conflict of interest; reference any ethics disclosures |
| No holdings or disclosures found | Neutral |

### What Not to Infer

- Congressional trading data **does not confirm insider information** — many trades are routine. Report the pattern; do not allege illegality.
- **Correlation is not causation.** A legislator buying a stock before good news may have used only public information.
- Always note data-unavailable gaps: non-US legislators and non-US listed companies are not covered by STOCK Act; note this limitation and mark as `data unavailable — not applicable` if the stock is non-US.

**Scoring guide:**

| Score | Criteria |
|-------|---------|
| 5 | No notable congressional/executive trading; or net buying by relevant committee members with no conflict concerns |
| 4 | Minor trading activity; mostly routine; no committee-relevant concern |
| 3 | Mixed — some cluster buying AND selling; limited relevance to oversight committees |
| 2 | Net selling by multiple legislators; or buying immediately preceding favorable legislation |
| 1 | Clear pattern of cluster selling before bad news; executive branch trading coincides with policy decisions; active ethics investigation |

---

## Red Flags — Composite Score

Score each sub-area (Compensation, Insider Trading, Conflicts, Litigation, News, Congressional & Presidential Trading) and average them, then **round to the nearest 0.5**, to produce the overall **Red Flags score out of 5**.

**Important:** A score of 1 in Litigation or Conflicts of Interest alone should cap the overall Red Flags score at 2, regardless of other sub-scores. A score of 1 in Congressional & Presidential Trading (clear conflict-of-interest pattern) also caps the overall score at 2.
