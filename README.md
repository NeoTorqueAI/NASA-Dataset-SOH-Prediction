# NASA-Dataset-SOH-Prediction
Author - Yash Shandilya
Short Description:- ML project to predict Li-ion battery State of Health (SOH) and Remaining Useful Life (RUL) using NASA’s battery dataset. Includes data preprocessing, feature engineering, machine learning modeling, and result visualization. Aims to support predictive maintenance in EVs with interpretable ML insights.
# 🔋 Battery SOH & RUL Prediction Using ML (NASA Dataset)

This project builds a machine learning pipeline to predict the **State of Health (SOH)** and **Remaining Useful Life (RUL)** of lithium-ion batteries using the publicly available NASA Prognostics battery dataset. The goal is to enable smart, interpretable battery health diagnostics for use in EVs and predictive maintenance systems.

---

## 📂 Dataset

- **Source**: [NASA Ames Prognostics Data Repository](https://www.nasa.gov/content/prognostics-center-of-excellence-data-set-repository)
- **Format**: Cycle-wise CSV logs of battery charge/discharge experiments  
- **Features**: Voltage, Current, Temperature, Capacity, Cycle number  
- **Target Variables**:
  - **SOH**: State of Health (% of rated capacity)
  - **RUL**: Remaining number of cycles until End-of-Life (EOL)

---

## 🛠 Project Structure

```plaintext
├── data/                  # Raw and processed battery datasets
├── notebooks/             # Jupyter notebooks for each step
│   ├── 01_data_loading.ipynb
│   ├── 02_feature_engineering.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_visualization.ipynb
├── models/                # Trained models and saved artifacts
├── src/                   # Python modules for pipeline components
├── results/               # Evaluation metrics, SHAP plots, graphs
├── README.md              # Project overview and instructions
├── requirements.txt       # Python dependencies
└── environment.yml        # (Optional) Conda environment file
