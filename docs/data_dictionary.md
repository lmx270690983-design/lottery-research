# Data Dictionary

## Lottery Draw Record

### Core Fields
- draw_id: unique identifier
- date: draw date
- front_numbers: list[int] (5 numbers, 1–35)
- back_numbers: list[int] (2 numbers, 1–12)

## Physical Metadata
- ball_set_id: int (e.g., BS1, BS2, BS3)
- draw_order: list[int] (actual sequence of drawn balls)
- position_features:
  - position_i_number

## Environmental Features
- temperature: float
- humidity: float
- pressure: float
- wind_speed: float
- rain_flag: bool

## Derived Features
- frequency_window_n
- rolling_mean
- z_score_per_number
- bayesian_posterior_weight

## Notes
All feature engineering must avoid leakage from future draws.
