# Crypto Catalyst Watch

English below · Magyar leírás lentebb

## English

`crypto-catalyst-watch` is a Codex skill for evidence-led, short-horizon crypto-market research. It follows a focused core universe:

- Bitcoin (BTC)
- Ethereum (ETH)
- Solana (SOL)

### What it produces

1. A compact **Catalyst Card** for a fast market view.
2. A linked **Deep Scan** with the evidence behind the signal.
3. A weekly or monthly multi-asset roundup when requested.

The analysis checks current prices, macro events, ETF and institutional flows, exchange flows, large-wallet activity, funding, open interest, liquidation heatmaps, network events, token supply, and regulation.

### Data integrity rules

- A wallet transfer is never automatically called a buy or sell.
- Wallet ownership is named only when a reliable source labels it.
- Liquidation heatmaps are treated as modelled risk zones, not targets or guaranteed orders.
- Funding, open interest, and similar metrics must have a visible current value and timestamp; otherwise the skill marks them as unavailable.
- A BUY, NEUTRAL, or SELL label is an informational research signal, not personalized investment advice or an execution instruction.

### Structure

```text
crypto-catalyst-watch/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── asset-universe.md
    ├── catalyst-rubric.md
    └── data-quality.md
```

Use the skill with a request such as:

> Use $crypto-catalyst-watch to run a current BTC, ETH, and SOL Catalyst Card with a Deep Scan.

## Magyar

A `crypto-catalyst-watch` egy Codex skill bizonyíték-alapú, rövid távú kriptopiaci kutatáshoz. A célzott alapuniverzum:

- Bitcoin (BTC)
- Ethereum (ETH)
- Solana (SOL)

### Kimenetek

1. Rövid **Catalyst Card** a gyors piaci képhez.
2. Kattintható **Deep Scan**, amely a jelzés mögötti részletes bizonyítékokat tartalmazza.
3. Igény szerint heti vagy havi, több eszközt összevető összefoglaló.

A skill az aktuális árak mellett figyeli a makrót, ETF- és intézményi flow-t, tőzsdei be-/kiáramlást, nagy walletmozgásokat, fundingot, open interestet, likvidációs heatmapet, hálózati eseményeket, tokenkínálatot és szabályozást.

### Adatminőségi szabályok

- Egy wallet-tranzakció önmagában nem „vétel” vagy „eladás”.
- Wallet-tulajdonost csak megbízható címkézés esetén nevez meg.
- A likvidációs heatmap modellezett kockázati zóna, nem célár vagy garantált megbízás.
- Funding, open interest és hasonló adat csak látható aktuális értékkel és időbélyeggel szerepelhet; különben a skill hiányzóként jelöli.
- A BUY, NEUTRAL vagy SELL címke tájékoztató kutatási jelzés, nem személyre szabott befektetési tanács és nem automatikus megbízás.

### Használat

Például:

> Használd a $crypto-catalyst-watch skillt egy aktuális BTC–ETH–SOL Catalyst Card és Deep Scan elkészítéséhez.

## License

Released under the [MIT License](LICENSE).
