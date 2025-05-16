# 🧠 Anomaly Detection with Transformer Model in High-Energy Physics (HEP)

## Overview

This repository contains a machine learning-driven analysis pipeline designed to enhance the discovery potential in High-Energy Physics (HEP) using **ATLAS Run-2 Open Data (2015–2016)**.

The goal is to preprocess ATLAS collision data and apply a **Transformer-based unsupervised anomaly detection model** to identify rare or Beyond the Standard Model (BSM) physics events hidden within large Standard Model backgrounds.

---

## 🚀 Project Highlights

- **Data Source:** ATLAS Open Data (Run 2, 2015–2016) in PhysLite `.root` format  
- **Processing Tools:** ROOT with Dask for scalable parallel data processing  
- **ML Model:** TabTransformer architecture tailored for tabular HEP data  
- **Objective:** Train on Standard Model background only, detect anomalies as events with high reconstruction loss  
- **Features:** Uses low-level physics variables such as jet/lepton kinematics, missing transverse energy, calorimeter deposits, and event topology  
- **Output:** Structured datasets (`.csv`, `.h5`) ready for anomaly detection downstream tasks

---

## 🧪 Notebook Contents

- Data extraction and selection of physics variables  
- Parallel processing of large `.root` datasets using Dask and ROOT RDataFrame  
- Preprocessing and filtering of collision events  
- Transformer-based reconstruction model for anomaly detection  
- Analysis of model performance and interpretation of results  

---

## 🔧 Setup & Usage

### Key Libraries & Frameworks

- ROOT and Dask for efficient HEP data handling  
- pandas, numpy for data manipulation  
- matplotlib, seaborn for visualization  
- PyTorch for implementing the Transformer model

### How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Anomaly-detection-with-transformer-model-in-HEP.git
   cd Anomaly-detection-with-transformer-model-in-HEP
