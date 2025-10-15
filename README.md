# Graph Neural Networks for IoT Sensor Network Optimization

This repository contains the complete implementation, analysis, and manuscript supporting the master’s thesis **“Graph Neural Networks for IoT Sensor Network Optimization: A Spatio-Temporal Forecasting Approach.”**

---

## Overview
The study explores how **Graph Neural Networks (GNNs)** can improve temperature forecasting accuracy in IoT sensor networks by modeling spatial dependencies among sensor nodes. The results show significant improvements compared to traditional machine learning methods while maintaining computational efficiency for real-world deployment.

---

## Dataset
- **Source:** [Intel Berkeley Research Lab](https://www.kaggle.com/datasets/divyansh22/intel-berkeley-research-lab-sensor-data/data)  
- **Description:** 54 Mica2Dot sensors deployed across an indoor environment collecting temperature, humidity, light, and voltage readings at 31-second intervals.  
- **Usage:** This study focuses primarily on temperature forecasting and spatial relationships among sensors.

---

## Methodology
- Data preprocessing and feature engineering  
- Graph construction based on sensor coordinates  
- Implementation of **Graph Convolutional Networks (GCN)** using PyTorch Geometric  
- Comparative evaluation with baseline models (Random Forest, LSTM, MLP)  
- Forecasting for horizons of 1, 3, and 5 steps  
- Sensor-level error analysis and ablation studies

---

## Getting Started

### Prerequisites
- Python 3.10+
- Jupyter Notebook
- PyTorch Geometric
- Pandas, NumPy, Scikit-learn, Matplotlib, NetworkX

### Installation
```bash
git clone https://github.com/swathikalburgi/GNN-IoT-Temperature-Forecasting-Study.git
cd GNN-IoT-Temperature-Forecasting-Study
pip install -r requirements.txt
`````

### Running the Notebook 
Open: [GNN_IoT_Temperature_Forecasting_Study_vFinal.ipynb](https://colab.research.google.com/drive/1_4m4CXXSrhlFrIx7gtkiyOLiLlQALIxq?usp=sharing)

---

## Key Results
- GCN outperformed Random Forest with a 73.16% reduction in MSE.
- Captured spatial correlations effectively across 54 sensors.
- Achieved stable forecasting performance across horizons 1, 3, and 5.
- Demonstrated unbiased estimators with near-zero mean error.
