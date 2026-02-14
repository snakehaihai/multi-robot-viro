# EPDOP Screening Algorithm

## 📐 Concept

EPDOP (Estimated Position Dilution of Precision) is a geometric quality metric used to assess the quality of positioning measurements based on the spatial configuration of measurement sources.

## 🎯 Key Features

- **Adaptive Threshold**: Dynamically adjusts based on measurement availability
- **Geometric Quality**: Evaluates measurement geometry for optimal estimation
- **Outlier Rejection**: Screens out poorly conditioned measurements

## 🔢 Mathematical Background

Details will be provided in the full paper (TIM, under review).

## ⚙️ Parameters

- `epdop.threshold`: Base EPDOP threshold value
- `epdop.min_satellites`: Minimum number of required measurements
- `epdop.adaptive`: Enable/disable adaptive threshold

## 📊 Performance

Performance evaluations and benchmarks will be released with the full implementation.
