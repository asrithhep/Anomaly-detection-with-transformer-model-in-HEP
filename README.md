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
- **Output:** Selected variables saved via ROOT RDataFrame snapshots, then fed into the ML model using TMVA TensorFlow batch generators for efficient training and evaluation  

---

## 🧪 Notebook Contents

- Data extraction and selection of physics variables  
- Parallel processing of large `.root` datasets using Dask and ROOT RDataFrame  
- Preprocessing and filtering of collision events  
- Saving selected variables with ROOT RDataFrame snapshot method  
- Feeding snapshot files into the ML pipeline via TMVA TensorFlow batch generators  
- Transformer-based reconstruction model for anomaly detection  
- Analysis of model performance and interpretation of results  

---

## 🔧 Setup & Usage

### Key Libraries & Frameworks

- ROOT and Dask for efficient HEP data handling 
- matplotlib, seaborn for visualization  
- tensorflow for implementing the Transformer model  
- TMVA TensorFlow batch generators for scalable input pipeline
- use container : gitlab-registry.cern.ch/asradhak/ml_cern_ch_docker_image@sha256:e97a96db2ff0bcb7270a22d943679a2e0483d26fcfcf650028c7ce6e39522ca0

### How to run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/Anomaly-detection-with-transformer-model-in-HEP.git
   cd Anomaly-detection-with-transformer-model-in-HEP
