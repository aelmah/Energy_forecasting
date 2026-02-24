#### Robust Bi-LSTM Attention Energy Forecaster
A deep learning framework for Short-Term Load Forecasting (STLF) using a Bidirectional LSTM integrated with a Self-Attention mechanism. This model predicts a consecutive 24-hour energy consumption horizon with high precision.

#### Key Features
***Architecture*** Bi-LSTM for bidirectional temporal context + Self-Attention for peak demand prioritization.

***Cyclical Encoding:*** Sine/Cosine transformations for hour and day features to maintain temporal continuity.

***Robust Optimization:*** Implements Huber Loss to minimize the impact of energy spikes and outliers.

***Performance:*** Achieved a 3.74% MAPE on the AEP hourly dataset.

#### Results
The model effectively mitigates the "multi-step penalty" typically seen in standard RNNs, tracking high-gradient transitions during peak demand periods more accurately than vanilla LSTMs.

Setup
1- Clone the repository:
```bash
https://github.com/aelmah/Energy_forecasting/
```
2- Install dependencies:
```bash
pip install -r requirements.txt
``` 
3- Run the notebook/script to train and evaluate on the AEP dataset.

