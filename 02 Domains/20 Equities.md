---
name: equities
description: Overlay for research on a public company as an investment — stock picking, valuation, thesis construction. Read alongside the protocol stages, not instead of them.
applies-to: "stocks, tickers, valuation, a company as an investment"
---

# 20 Equities

An overlay. The protocol still runs; this adds what equity work specifically requires.

## Framing

The output is **research, not advice.** It is a position on a business and what is priced into it — not a recommendation to buy, sell, or size anything. Say so in the deliverable. Position sizing, tax, and suitability are outside every brief here unless the user explicitly puts them in.

## Four questions people conflate

Answer them separately. Most bad equity research is a strong answer to one presented as an answer to all four.

1. **Is this a good business?** — economics, durability
2. **Is this a good price?** — what is priced in
3. **Is there a catalyst?** — what makes the gap close
4. **What is the timeframe?** — over which the thesis must hold

A great business at a demanding price and a mediocre business at a cheap one are different theses with different risks. Never let "good company" do the work of "good investment".

## Sources, in order

1. **Filings** — 10-K, 10-Q, 8-K, DEF 14A (proxy: compensation, ownership, related-party). Read the actual filing, not coverage of it. Footnotes and the risk factors that *changed year over year*.
2. **Earnings call transcripts** — especially the Q&A, and especially which analyst questions get non-answers.
3. **Official data** — regulator filings, industry statistics, government data.
4. **Everything else** — C-tier or below. Sell-side is D-tier: read for the numbers and the disclosed assumptions, never for the conclusion.

## Establish, in order

- **What it sells, to whom, and why they pay.** In plain language, without the company's vocabulary. If this cannot be written in three sentences, that is a finding.
- **Unit economics** — gross margin and its trend, contribution economics, what scales and what does not.
- **Capital allocation** — where cash has actually gone over five years: buybacks (and at what prices), dividends, M&A (and its returns), capex. This is management's revealed strategy, and it usually contradicts the strategy slide.
- **Share count trend** — dilution over five years. Growth per share is the only growth that reaches the owner.
- **Durability** — why does the advantage persist? Name the mechanism (switching costs, scale economics, network, regulation, brand). "Great product" is not a mechanism.
- **What is priced in** — reverse the multiple into the growth and margin the market appears to expect. Compare against history and against the disconfirming case.

## Mandatory: write the bear case first

Before forming a view, write the strongest bear case in full, from evidence you went looking for. This is not `14 Adversarial Review` — that comes later and attacks the finished thesis. This comes *before* the thesis exists, and it is what prevents the research from being a search for confirmation.

If the bear case is thin after a genuine search, that is a finding worth stating.

## Accounting red flags

Check each. Log the absence as well as the presence.

- Receivables or inventory growing faster than revenue
- Revenue recognition policy changed, or an unusual proportion recognised over time
- Persistent "one-time" adjustments; a widening GAAP-to-adjusted gap
- Capitalised costs that peers expense
- Auditor change, restatement, material weakness, late filing
- Related-party transactions in the proxy
- Insider selling patterns; unusual comp structure changes

## Freshness

The fastest-decaying research in this vault. Price, multiple, guidance, and estimates move in days. **Date-stamp every market-derived figure with the day.** Any deliverable states its as-of date prominently, and says that market-dependent conclusions expire.

Business facts decay slowly. Market facts decay in hours. Never let a fresh price sit next to a stale margin without labelling both.

## Base rates

Before accepting a growth or margin projection, ask what fraction of companies actually sustain that rate for that long. The base rates for sustained high growth, successful turnarounds, and accretive serial M&A are all much worse than any individual narrative suggests.

## Typical deliverable

A memo (`15 Deliverable`) plus a supporting sheet — comps, a simple reverse-DCF, or a segment build — via the **xlsx** skill. The sheet shows its assumptions as editable inputs, not hardcoded into formulas.
