# Methodology Lock

## Principle
Once the blind-test protocol is defined, it MUST NOT be modified based on test results.

## Forbidden Actions
- No tuning based on final test set outcomes
- No adding new features after seeing blind-test performance
- No selective reporting of favorable results

## Allowed Actions
- Fixing data bugs unrelated to outcomes
- Improving code efficiency without changing logic
- Reproducing results for validation

## Experiment Separation
1. Discovery Phase (2007-2014)
2. Model Selection Phase (2015-2021)
3. Blind Test Phase (2022-2026)

## Rule
Any model that does not outperform random baseline in blind test must be marked as failed, regardless of historical interpretability.
