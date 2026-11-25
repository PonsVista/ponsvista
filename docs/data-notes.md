# Data notes

These notes explain how to read the public analytics views. They describe the available V31 project materials; they are not a live health report or a guarantee of complete coverage.

## Metrics and scope

| Label | Interpretation |
| --- | --- |
| Price | The latest usable price observation available to the source, in the displayed currency. |
| Circulating market cap | A market-cap observation based on circulating supply. It should not be substituted with total-supply valuation without a label. |
| Age | Time since the recorded launch timestamp, when that timestamp is available. |
| Volume (24h) | Reported or supported volume for the 24-hour window, subject to source coverage and currency. |
| Volume (total) | An available lifetime volume total. It is separate from daily volume. |
| Volume (source) | A source-reported value whose time window may not be labeled. It should not silently become a daily or lifetime total. |
| Trades | An available trade count. Read its scope and period; a lifetime count is not a 24-hour count. |
| Liquidity | The liquidity observation supplied for a supported market or pool. It is not trading volume. |
| 5m / 1h / 6h / 24h | Price changes over the labeled window, where supported observations exist. |
| Since first indexed trade | A historical price-change measure with a supported indexed baseline, using the stated quote currency. |
| Curve progress | A launch-curve state observation. A genuine zero or fractional percentage can be valid. |
| Stage | A launch-state label from the available launch or contract data. |

## Updates and freshness

The available implementation combines public Pons Family information with Robinhood Chain RPC observations. Optional providers can enrich the available data. Source requests, indexing and browser delivery are distinct steps, so an interface refresh does not establish that every upstream value is new.

The implementation uses polling and streamed interface updates. It should not be described as guaranteed tick-by-tick data. A source can be active while historical indexing or supplementary metrics remain incomplete.

When a source is unavailable, the last usable observation may remain visible with its original date or stale status. Receiving an old response again does not make its underlying observation fresh.

## Missing data and zero

- A measured zero is a valid value and should remain zero.
- An unavailable observation should remain unavailable, rather than becoming an invented zero.
- A chart with insufficient coverage should not be used to manufacture a daily total.
- Historical change requires a supported baseline; a 24-hour change is not a replacement for a lifetime change.

## Currency and pool coverage

USD amounts and quote-asset amounts are different units. Keep the displayed unit when comparing observations. A value marked as pool-scoped describes one indexed pool and may not represent all activity for that token.

## Identity and ranking

Contract addresses identify tokens. Names, symbols and similar logos can occur on more than one contract. Board order, pair filters, missing metrics and the available indexed subset can all affect the entries visible in a category.

## Historical visuals

A static screenshot or promotional image is a snapshot. Its token order, age badges and numbers should not be treated as a current feed after capture.
