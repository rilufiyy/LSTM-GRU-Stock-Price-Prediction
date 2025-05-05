# 📈 Stock Price Prediction using LSTM & GRU

This project aims to predict stock prices of selected Indonesian property companies using deep learning models, specifically **LSTM** (Long Short-Term Memory) and **GRU** (Gated Recurrent Unit). The dataset used includes daily stock price data from 10 companies, and the goal is to model temporal dependencies to forecast future prices.

## 🗂️ Companies Covered

- APLN (Agung Podomoro Land)
- BSDE (Bumi Serpong Damai)
- CTRA (Ciputra Development)
- DILD (Intiland Development)
- DMAS (Puradelta Lestari)
- LPKR (Lippo Karawaci)
- MDLN (Modernland Realty)
- PANI (Pantai Indah Kapuk Dua)
- PWON (Pakuwon Jati)
- SMRA (Summarecon Agung)

## 📌 Objectives

- Perform **exploratory data analysis (EDA)** on stock prices.
- Apply **data preprocessing**, including normalization and sequence generation.
- Train and compare **LSTM** and **GRU** models on each company’s stock price data.
- Evaluate model performance using metrics such as **MAE**, **RMSE**, and **MSE**.
- Visualize actual vs predicted stock prices for insight and comparison.

## 🛠️ Tech Stack

- **Python**
- **Pandas**, **NumPy** – data manipulation
- **Matplotlib**, **Seaborn**, **Plotly** – visualization
- **TensorFlow**, **Keras** – deep learning models
- **Scikit-learn** – metrics and preprocessing

## 🧠 Methodology

1. **Data Preparation**
   - Load and clean stock price data.
   - Use closing price as primary target.
   - Normalize using `MinMaxScaler`.
   - Generate sequences with lookback window.

2. **Modeling**
   - Build LSTM and GRU models using Keras Sequential API.
   - Train models per company dataset.
   - Tune hyperparameters such as epochs, batch size, units.

3. **Evaluation**
   - Compare model predictions with actual prices.
   - Use error metrics to assess model quality.
   - Visualize with line plots to interpret trends.

## 📊 Results & Insights

- LSTM performed better for longer-term dependencies, while GRU offered faster convergence.
- Stock price trends in certain companies like SMRA and PWON showed higher predictability due to more stable fluctuations.

## 📁 Folder Structure
LSTM-GRU-Stock-Prediction/
│
├── data/ # CSV files of stock prices (e.g., apln.csv, bsde.csv, etc.)
├── notebooks/ # Jupyter Notebooks for EDA, LSTM, GRU models
├── models/ # Saved model files (.h5)
├── results/ # Plots and evaluation metrics
├── README.md
├── requirements.txt
└── utils.py # Custom preprocessing functions


## 🔮 Future Improvements

- Integrate real-time stock data with APIs.
- Deploy as a web dashboard using Streamlit or Flask.
- Extend to other sectors (banking, consumer goods).
- Add attention mechanism for enhanced temporal focus.

## 📎 Requirements

To install the required dependencies:

```bash
pip install -r requirements.txt


