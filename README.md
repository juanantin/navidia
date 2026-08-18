# Na'vidia — $NAVIDIA

Single-page landing site for the Na'vidia memecoin (Base chain).

## Setup before launch

1. **Background image** — drop the hero artwork in as `assets/hero-bg.jpg` (referenced in `index.html`'s `.hero` background). Until then, a dark blue placeholder gradient is shown.
2. **Contract address** — edit `CONTRACT_ADDRESS` near the bottom of `index.html` (in the `<script>` block) once $NAVIDIA is deployed on Base. This value drives:
   - the header "CA" copy button
   - the "Chart" link (Dexscreener)
   - the "BUY $NAVIDIA" button (Uniswap on Base)
3. **Dashboard numbers** — the six stat cards (fees collected, $NVIDIA distributed, holders, market cap, liquidity, 24h volume) are currently static placeholder values matching the mockup. Wire them to a live data source (subgraph/API) by updating the `#feesValue`, `#nvidiaValue`, `#nvidiaUsdValue`, `#holdersValue`, `#mcapValue`, `#liquidityValue`, and `#volumeValue` elements.

## Run locally

Just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```
