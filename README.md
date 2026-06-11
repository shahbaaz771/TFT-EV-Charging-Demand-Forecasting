# Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting

[![Conference](https://img.shields.io/badge/Conference-SMiLE%202025-blue)](https://smileconf.com/en)

[![Paper](https://img.shields.io/badge/Paper-ScienceDirect-orange)](https://www.sciencedirect.com/science/article/pii/S2352146526003285)



---

## Overview

This repository accompanies the research paper:

**Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting**

Published in **Transportation Research Procedia (Elsevier)** and presented at the **2nd International Conference on Smart Mobility and Logistics Ecosystems (SMiLE 2025/2026), KFUPM, Saudi Arabia.**

The work proposes an interpretable Temporal Fusion Transformer (TFT) framework for multi-horizon forecasting of electric vehicle charging station occupancy rates using temporal, spatial, and contextual information.

---

## Authors

* El-Sayed M. El-Alfy
* Shahbaaz A. Sadiq
* Mohammed Ayub
* M. Faisal Nurnoby

King Fahd University of Petroleum and Minerals (KFUPM), Saudi Arabia

---

## Abstract

Traditional forecasting approaches face challenges in accurately modeling the highly dynamic characteristics of electric vehicle charging demand. This work presents a Temporal Fusion Transformer (TFT)-based framework for short-term multi-horizon forecasting of charging station occupancy rates.

The framework combines:

* Static station metadata
* Historical charging behavior
* Calendar-based temporal information
* Spatial neighborhood information

Experimental evaluation on the ST-EVCDP dataset demonstrates strong predictive performance, achieving:

| Metric | Value  |
| ------ | ------ |
| MAE    | 0.0064 |
| RMSE   | 0.0098 |
| MAPE   | 4.24%  |
| R²     | 0.9588 |

The TFT model also provides interpretability through variable selection networks and temporal attention mechanisms.

---

## Research Contributions

The main contributions of this work are:

1. A Temporal Fusion Transformer framework tailored for EV charging demand forecasting.
2. Integration of static, temporal, and spatial features within a unified forecasting architecture.
3. Multi-horizon occupancy forecasting at station level.
4. Attention-based interpretability for understanding influential forecasting factors.
5. Comprehensive evaluation using real-world EV charging data.

---

## Dataset

The experiments utilize the **ST-EVCDP (Spatio-Temporal Electric Vehicle Charging Demand Prediction)** dataset collected from Shenzhen, China.

Dataset characteristics:

* 247 charging stations
* 18,061 public charging piles
* 5-minute temporal resolution
* 30-day observation period

Target variable:

* Charging station occupancy rate

---

## Methodology

The proposed framework leverages the Temporal Fusion Transformer (TFT) architecture and incorporates:

### Static Features

* Station capacity
* Geographic location
* Network topology characteristics

### Known Future Features

* Hour of day
* Day of week
* Weekend indicators
* Pricing information

### Historical Features

* Occupancy history
* Charging volume
* Charging duration
* Neighbor station statistics

### TFT Components

* Variable Selection Networks
* Gated Residual Networks
* LSTM Encoder-Decoder
* Multi-Head Attention
* Quantile Forecasting Layer

---

## Results

Average performance across nine representative charging stations:

| Metric | Value  |
| ------ | ------ |
| MAE    | 0.0064 |
| RMSE   | 0.0098 |
| MAPE   | 4.24%  |
| R²     | 0.9588 |

The TFT model consistently outperformed baseline approaches including:

* Naive Persistence Forecasting
* Moving Average
* ARIMA/SARIMAX

---

## Code Availability

The implementation used in this study is not publicly released at this time.

This repository is intended to provide access to the published research article, methodology, experimental findings, and citation information.

Researchers interested in collaboration or further details are welcome to contact the authors.

---

## Citation

If you use this work, please cite:

```bibtex
@article{ELALFY2026868,
title = {Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting},
journal = {Transportation Research Procedia},
volume = {96},
pages = {868-875},
year = {2026},
note = {TRPRO_SMILE 2026},
issn = {2352-1465},
doi = {https://doi.org/10.1016/j.trpro.2026.04.067},
url = {https://www.sciencedirect.com/science/article/pii/S2352146526003285},
author = {El-Sayed M. El-Alfy and Shahbaaz A. Sadiq and Mohammed Ayub and M Faisal Nurnoby},
keywords = {Electric vehicle, Charging demand, Temporal Fusion Transformer, Forecasting, Multi-horizon},
abstract = {Traditional forecasting approaches struggle to accurately model the high temporal volatility of electric vehicle (EV) charging demand, which is influenced by factors such as socioeconomic conditions, seasonal cycles, and regulatory incentives. In this paper, we present a Temporal Fusion Transformer (TFT)-based predictive modeling framework for short-term, multi-horizon forecasting of station-level occupancy rates. The model combines static station metadata, known-future calendar/tariff signals, and observed-past local history with spatial neighbor aggregates to provide attention-based interpretability through variable selection and masked, interpretable multi-head attention. Evaluated on the ST-EVCDP dataset, the TFT-based model achieved very high accuracy when compared to other methods across nine stations at 5-minute resolution with an average Mean Absolute Error (MAE) of 0.0064 and a high Coefficient of Determination (R2) of 0.959, indicating outstanding predictive performance.}
}
```

---

## License

This repository is distributed under the MIT License.

---

## Acknowledgments

The authors thank King Fahd University of Petroleum and Minerals (KFUPM) for supporting this research.

