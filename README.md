# Sweden's grid batteries

A one-page site showing official statistics on grid-connected battery storage in Sweden for 2024 and 2025.

**Live site:** https://andreasn.github.io/sweden-battery-storage/

## Data

The data comes from table TAB6631, *Grid connected batteries by storage capacity*. Statistics Sweden (SCB) publishes it for the Swedish Energy Agency, and it was last updated on 8 October 2026.

- [Open the table at Statistics Sweden](https://www.statistikdatabasen.scb.se/goto/en/ssd/Batterier)
- [`data/scb-tab6631.csv`](data/scb-tab6631.csv) is a copy of the official figures used on the page.
- [`data/yearly.csv`](data/yearly.csv) is the year-by-year table. It combines the official 2024–2025 figures with industry estimates for 2023 and 2026, which are flagged and sourced on the page.

Statistics Sweden notes that the figures are likely underreported.

## Updating

The figures are also embedded in `index.html`, in the `<script id="data">` block. When SCB publishes a new year, update both that block and the CSV.
