# Cross-Project-TBM-Database_net-penetration-rate_prediction_ML- 
### Machine Learning Approach for Prediction of TBM Performance and Associated Risk in Himalayan Geology Using a Cross-Project Tunnelling Database

**Authors:** Tek Bahadur Katuwal, Krishna Kanta Panthi, Chhatra Bahadur Basnet  
**Institution:** Norwegian University of Science and Technology (NTNU)

---

## Table of Contents
1. [Overview](#1-overview)  
2. [Key Objectives](#2-key-objectives)  
3. [Database Availability](#3-database-availability)  
4. [Repository Structure](#4-repository-structure)  
5. [Data & Methodology](#5-data--methodology)  
6. [Key Findings](#6-key-findings)  
7. [Insights](#7-insights)  
8. [Conclusions](#8-conclusions)

---

## 1. Overview
This repository presents a **machine learning (ML)-based framework** for **TBM penetration rate prediction** in the challenging geological conditions of the Himalayas. The study utilizes **Cross-Project Database** with **TBM operational data from the Bheri Babai Diversion Multipurpose (BBDM) Project and Sunkoshi Marin Diversion Multipurpose (SMDM) project in Nepal**.

### Key Highlights
- Machine learning (ML)-based model developed to predict **TBM net penetration rate (PRnet)** using **cross-project database**.  
- **TBM operational parameters** and **geological conditions** are utilized as input parameters.  
- Prediction model incorporates **data anomalies** associated with complex geological environments.  
- Impact of input features on TBM net penetration rate evaluated using the **SHAP method**.  
- **Combined Jamming Risk (CJR)** scoring system used to forecast TBM jamming risk.
- **TBM jamming** can potentially be predicted **at least 1.5 m ahead** of the tunnel face.
- **Empirical ranges** of TBM parameters were established to ensure **operational safety**.



---

## 2. Key Objectives
Develop a well-structured **Machine Learning (ML)-based framework** to predict **TBM net penetration rate (PRnet)** in complex geological environments using **Cross-Project Database**.

---

## 3. Database Availability
Due to project confidentiality, the dataset **cannot be publicly shared**.

**Details:**
- **Source:** Bheri Babai Diversion Multipurpose (BBDM) Project and Sunkoshi Marin Diversion Multipurpose (SMDM) project, Nepal 
- **Size:** 8,614 (from BBDMP) and 9,471 (from SMDMP)TBM cycle datasets with corresponding mapped geological parameters  

---

## 4. Repository Structure
Cross-Project-TBM-Database_net-penetration-rate_prediction_ML/
│
├── 1. Data Analysis and Visualisation for_Both Projects.ipynb
│ (Script that produces general dataset info, Pearson Correlation Analysis,
│ feature importance, Box–Whisker & Violin Plot, histogram distributions)
│
├── 2. PRnet Prediction for TBM Tunneling Using Cross-Project Datasets.ipynb
│ (Scripts for ML model with different scenarios)
│
├── 2. PRnet Prediction for TBM Tunneling Using Cross-Project Datasets.ipynb
│ ├── Scripts for ML model with different scenarios
│ └── Model interpretability and feature influence analysis using SHAP
│
├── 3. TBM Jamming Risk Assessment.ipyn
│ (Analysis of TBM performance with rock mass quality, and TBM parameters; Prediction of potential jamming events;
│ Prediction of potential jamming events; Empirical range of parameters)
│
└── README.md
---

## 5. Data & Methodology

- **Dataset:** Cross-project databse
  
- **Input Features:**  
  - Geological: Rock mass rating (RMR), weathering, rock strength  
  - Machine: Torque, thrust, cutterhead speed (CRS), penetration rate (PRchd)
- **ML Models Used:**    
  - *Ensemble:* Bagging, Random Forest, XGBoost, Stacking  
  - *Neural Network:* Artificial Neural Network (ANN)
- **Evaluation Metrics:** R², MAE, RMSE, MAPE  
- **Interpretability Tool:** SHAP (Shapley Additive Explanations)

---

## 6. Key Findings

- **The merged and shuffled cross-project database results in improved model performance, with:**R² values ranging from 0.956 to 0.963**.  
- **SHAP Analysis:**  
  - Most influential features: Cutterhead penetration rate (PRchd), cutterhead speed (CRS), rock mass rating (RMR), torque, thrust.  
  - Geological features (lithology, rock strength) also contributed but with lesser influence.  
- **TBM jamming can potentially be predicted at least 1.5 m ahead of the tunnel face**.  
- **Empirical ranges of TBM parameters were established to ensure operational safety**.

---

## 7. Insights

- **Geological Complexity:** Himalayan geology exhibits extreme variability due to tectonic activity, making TBM performance prediction challenging.  
- **ML Advantage:** Machine learning models outperform traditional empirical/statistical approaches in capturing nonlinear dependencies and handling complex datasets.  
- **Safety & Efficiency:** The framework aids in **early risk detection**, **optimization of TBM operations**, and **enhancement of tunneling safety**.

---

## 8. Conclusions

- ML-based models can accurately predict TBM performance in **complex geological environments**.  
- Integration of **geological and machine parameters** enhances model reliability.  
- The developed framework is **generalizable** but requires further validation using **data from other tunneling projects**.

---

**© 2025 Norwegian University of Science and Technology (NTNU)**  
*Authors: Tek Bahadur Katuwal, Krishna Kanta Panthi  & Chhatra Bahadur Basnet*
