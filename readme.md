# Machine Learning-Based Short-Term Earthquake Forecasting for the Indian Plate Seismogenic System

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.XXXXXXX.svg)](https://doi.org/10.5281/zenodo.XXXXXXX)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)

This repository contains the complete code, data processing pipeline, and model implementations for the paper:

> **"Machine Learning-Based Short-Term Earthquake Forecasting for the Indian Plate Seismogenic System: A Multi-Zone, Multi-Threshold Ensemble Study with Interpretability and ETAS Benchmarking"**  

| # | Author | Affiliation | Email | ORCID |
|---|--------|-------------|-------|-------|
| 1,2 | **Uday Pratap Singh** * (Corresponding) | Dept. of AI & Data Science, Poornima Institute of Engineering and Technology, Jaipur; K. Banerjee Centre of Atmospheric & Ocean Studies, University of Allahabad | udaypratap@allduniv.ac.in<br>uday.pratap@poornima.org | [0000-0001-7573-8550](https://orcid.org/0000-0001-7573-8550) |
| 3 | **Bersha Kumari** | Dept. of Computer Engineering, Poornima Institute of Engineering and Technology, Jaipur | bersha.kumari@poornima.org | [0009-0000-0724-8875](https://orcid.org/0009-0000-0724-8875) |
| 1 | **Ebtasam Ahmad Siddiqui** | Dept. of AI & Data Science, Poornima Institute of Engineering and Technology, Jaipur | ebtasam.siddiqui@poornima.org | [0000-0002-0323-5441](https://orcid.org/0000-0002-0323-5441) |

**Affiliations:**  
¹ Department of AI & Data Science, Poornima Institute of Engineering and Technology, Jaipur, India  
² K. Banerjee Centre of Atmospheric & Ocean Studies, University of Allahabad, India  
³ Department of Computer Engineering, Poornima Institute of Engineering and Technology, Jaipur, India

## 📋 Overview

This study presents the first systematic multi-architecture, multi-threshold machine learning earthquake forecasting benchmark for the Indian plate system. We train and evaluate:

- **Tabular models**: Logistic Regression, Balanced Random Forest (BRF), XGBoost
- **Deep learning models**: LSTM, TCN, WaveNet, Transformer
- **Baseline**: ETAS (Epidemic-Type Aftershock Sequence)

Forecasting targets: M≥5.5, M≥6.0, M≥6.5 over a 30-day horizon across five seismotectonic zones.

### Key Results
| Model | Target | ROC-AUC | BSS |
|-------|--------|---------|-----|
| XGB | M≥5.5 | **0.725** | 0.140 |
| BRF | M≥6.0 | **0.651** | -0.014 |
| XGB | M≥6.5 | **0.776** | 0.005 |
| WaveNet | Himalaya M≥5.5 | 0.640 | 0.023 |

## 📦 Repository Structure
