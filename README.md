<div align="center">
  <img src="public/genlayer-spinner.svg" alt="GenLayer Spinner" width="96" />
  <h1 align="center">GenLayer Spinner</h1>
  <p align="center">
    Consensus in Motion — a branded animated loading indicator built from the three geometric pieces of the <strong>GenLayer</strong> mark.
  </p>
  <p align="center">
    <a href="https://raw.githubusercontent.com/Misagh95/genlayer-spinner/master/public/genlayer-spinner.svg" target="_blank"><strong>▶ View Live</strong></a>
    ·
    <a href="demo.html" target="_blank"><strong>🎬 Demo Page</strong></a>
  </p>
</div>

---

## Concept

The opposing wings of the GenLayer mark trade emphasis while moving toward the center, representing independent validators converging on consensus. The complete mark rotates on a constant linear loop so the first and last frames join without a jump.

## Deliverables

| File | Purpose |
|---|---|
| [`public/genlayer-spinner.svg`](public/genlayer-spinner.svg) | Standalone animated SVG — no JS, fonts, libraries, or external assets |
| [`src/components/GenLayerSpinner.tsx`](src/components/GenLayerSpinner.tsx) | Reusable React component (`size`, `color`, `animated`, `label`) |
| [`src/components/styles.css`](src/components/styles.css) | CSS animations, glow, reduced-motion rules |

Both versions honor `prefers-reduced-motion` and display the complete static GenLayer mark when animation is disabled.

## Usage

Plain HTML:

```html
<img src="/genlayer-spinner.svg" width="32" height="32" alt="Loading" />
```

React:

```tsx
<GenLayerSpinner size={32} color="#110fff" label="Loading markets" />
```

## Treats

- Transparent background, scales to any size, remains recognizable at 16px.
- Electric GenLayer blue (`#110fff`) tuned for visibility on light and dark surfaces.
- Dark mode variant in the standalone SVG via `prefers-color-scheme`.

## Integration

This spinner is production of the **DGDreams — Web3 Space Terminal** at **[dgdreams.space](https://dgdreams.space)** — a multi-chain daily task dashboard across 14 networks with GenLayer AI contracts (Bradbury testnet) and soulbound NFT streaks. It is used as the branded loading state across the GenLayer hub, oracle, market, and escrow pages, and as the GenLayer mark in the dashboard UI and documentation.

- Live site: <https://dgdreams.space>
- Dashboard repository: <https://github.com/Misagh95/dgdreams>
- Spinner page in the site: <https://dgdreams.space/genlayer>

---

Built by [@Misagh95](https://github.com/Misagh95) for the GenLayer ecosystem.