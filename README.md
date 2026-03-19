# uruguay-exchange-rate-forecasting-wiht-ML-and-DL

## 🧠 Project Description

This repository contains the full development of a Master's thesis in Data Science focused on forecasting the USD/UYU exchange rate in Uruguay.

The project combines traditional econometric approaches with advanced Machine Learning and Deep Learning models, using a database built from multiple economic, financial, and external data sources.

A reproducible notebook-based pipeline is implemented, covering the full workflow from data construction to production forecasting.

---

## 🎯 Objectives

- Forecast the USD/UYU exchange rate over the following horizons:
  - 1 month
  - 3 months
  - 6 months
  - 12 months

- Compare the performance of:
  - Machine Learning models
  - Deep Learning models
  - Traditional econometric benchmarks:
    - Random Walk
    - RPPP (Relative Purchasing Power Parity)
    - CIRP (Covered Interest Rate Parity)
    - BCU survey expectations

- Identify the most relevant variables explaining exchange rate dynamics.

- Build an automated and reproducible pipeline for economic forecasting.

---

## ⚙️ Methodology

The project follows a structured pipeline-based approach:

1. **Database construction**
   - Integration of multiple economic and financial data sources.
   - Daily-frequency data with transformations tailored to forecasting horizons.

2. **Feature engineering**
   - Transformations such as log-differences, lags, and normalizations.
   - Generation of explanatory variables and forward-looking targets.

3. **Feature selection**
   - Horizon-specific correlation analysis
   - Multicollinearity reduction
   - Stability assessment across forecasting horizons

4. **Benchmark models**
   - Random Walk
   - RPPP
   - CIRP
   - BCU expectations

5. **Predictive models**
   - Machine Learning models (e.g., Random Forest, XGBoost, etc.)
   - Deep Learning models (e.g., LSTM, GRU, hybrid architectures)

6. **Performance evaluation**
   - Out-of-sample metrics
   - Model comparison
   - Best-model selection by forecasting horizon

7. **Production**
   - Final pipeline for generating forecasts in a production environment

---

## 🗂️ Repository Structure

```text
Base_de_datos/
Flujo/
Produccion/
📁 Base_de_datos

Contains the consolidated database and the original inputs used throughout the project.

📁 Flujo

Contains the full project pipeline divided into sequential notebooks.

📁 Produccion

Contains the final notebook designed for forecast generation in a production environment.

🧪 Technologies Used

Python

Pandas / NumPy

Scikit-learn

XGBoost / LightGBM

TensorFlow / Keras / PyTorch

Matplotlib

Jupyter Notebooks

▶️ How to Reproduce the Project

Clone the repository

git clone <repo-url>
cd <repo-name>

Install dependencies

pip install -r requirements.txt

Run the notebooks in sequence

Flujo/
N00 → N01 → N02 → N03 → N04 → N05 → N06

Run the production notebook

Produccion/N07_produccion.ipynb
📌 Notes

Some notebooks are intended for research and experimentation, while others are part of the production pipeline.

Folder names and execution order are important for reproducibility.

Model artifacts may be stored in separate directories depending on the workflow.

© Copyright and Use

© 2026 Juan Briozzo. All rights reserved.

This repository is made publicly available for viewing and academic reference only.
No permission is granted to copy, modify, distribute, publish, sublicense, or use the code, notebooks, text, figures, or other materials contained in this repository without prior written permission from the author.

Unauthorized reproduction, redistribution, or commercial use of any part of this repository is strictly prohibited.

Pa creo que te estás apurando, me dejás secciones por afuera como texto plano sin un buen formato. tomate tu tiempo y devolvemo bien por favor, es para un Read.Me, no lo olvides
Pensó durante un segundo
# Exchange Rate Forecasting in Uruguay: A Machine Learning and Deep Learning Approach

## 🧠 Project Description

This repository contains the full development of a Master's thesis in Data Science focused on forecasting the USD/UYU exchange rate in Uruguay.

The project combines traditional econometric approaches with advanced Machine Learning and Deep Learning models, using a database built from multiple economic, financial, and external data sources.

It implements a reproducible notebook-based pipeline that covers the entire workflow, from data construction and feature engineering to model evaluation and production forecasting.

---

## 🎯 Objectives

The main objectives of this project are:

- To forecast the USD/UYU exchange rate over the following horizons:
  - 1 month
  - 3 months
  - 6 months
  - 12 months

- To compare the performance of:
  - Machine Learning models
  - Deep Learning models
  - Traditional econometric benchmarks, including:
    - Random Walk
    - RPPP (Relative Purchasing Power Parity)
    - CIRP (Covered Interest Rate Parity)
    - BCU survey expectations

- To identify the most relevant variables explaining exchange rate dynamics.

- To build an automated and reproducible pipeline for economic forecasting.

---

## ⚙️ Methodology

The project follows a structured pipeline-based approach composed of the following stages:

### 1. Database Construction
- Integration of multiple economic and financial data sources.
- Construction of a unified daily-frequency dataset.
- Preparation of the data according to the requirements of each forecasting horizon.

### 2. Feature Engineering
- Application of transformations such as log-differences, lags, and normalizations.
- Creation of explanatory variables.
- Construction of forward-looking target variables.

### 3. Feature Selection
- Horizon-specific correlation analysis.
- Reduction of multicollinearity.
- Assessment of variable stability across forecasting horizons.

### 4. Benchmark Models
Traditional benchmark models are included for comparison purposes:
- Random Walk
- RPPP
- CIRP
- BCU expectations

### 5. Predictive Models
The predictive framework includes both Machine Learning and Deep Learning approaches:

- **Machine Learning**
  - Random Forest
  - XGBoost
  - LightGBM
  - Support Vector Regression
  - Other tree-based and supervised learning models

- **Deep Learning**
  - LSTM
  - GRU
  - Hybrid recurrent architectures

### 6. Performance Evaluation
- Out-of-sample evaluation metrics.
- Model comparison across horizons.
- Selection of the best-performing model for each forecasting horizon.

### 7. Production
- Final notebook for generating forecasts in a production environment.
- Reproducible workflow for updating inputs and producing new predictions.

---

## 🗂️ Estructura del Repositorio


📁 Base_de_datos/
📁 Flujo/
📁 Produccion/


### 📁 Base_de_datos
Contains the consolidated database and the original inputs used throughout the project.

### 📁 Flujo
Contains the full research and modeling pipeline divided into sequential notebooks..

### 📁 Produccion
Contains the final notebook designed for forecast generation in a production environment.

---

## 🧪 Tecnologías Utilizadas

- Python 🐍
- Pandas / NumPy
- Scikit-learn
- XGBoost / LightGBM
- TensorFlow / Keras / PyTorch (Deep Learning)
- Matplotlib / Seaborn
- Jupyter Notebooks

---

## ▶️ Cómo Reproducir el Proyecto

1. Clone the repository

```bash
git clone <repo-url>
cd <repo-name>

2. Install dependencies:

pip install -r requirements.txt

3. Run the notebooks in sequence

The research pipeline is organized as a sequence of notebooks inside the Flujo/ folder:

Flujo/
N00 → N01 → N02 → N03 → N04 → N05 → N06

4. Run the production notebook

Produccion/N07_produccion.ipynb



## © Copyright and Use

© 2026 Juan Briozzo. All rights reserved.

This repository is made publicly available for viewing and academic reference only.

No permission is granted to copy, modify, distribute, publish, sublicense, reuse, or otherwise exploit the code, notebooks, text, figures, or any other materials contained in this repository without prior written permission from the author.

Unauthorized reproduction, redistribution, or commercial use of any part of this repository is strictly prohibited.
