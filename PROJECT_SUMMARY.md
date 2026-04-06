# Project Summary

## Objective

Build rule-based trading frameworks that combine macro context, intermarket confirmation, and technical execution across multiple asset classes.

## Research Approach

The research process followed a consistent structure:

1. Form a market hypothesis
2. Translate the idea into a rule set
3. Backtest the rules
4. Review winners and losers
5. Refine the filter logic
6. Separate public logic from private edge

## Public Framework Components

The public scripts in this repository use combinations of:

- Supertrend-based execution
- calendar spread confirmation
- nominal yield spread confirmation
- inflation spread confirmation
- real-yield bias filtering

## Asset Coverage

### NQ

Baseline trend-following implementation used as a simple benchmark.

### CL

Crude strategy built around the idea that the calendar spread contains useful physical-market information. The public version uses spread trend confirmation without exposing the private macro-state playbook.

### USDJPY

FX framework built on:
- price trend
- front-end rate differential
- inflation differential

### EURUSD

FX framework built on:
- price trend
- relative 2Y yield differential
- relative inflation differential

### Gold

Gold framework using real yields as a bias filter rather than as a fully symmetric trigger.

## Key Research Lessons

- Backtesting matters more than narrative confidence.
- Different assets need different filters.
- Spread confirmation can be more useful than raw price trend alone.
- Some market relationships are structural but still require selective use.
- Internal consistency is more important than theoretical perfection.

## Public vs Private Boundary

This summary describes the public architecture only.

Not included:
- private regime classification tables
- internal trade selection playbooks
- asset-specific decision matrices
- post-trade edge refinement rules

## Why This Exists

This repository is intended as a portfolio artifact demonstrating:

- systematic trading research
- signal design
- backtest-driven iteration
- Pine Script implementation
- disciplined separation between idea generation and edge preservation

## Relevance to Trading and Analytics Roles

This project demonstrates the ability to:

- turn qualitative market views into structured decision rules
- compare competing strategy ideas using evidence instead of narrative preference
- identify where edge is actually coming from
- build reusable tools for screening, confirmation, and execution logic
- communicate research clearly without disclosing sensitive implementation details
