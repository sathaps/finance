# Finance Tools

Free, browser-only calculators for investors who use margin and options. Every tool is a single static HTML file: no build step, no backend, and nothing you enter leaves your browser.

## Tools

| Tool | What it answers |
|---|---|
| [Margin Cushion Calculator](margin-calculator/) | How far can my portfolio fall, market-wide or one stock at a time, before excess liquidity hits zero and the broker can auto-liquidate? |

Planned: PMCC income calculator, and a cost calculator for buying gold abroad vs. in India.

## How the margin math works

- **Equity** = market value − margin loan
- **Maintenance requirement** = Σ (position value × maintenance %)
- **Excess liquidity** = equity − maintenance requirement
- **Market-wide drop to liquidation** = 1 − loan ÷ (market value − requirement)
- **Single-stock drop to liquidation** = excess liquidity ÷ (position value × (1 − maintenance %))

Real brokers are stricter: IBKR checks margin in real time, can raise maintenance rates on volatile or concentrated positions, and generally liquidates without a grace period. Treat the result as a best case.

## Run locally

Open `margin-calculator/index.html` in any browser. That's it.

## Disclaimer

For education only. This is not financial advice.

## License

MIT
