# Blind Test Protocol

## Objective
Evaluate whether any model built on historical lottery data can outperform a uniform random baseline in truly unseen data.

## Data Split
- Training / Discovery: 2007–2014
- Validation / Model Selection: 2015–2021
- Blind Test: 2022–2026 (locked)

## Rules
- Blind test data must NOT be used for feature selection
- No iterative feedback from blind test results
- No manual adjustment based on outcomes

## Baseline
Uniform random sampling over:
- 1–35 (front area, 5 numbers)
- 1–12 (back area, 2 numbers)

## Metrics
- Log Loss
- Brier Score
- Top-k coverage (k=5,7,10,15)
- Expected Value (EV) simulation
- Yearly stability variance

## Output Requirement
Every model must output full probability distribution over all numbers, not just selected combinations.

## Success Criteria
A model is considered successful only if:
- It consistently outperforms baseline across all blind-test years
- Improvement is statistically significant under Monte Carlo validation
- Improvement is stable across time slices

Otherwise:
- Mark as non-predictive system
