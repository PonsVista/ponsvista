<p align="center">
  <img src="assets/ponsvista-mark.png" alt="PonsVista" width="88" />
</p>

<h1 align="center">PonsVista</h1>

<p align="center">Token discovery and market analytics for the Pons ecosystem on Robinhood Chain.</p>

<p align="center">
  <a href="https://ponsvista.xyz/">Website</a> ·
  <a href="https://x.com/ponsvista">X</a> ·
  <a href="docs/screener.md">Screener guide</a> ·
  <a href="docs/data-notes.md">Data notes</a>
</p>

## Overview

PonsVista brings Pons token discovery and market information into one interface. Explore different views of the ecosystem, search for a token, and inspect the available price, volume, liquidity and activity information.

This repository contains public project documentation and brand assets. It does not contain the application server, deployment configuration or transaction execution code.

## Explore the Screener

| View | What it shows |
| --- | --- |
| [Top](https://ponsvista.xyz/) | Pons tokens ranked by circulating market cap. |
| [Volume](https://ponsvista.xyz/volume) | Tokens ranked by reported 24-hour trading volume. |
| [New](https://ponsvista.xyz/new) | Recent launches, with the newest entries first. |
| [Active](https://ponsvista.xyz/active) | An activity-focused view of recently traded Pons tokens. |
| [Gainers](https://ponsvista.xyz/gainers) | Supported price changes since the first indexed trade, with the quote currency shown. |
| [Near graduation](https://ponsvista.xyz/near-graduation) | Curve-stage tokens organized around reported curve progress. |
| [Graduated](https://ponsvista.xyz/graduated) | Tokens reported as graduated by the available launch data. |

Search and quote-pair filters help narrow the available list. ETH, USDG and other supported quote assets appear in the product's filters. Token identity is based on its contract address; a matching name or ticker alone does not establish that two entries are the same token.

## Read the data in context

The time window, currency and source matter when comparing tokens. A lifetime total is different from a 24-hour total, and a single pool may cover only part of a token's activity.

Market data can be delayed or incomplete. A missing observation is not automatically zero. Source updates, indexed history and coverage can differ across tokens and views.

See [Data notes](docs/data-notes.md) for metric definitions and [Screener guide](docs/screener.md) for the category overview.

## Repository contents

- `assets/` - PonsVista logo assets.
- `docs/` - Screener documentation, metric notes and project profile text.
- `.github/ISSUE_TEMPLATE/` - A template for documentation and display reports.
- `CONTRIBUTING.md` - How to suggest a documentation correction.

## Project links

- Website: [ponsvista.xyz](https://ponsvista.xyz/)
- X: [@ponsvista](https://x.com/ponsvista)

Documentation prepared on 25 November 2026 from the available V31 project materials. The hosted product may change independently of this repository.
