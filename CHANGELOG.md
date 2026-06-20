# Changelog

All notable changes to this project will be documented in this file.  
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

---

## [Unreleased]

---

## [1.0.0] — 2024

### Added
- 4 fully configurable market sessions: London, New York, Tokyo, Sydney
- 4 fully configurable ICT kill zones: Asian KZ, London KZ, NY AM KZ, NY PM KZ
- Box display styles: Box, Background, Hamburger, Sandwich
- Opening range highlight with R1/R2/S1/S2 target levels (based on historical average range)
- Fibonacci retracement levels (0.382, 0.500, 0.628) per session
- Session-wide candle rendering — OHLC or OC mode
- Bar colouring per session and kill zone (bull/bear colours configurable separately)
- Session labels with optional name, day of week, price range, and pips
- Open/close dot markers with directional fill between them
- Range information table (top-right) — live vs. average range, colour-coded
- Opening range hit-rate statistics table (bottom-right)
- Alerts: session start/end, opening range breakout, H/L cross after session close
- Timezone support: GMT-11 through GMT+12
- History period control
- Pine Script v6 — full OOP type system (`Session`, `OHLC`, `OpeningRange`, `State`, `Candle`, `Dot`)
