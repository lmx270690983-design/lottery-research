# Lottery Research

DLT lottery statistical and physical randomness research project.

## Project Positioning

This repository is a research-grade project for historical lottery data analysis, randomness testing, physical-bias hypothesis evaluation, and blind-test validation.

It is **not** positioned as a guaranteed winning-number prediction system.

## Core Research Questions

1. Are historical DLT front-area numbers statistically consistent with uniform randomness?
2. Did earlier periods show stronger deviations than later periods?
3. Can ball-set metadata, draw order, position effects, or weather variables explain observed deviations?
4. Can any model improve out-of-sample probability scoring versus a uniform random baseline?
5. Are detected effects strong enough to have any practical betting value after lottery odds and payout structure?

## Repository Structure

```text
lottery-research/
├── data/
│   ├── raw/              # Raw source data. Large files should not be committed directly.
│   ├── processed/        # Cleaned datasets and derived tables.
│   └── external/         # Third-party or manually collected auxiliary data.
├── docs/
│   ├── methodology_lock.md
│   ├── blind_test_protocol.md
│   ├── research_summary.md
│   ├── rejected_hypotheses.md
│   └── data_dictionary.md
├── src/
│   ├── ingestion/        # Data collection and normalization.
│   ├── features/         # Feature construction.
│   ├── models/           # Statistical and probabilistic models.
│   ├── evaluation/       # Baselines, metrics, Monte Carlo tests.
│   └── visualization/    # Charts and report figures.
├── reports/
├── notebooks/
├── tests/
├── requirements.txt
└── README.md
```

## Methodological Rule

All future modeling work must separate:

- historical explanation;
- hypothesis discovery;
- model selection;
- final blind-test validation.

The final blind-test set must not be used for iterative tuning.

## Current Research Status

Preliminary findings from previous research notes:

- DLT front-area frequency distribution shows stronger deviation than SSQ.
- 2007-2014 appears more anomalous than later periods.
- Ball-set-level evidence from 2017-2025 does not show robust statistically significant per-ball bias.
- Some draw-order and weather-related signals were observed, but they remain weak and require strict blind validation.
- Most formula, machine-learning, association-rule, and sequence-memory hypotheses failed out-of-sample validation.

## Recommended Next Step

Implement the final blind-test experiment:

- Discovery set: 2007-2014
- Model-selection set: 2015-2021
- Final blind-test set: 2022-2026

The project should conclude honestly whether models are:

- consistently better than random;
- locally interesting but unstable;
- indistinguishable from random.
