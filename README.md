# Sessions and Killzones

> A TradingView Pine Script v6 indicator by [Sagar](https://github.com/Sagar4575)

Visualises the four major FX market sessions and four ICT kill zones as coloured range boxes directly on your chart. Each session and kill zone is fully configurable — times, timezone, colours, box style, opening range, Fibonacci levels, bar colouring, candles, labels, and more.

---

## Features

### Sessions (4 × configurable)
| # | Default Name | Default Time (GMT+0) | Colour |
|---|---|---|---|
| 1 | London | 08:00 – 17:00 | `#66D9EF` Cyan |
| 2 | New York | 13:00 – 22:00 | `#FD971F` Orange |
| 3 | Tokyo | 00:00 – 09:00 | `#AE81FF` Purple |
| 4 | Sydney | 20:00 – 05:00 | `#FB71A3` Pink |

### Kill Zones (4 × configurable)
| # | Default Name | Default Time (GMT+0) | Colour |
|---|---|---|---|
| 1 | Asian KZ | 20:00 – 00:00 | `#00BCD4` Teal |
| 2 | London KZ | 02:00 – 05:00 | `#8BC34A` Green |
| 3 | NY AM KZ | 08:30 – 11:00 | `#FFC107` Amber |
| 4 | NY PM KZ | 13:30 – 16:00 | `#E91E63` Pink |

### Per-session / kill zone options
- **Box styles** — Box, Background, Hamburger (H/L lines only), Sandwich (vertical lines)
- **Opening Range** — Highlights the H/L of the first N minutes with optional R1/R2/S1/S2 target levels, derived from the session's historical average range
- **Fibonacci levels** — 0.382, 0.500, and 0.628 retracements drawn within each session range
- **Session candle** — A single OHLC or OC candle rendered across the full session width
- **Bar colouring** — Colours chart bars while inside a session or kill zone
- **Labels** — Session name, day of week, price range, and pips
- **Dots** — Open/close markers with a directional fill between them
- **Extend** — Optionally extend lines to the right beyond the session close

### Global features
- **Range table** (top-right) — Live current range vs. N-period average per session, colour-coded green/orange/red
- **Opening range stats table** (bottom-right) — Historical hit rates for R1, S1, R2, S2 targets
- **Alerts** — Session start/end · Opening range breakout · Price crossing a closed session's H/L

---

## Installation

1. Open [TradingView](https://www.tradingview.com) and go to the Pine Script editor (bottom panel).
2. Delete the default script and paste the full contents of [`fx_market_sessions_with_killzones.pine`](fx_market_sessions_with_killzones.pine).
3. Click **Add to chart**.

> **Note:** This script uses two TradingView published libraries (`boitoki/AwesomeColor` and `boitoki/Utilities`) which are resolved automatically at compile time — no extra steps needed.

---

## Configuration

All settings are in the indicator's **Settings panel** (⚙ icon on the chart).

| Group | Key settings |
|---|---|
| `GENERAL` | Timezone (GMT-11 → GMT+12), history lookback |
| `SESSION 1–4` | Show/hide, label, colour, time range, extend, opening range, Fibonacci, bar style |
| `KILL ZONE 1–4` | Same options as sessions |
| `BOX` | Style (Box/Background/Hamburger/Sandwich), border style/width, background, dots, end offset |
| `LABELS` | Show/hide, size, position (top/bottom · inside/outside), content (name, day, price, pips) |
| `OPENING RANGE` | Period (minutes), label size/colour/text, current-session only, breakout flag, target lines/boxes, stats table |
| `CANDLE` | Show/hide, OHLC or OC mode, border width, colour mode |
| `FIBONACCI LEVELS` | Show/hide, line style, line width |
| `INFORMATION` | Show/hide table, size, value type (price/pips), averaging period |
| `ALERTS VISUALISED` | Toggle visual markers for each alert type |

---

---

## License

[Mozilla Public License 2.0](LICENSE) — © 2024 [Sagar](https://github.com/Sagar4575)
