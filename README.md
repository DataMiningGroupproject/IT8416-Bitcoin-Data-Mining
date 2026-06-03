
# IT8416 Data Mining – Group Project
 Bitcoin Price Prediction

Bahrain Polytechnic — Course **IT8416 (Data Mining)**

This project applies the Data Mining (KDD) life cycle to predict the next-day price direction (Up / Down) of Bitcoin using historical market data and engineered technical and blockchain indicators. Models were built and evaluated in RapidMiner .

---

## Group Members

| # | Name | Student ID | Role |
|---|------|-----------|------|
| 1 |   Abdulla Murad     | 202302258 | Data Scientist |
| 2 | Mishal Alaraibi  | 202301287  | Data Mining Engineer |
| 3 | Hood Alabbasi  | Hood Alabbasi  | Data Analyst |
| 4 | Ahmed Alansari  | 202304215  | Data Analyst / Coordinator |

**Section / Class No:** 001   **Group No:** 3

---

## Project Overview

- **Problem:** Classify whether Bitcoin's next-day closing price will go up or down.
- **Data:** Daily Bitcoin OHLCV history (Apr 2013 – Sep 2017) from Kaggle's "Cryptocurrency Historical Prices" dataset, merged with blockchain network metrics.
- **Pipeline (KDD):** Data selection → cleaning → feature engineering → redundancy removal → normalization → PCA → modelling → evaluation.
- **Models:** Decision Tree, k-Nearest Neighbours (k=15), and a Random Forest ensemble, evaluated with Accuracy, Precision, Recall, F1 and confusion matrices using a chronological test split.

## Key Result

None of the models convincingly beat the ~58% majority-class baseline. k-NN was the most balanced model (highest real F1 ≈ 71%), the Decision Tree only matched the baseline by always predicting "Up", and the Random Forest was the weakest — an honest finding showing next-day Bitcoin direction is only weakly predictable from price/volume data.

---

## Repository Contents

| File | Description |
|------|-------------|
| `Data Mining Report Class1 Group3.docx` | Final project report (all 6 tasks) |
| `IT8416_Bitcoin_Process.rmp` | RapidMiner / AI Studio process file |
| `bitcoin_modeling_dataset.csv` | Cleaned, feature-engineered dataset used for modelling |
| `bitcoin_price.csv` | Original raw Bitcoin price data |
| `bitcoin_dataset.csv` | Original blockchain metrics data |
| `video_link.txt` | Link to the narrated demonstration video |

## How to Reproduce

1. Open `IT8416_Bitcoin_Process.rmp` in RapidMiner .
2. Import `bitcoin_modeling_dataset.csv` into the repository.
3. Run the process to reproduce the preprocessing, PCA, models and performance results.

---

