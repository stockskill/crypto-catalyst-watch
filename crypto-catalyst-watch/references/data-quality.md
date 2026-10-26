# Data quality and interpretation

## Wallet attribution

Use a known owner label only when the source provides one. Preserve the transaction hash or explorer link when available. For a cluster without reliable attribution, report its behaviour, not its owner.

| Observed fact | Allowed interpretation | Do not claim |
|---|---|---|
| Transfer to a known exchange | potential sell-side liquidity | a completed sale |
| Withdrawal from an exchange or market maker | potential custody accumulation or settlement | a new purchase |
| Stable wallet balance | no observed transfer in the checked window | intent to hold |
| Exchange-to-exchange transfer | likely operational movement | directional market intent |

## Heatmaps and derivatives

Heatmap bands are estimates based on leverage and market-structure models. Report them as `estimated long/short liquidation zone`, never as support, resistance, or a price target. Recheck their retrieval time because they can change rapidly.

Use a numerical funding, OI, basis, or liquidation statistic only when it is visible with an observation time. If a dashboard exposes the metric name but not its current value, write `not independently verifiable`.

## Minimum evidence for a directional signal

Require one material catalyst plus confirmation from a second independent layer. Examples:

- positive ETF flow plus constructive macro reaction;
- successful upgrade plus improving network activity;
- negative unlock/financing pressure plus exchange inflow or weakening price structure.

One-off transfers, unverified social posts, and a single heatmap cluster cannot satisfy the rule.
