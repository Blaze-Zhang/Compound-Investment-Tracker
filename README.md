# Compound — Investment Tracker

A personal finance OS built for long-term, rules-based investing. No backend, no accounts, no ads. Just a single HTML file that runs entirely in your browser.

---

## What it does

**① Cash Flow** — Map your monthly income from living expenses → rigid goals → investable capital. Customize how your disposable income splits across investing, saving, and spending.

**② Monthly Allocation** — Distribute your investment budget across crypto and US stocks by fixed ratios. Built-in cold wallet transfer alert (triggers at 2,000 USDT). Save a monthly record with one click.

**③ Rebalance** — Annual rebalance checker. Set target allocations, input current market values, and the tool tells you exactly what to sell and what to buy with the proceeds. Triggers at ≥5% deviation.

**④ Dream Jars** — Goal-based savings buckets, isolated from your investment accounts. Auto-distributes your monthly savings budget across jars by ratio. Tracks progress toward each goal.

**⑤ Record Book** — Unified transaction log for all assets (stocks + crypto). Calculates moving average cost automatically. Filter by asset or by time period. Import records directly from a JSON file.

**⑥ Summary** — Monthly snapshot: cash flow breakdown, investment allocation, transactions recorded, and rigid goal checklist — all in one view.

---

## Key features

- **100% local** — all data stored in your browser's localStorage, nothing sent to any server
- **Single HTML file** — download and open, or use the live link below
- **Import / Export** — back up and restore all your data as a JSON file
- **Order screenshot → JSON import** — paste your IBKR or OKX order screenshot into Claude, get a JSON file back, import directly into Record Book
- **No dependencies** — no npm, no build step, no login

---

## Live

🔗 [Open Compound](https://blaze-zhang.github.io/Compound-Investment-Tracker/))

---

## How to use

**Option A — Use online**
Click the live link above. Works on desktop and mobile.

**Option B — Run locally**
1. Download `index.html`
2. Open it in any browser
3. Your data stays on your device

**Option C — Self-host**
Fork this repo, enable GitHub Pages, done.

---

## Importing order screenshots

This tool works well with Claude (claude.ai):

1. Take a screenshot of your IBKR or OKX order confirmation
2. Send it to Claude with the message from your system prompt
3. Claude returns a `.json` file
4. In Record Book → click **📂 Import JSON**
5. Done — auto-deduplication handles repeats

---

## Data & privacy

All data is stored in `localStorage` in your own browser. No data is ever transmitted anywhere. Each person who uses this tool has completely separate, isolated data.

Exporting your data produces a single `.json` file you can back up anywhere.

---

## Philosophy

> Buy good businesses at fair prices. Let time and compounding do the work.

This tool is built around a specific set of rules:
- Fixed monthly investment ratios, never adjusted for market conditions
- Crypto: 70% BTC/ETH, 30% stablecoin cash position
- US Stocks: VOO / QQQ / SMH / SGOV at fixed weights
- Annual rebalance only, triggered by ≥5% deviation
- Cold wallet transfer when exchange balance ≥ 2,000 USDT

You don't have to follow these rules — all ratios and assets are fully customizable.

---

## License

MIT — free to use, fork, and modify.
