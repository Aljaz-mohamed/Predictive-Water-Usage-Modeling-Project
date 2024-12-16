# Predictive-Water-Usage-Modeling-Project
## Overview
FairWater is a machine learning project that focuses on analyzing and forecasting household water usage using time series data. It leverages advanced predictive modeling techniques and anomaly detection to optimize water management and minimize wastage. Key features include:

- **Time Series Forecasting**: Implementation of LSTM, GRU, and XGBoost models to predict water consumption patterns.
- **Anomaly Detection**: Utilization of the ADTK library to detect unusual water usage behaviors.
- **Exploratory Data Analysis (EDA)**: Insights into water consumption trends across various household fixtures.

This project is a part of the CSC8633 Group Project in Data Science, conducted in collaboration with Newcastle University and industry partners.

---

## Repository Structure
```
data/
├── raw/                # Original dataset files
├── processed/          # Cleaned/processed data

notebooks/
├── eda.ipynb           # Exploratory Data Analysis notebook
├── time_series_models.ipynb  # LSTM, GRU, XGBoost implementation
├── anomaly_detection.ipynb   # ADTK anomaly detection models

requirements.txt         # Python dependencies
```

---

## Key Features
1. **Exploratory Data Analysis (EDA)**:
   - Provides an overview of household water consumption trends.
   - Visualizations of seasonal, monthly, and fixture-level water usage patterns.

2. **Time Series Modeling**:
   - **LSTM, GRU, and Simple RNN**: Capture long-term dependencies in sequential data.
   - **XGBoost**: Efficiently models non-linear relationships and delivers high accuracy for hourly and weekly predictions.

3. **Anomaly Detection**:
   - Utilizes the ADTK library for identifying anomalies such as spikes, drops, and level shifts.
   - Algorithms include InterQuartileRangeAD, AutoregressionAD, PersistAD, and LevelShiftAD.

---

## Setup Instructions

### Prerequisites
Ensure you have the following installed:
- Python 3.8+
- Jupyter Notebook

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/username/FairWater.git
   cd FairWater
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook to explore the provided notebooks:
   ```bash
   jupyter notebook
   ```

---

## Usage
1. **Data Preprocessing**:
   - Place the raw dataset files in the `data/raw/` folder.
   - Process and clean the data using the steps outlined in the `eda.ipynb` notebook. Save processed data to `data/processed/`.

2. **Exploratory Data Analysis**:
   - Open the `notebooks/eda.ipynb` notebook to visualize and analyze household water usage trends.

3. **Time Series Modeling**:
   - Use the `notebooks/time_series_models.ipynb` notebook to run predictive models and evaluate their performance.

4. **Anomaly Detection**:
   - Detect anomalies in water usage using the `notebooks/anomaly_detection.ipynb` notebook.

---

## Results
- **Exploratory Data Analysis**: Identified significant fluctuations in water usage across different seasons and fixtures.
- **Modeling**:
   - XGBoost achieved the highest accuracy for time series forecasting with an R² score of 0.97.
   - LSTM and GRU models were tested but were limited by data constraints.
- **Anomaly Detection**:
   - Successfully detected spikes, drops, and level shifts in water flow data.

---

## Dependencies
The project uses the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- tensorflow
- xgboost
- adtk

Install all dependencies using the `requirements.txt` file.

---

## Project Highlights
- Developed predictive models tailored to water consumption data.
- Enhanced water management insights through anomaly detection and trend analysis.
- Created reproducible and modular notebooks for each analysis stage.
