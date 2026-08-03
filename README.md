<div align="center">

# 🌍 Geospatial Property Valuation

### GNN / Attention-Based Real Estate Valuation Engine

**Beating tabular baselines by modeling how neighborhoods actually shape price.**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![PyTorch](https://img.shields.io/badge/PyTorch-Geometric-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)](https://pytorch.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-Baseline-018EFA?style=for-the-badge)](https://xgboost.readthedocs.io/)
[![Streamlit](https://img.shields.io/badge/Streamlit-Dashboard-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://streamlit.io/)
[![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge)]()
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)]()

</div>

---

## 📌 Overview

**Geospatial Property Valuation** is a 4-week sprint project that builds a **spatial-embedding / Graph Neural Network (GNN)** based property valuation engine for the **Construction & Real Estate** domain.

Traditional tabular models (like XGBoost) treat every property in isolation — they don't understand that a house's value is deeply tied to *what's around it*. This project fixes that by representing properties as nodes in a **spatial graph**, connecting each one to its nearest neighbors, and letting a GNN/Attention model learn how neighborhoods actually shape price.

> 🎯 **Goal:** Beat the XGBoost tabular baseline's MAPE using spatial embeddings + GNN/Attention.

---

## ✨ Key Features

| 🚀 Feature | Description |
|---|---|
| 🗺️ **Geospatial Processing** | Haversine distance utilities, spatial cleaning, interactive Folium/Kepler.gl visualizations |
| 📊 **Baseline Model** | Tuned XGBoost regressor on engineered tabular features |
| 🕸️ **Graph Construction** | KNN-based property neighborhood graph built with BallTree + haversine metric |
| 🧠 **GNN / Attention Model** | GraphSAGE / GAT-style architecture in PyTorch Geometric |
| 📈 **Model Comparison** | Transparent MAPE/RMSE benchmarking: Baseline vs GNN |
| 🖥️ **Interactive Dashboard** | Streamlit app with address input, price prediction, and neighbor influence heatmap |

---

## 🏗️ Tech Stack

<div align="center">

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![GeoPandas](https://img.shields.io/badge/-GeoPandas-139C5A?style=flat-square&logo=pandas&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![PyG](https://img.shields.io/badge/-PyTorch%20Geometric-3C2179?style=flat-square)
![XGBoost](https://img.shields.io/badge/-XGBoost-018EFA?style=flat-square)
![Scikit--learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![Folium](https://img.shields.io/badge/-Folium-77B829?style=flat-square)
![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)

</div>

---

## 📂 Project Structure

```
Geospatial-Property-Valuation/
├── data/            # Raw & processed datasets (gitignored)
├── notebooks/        # Exploration & experimentation notebooks
├── src/              # Core source code
│   ├── geo_utils.py       # Haversine distance & spatial helpers
│   ├── build_features.py  # Tabular feature engineering
│   ├── build_graph.py     # Graph construction pipeline
│   ├── gnn_model.py       # GNN/Attention architecture
│   └── graph_viz.py       # Graph visualization helpers
├── models/           # Trained model checkpoints (gitignored)
├── app.py            # Streamlit dashboard
├── results_comparison.md  # Baseline vs GNN results log
├── model_results.md       # Model tracking table
└── README.md
```

---

## 🗓️ Sprint Roadmap

| Week | Focus | Status |
|---|---|---|
| **Week 1** | 🌐 Geospatial Data Acquisition & Processing | 🟡 In Progress |
| **Week 2** | 🧮 Feature Engineering & Baseline ML | ⚪ Upcoming |
| **Week 3** | 🕸️ Spatial Embeddings & Graph Construction | ⚪ Upcoming |
| **Week 4** | 🧠 GNN/Attention Modeling & Dashboard | ⚪ Upcoming |

---

## ⚡ Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/tarunsaxena2/Geospatial-Property-Valuation.git
cd Geospatial-Property-Valuation
```

### 2. Set up the environment
```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate   # macOS/Linux

pip install geopandas shapely folium xgboost torch pandas
```

### 3. Run the dashboard *(once built)*
```bash
streamlit run app.py
```

---

## 👥 Team

<div align="center">

| Member | Role |
|---|---|
| **Tarun Saxena** | Geospatial Data Engineer + Integration & Deploy Lead |
| **Vaibhav Gautam** | Baseline ML Engineer + Graph/GNN Engineer |

</div>

---

<div align="center">

**⭐ Built as part of a 4-week engineering sprint at Infotact Solutions & Co. ⭐**

</div>
