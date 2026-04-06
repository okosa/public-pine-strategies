# Public Pine Strategies

Public Pine Script strategy bundle demonstrating systematic trading research across index futures, FX, crude oil, and gold. The repository is intended as a portfolio artifact showing how market ideas can be translated into structured rule sets, tested, refined, and packaged into reusable tools.

## Included Scripts

- `NQ_Supertrend.pine`
- `CL_Spread_Supertrend_Filter.pine`
- `USDJPY_2Y_Inflation_Filters.pine`
- `EURUSD_2Y_Inflation_Filters.pine`
- `Gold_Real_Yield_Bias_Filter.pine`

## What This Repo Shows

- Rule-based strategy design in Pine Script
- Use of spread confirmation and intermarket filters
- Asset-specific logic instead of one generic model
- Research structure that separates trigger, filter, and exit logic

## Skills Demonstrated

- systematic strategy research
- hypothesis testing through backtesting
- signal design using spreads, yields, inflation, and price
- asset-specific framework design
- post-trade review and iterative refinement
- Pine Script implementation for trading logic
- clear separation between public research artifacts and private edge

## Public vs Private Logic

These scripts are the public-facing versions of the research.

Included here:
- execution logic
- spread-based confirmation logic
- yield and inflation filter logic

Intentionally excluded:
- manual macro-regime gating tables
- trade review decision matrices
- private asset playbooks
- internal filtering rules derived from post-trade analysis

In other words, this repo shows the framework architecture without exposing the full discretionary/systematic edge layer.

## Script Notes

### `NQ_Supertrend.pine`

Baseline trend-following implementation for NQ.

### `CL_Spread_Supertrend_Filter.pine`

Crude oil strategy using a calendar spread confirmation layer based on `CL1! - CL2!`.

### `USDJPY_2Y_Inflation_Filters.pine`

USDJPY strategy combining:
- price trend
- `US02Y - JP02Y`
- `USIRYY - JPIRYY`

### `EURUSD_2Y_Inflation_Filters.pine`

EURUSD strategy combining:
- price trend
- `EU02Y - US02Y`
- `EUIRYY - USIRYY`

### `Gold_Real_Yield_Bias_Filter.pine`

Gold strategy using real yields as a directional bias filter with price as the execution trigger.

## Portfolio Summary

A one-page summary of the project is available in [PROJECT_SUMMARY.md](PROJECT_SUMMARY.md).

## Results Framing

The scripts in this repository are public-safe research versions. Some produced encouraging historical results in testing, but the goal of the repository is to demonstrate research process, strategy design, and implementation discipline rather than publish a complete production-ready trading stack.

## Disclaimer

These scripts are research artifacts and educational portfolio material. They are not investment advice, production trading systems, or a complete representation of the private research process behind the full framework.
