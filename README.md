# Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting

[![Conference]((https://smileconf.com/en))]()
[![Paper]((https://www.sciencedirect.com/science/article/pii/S2352146526003285))]()

## Overview

This repository accompanies the research paper:

**Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting**

presented at:

**The 2nd International Conference on Smart Mobility and Logistics Ecosystems (SMiLE 2025)**
King Fahd University of Petroleum and Minerals (KFUPM), Saudi Arabia.

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

## Paper

The full conference paper is available in:

```text
paper/Temporal_Fusion_Transformer_EV_Forecasting.pdf
```

---

## Code Availability

The implementation used in this study is not publicly released at this time.

This repository is intended to provide access to the published research article, methodology, experimental findings, and citation information.

Researchers interested in collaboration or further details are welcome to contact the authors.

---

## Citation

If you use this work, please cite:

```bibtex
@inproceedings{sadiq2025tft,
  title={Temporal Fusion Transformer-Based Framework for Electric Vehicle Charging Demand Forecasting},
  author={El-Alfy, El-Sayed M. and Sadiq, Shahbaaz A. and Ayub, Mohammed and Nurnoby, M. Faisal},
  booktitle={The 2nd International Conference on Smart Mobility and Logistics Ecosystems (SMiLE)},
  year={2025}
}
```

---

## License

This repository is distributed under the MIT License.

---

## Acknowledgments

The authors thank King Fahd University of Petroleum and Minerals (KFUPM) for supporting this research.
