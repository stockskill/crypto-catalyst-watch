---
name: crypto-catalyst-watch
description: Research current crypto-market catalysts for Bitcoin (BTC), Ethereum (ETH), and Solana (SOL). Use for a short Catalyst Card, a linked Deep Scan, a weekly/monthly crypto roundup, or an evidence-led buy/neutral/sell research signal. Verify current prices, macro, ETF flows, on-chain whale activity, derivatives, liquidation heatmaps, network events, token supply, and regulation; distinguish observed facts from inference.
---

# Crypto Catalyst Watch

Create evidence-led research for the BTC–ETH–SOL core universe. Output a research signal, not an order, position size, leverage recommendation, or personalized investment advice.

## Read first

Read [references/asset-universe.md](references/asset-universe.md) and [references/data-quality.md](references/data-quality.md) for every request. Read [references/catalyst-rubric.md](references/catalyst-rubric.md) before assigning a signal or writing a weekly/monthly summary.

## Workflow

1. Establish the horizon: intraday/event, 1–4 weeks, or weekly/monthly. Default to 1–4 weeks.
2. Get a timestamped BTC, ETH, and SOL price snapshot. Do not imply stale or closed-market data is live.
3. Check primary public sources first: central banks and macro releases, regulators, ETF issuers/filings, protocol foundations, client teams, and exchange status pages. Use market-data providers and reputable reporting only for context or data unavailable from a primary source.
4. Compare the new information with the prior expectation. A headline is material only if it can change liquidity, demand, supply, execution, regulatory access, or a stated network milestone.
5. Run the Deep Scan quality gates: wallet attribution, exchange flow, ETF flow, derivatives, heatmap, token supply, network/security, and macro. Mark a field unavailable rather than inventing a number.
6. Cite every material current fact near the claim. Label interpretation as inference.

## Wallet and heatmap rules

- Name a wallet owner only when a reliable source labels it. Otherwise use `unattributed address/cluster`.
- A transfer to an exchange is **potential** sell-side liquidity, not proof of a sale. A withdrawal is **potential** custody accumulation, not proof of a purchase. An unchanged balance is not proof of a holder's intent.
- For every wallet item, state chain, amount, destination/source category, observation time, attribution quality, and the narrowest justified interpretation.
- Treat liquidation heatmaps as modelled zones, not guaranteed orders or targets. State the provider, retrieval time, direction, distance from spot, and estimated size if available.
- Never derive a buy/sell signal from a single wallet transfer or a single heatmap band.

## Research-signal rules

- **BUY research signal:** verified improvement in expectations, a near-term catalyst, no material unaddressed supply/liquidity or execution red flag, and confirmation from more than one relevant data layer.
- **NEUTRAL / WATCH:** evidence is mixed, a major event is pending, or a required data layer is unavailable.
- **SELL research signal:** verified deterioration in expectations, material supply/unlock or liquidity pressure, a failed milestone, regulatory loss, or a confirmed risk-off deterioration.

Do not force a label. If current funding, open interest, heatmap, or wallet attribution cannot be verified, report the gap and use NEUTRAL / WATCH unless other evidence is decisive.

## Output: Card first, Deep Scan second

Start with the short card. Then add this link before the detailed section:

```markdown
[Részletes Deep Scan](#deep-scan)
```

Use a `## Deep Scan` heading immediately below the short card so GitHub Markdown renders the anchor. In chat surfaces where anchor links are unsupported, place the Deep Scan directly below the card.

### Catalyst Card

```markdown
## Crypto Catalyst Card — BTC / ETH / SOL

**As of:** [date, timezone]
**Horizon:** [event / 1–4 weeks / weekly]
**Research status:** BUY / NEUTRAL / SELL

| Asset | Price | 24h change | Relative state |
|---|---:|---:|---|
| BTC | | | |
| ETH | | | |
| SOL | | | |

**What changed**
- [verified catalyst]

**Why it matters now**
- [expectation change]

**Bull / bear condition**
- Bull: [specific confirmation]
- Bear: [specific invalidation]
```

## Deep Scan

Cover only material findings, but explicitly mark unavailable data:

1. Price structure and relative strength
2. Macro and risk regime
3. ETF and institutional flow
4. On-chain exchange flow and labelled/unattributed whale activity
5. Funding, open interest, basis, liquidations, and options when verifiable
6. Liquidation heatmap: largest and nearest zones above/below spot
7. Network, protocol, security, governance, and token-supply checks
8. Synthesis: bull case, bear case, invalidation, and next decisive event

For weekly/monthly output, lead with one table across BTC, ETH, and SOL. Include only data that changed the thesis; write `No material update` when appropriate.
