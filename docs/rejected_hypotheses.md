# Rejected Hypotheses Log

This document tracks hypotheses that failed out-of-sample validation.

## 1. Deterministic Formula Hypothesis
- Claim: Lottery numbers follow hidden deterministic formula
- Result: Failed (random baseline not exceeded)

## 2. Machine Learning Predictability
- Models: RF, KNN, Logistic Regression
- Result: Overfitting on training data, no generalization

## 3. Association Rule Mining
- Claim: Certain number combinations co-occur
- Result: False positives due to combinatorial explosion

## 4. Sequence Memory Effect
- Claim: Long-term dependencies exist between draws
- Result: DFA alpha ≈ 0.5 (random walk)

## 5. Weather Strong Causality
- Claim: Weather strongly affects number selection
- Result: Only weak, non-robust signals (e.g., Rain × 31)

## 6. Ball Weight Large Bias Hypothesis
- Claim: Strong physical bias (~7%) exists per ball
- Result: Not supported by 2017–2025 data

## Conclusion
All tested predictive hypotheses failed to demonstrate stable out-of-sample predictive power.
