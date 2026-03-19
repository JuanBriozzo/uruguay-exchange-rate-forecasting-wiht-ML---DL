# uruguay-exchange-rate-forecasting-wiht-ML-and-DL

## 🧠 Descripción del Proyecto

Este repositorio contiene el desarrollo completo de una tesis de Maestría en Ciencia de Datos enfocada en la predicción del tipo de cambio USD/UYU en Uruguay.

El proyecto combina enfoques tradicionales de econometría con modelos avanzados de Machine Learning y Deep Learning, utilizando una base de datos construida a partir de múltiples fuentes económicas, financieras y externas.

Se implementa un pipeline reproducible basado en notebooks que abarca desde la construcción de datos hasta la generación de predicciones en producción.

---

## 🎯 Objetivos

- Predecir el tipo de cambio USD/UYU en horizontes de:
  - 1 mes
  - 3 meses
  - 6 meses
  - 12 meses

- Comparar el desempeño de:
  - Modelos de Machine Learning
  - Modelos de Deep Learning
  - Benchmarks econométricos tradicionales:
    - Random Walk
    - RPPP (Relative Purchasing Power Parity)
    - CIRP (Covered Interest Rate Parity)
    - Encuestas del BCU

- Identificar variables relevantes que explican la dinámica del tipo de cambio.

- Construir un pipeline automatizado y reproducible para predicción económica.

---

## ⚙️ Metodología

El proyecto sigue un enfoque estructurado tipo pipeline:

1. *Construcción de la base de datos*
   - Integración de múltiples fuentes económicas y financieras.
   - Frecuencia diaria con transformaciones hacia horizontes de predicción.

2. *Ingeniería de variables*
   - Transformaciones (log-diferencias, rezagos, normalizaciones).
   - Generación de variables explicativas y targets forward-looking.

3. *Selección de variables*
   - Correlación por horizonte
   - Reducción de multicolinealidad
   - Evaluación de estabilidad entre horizontes

4. *Modelos benchmark*
   - Random Walk
   - RPPP
   - CIRP
   - Expectativas del BCU

5. *Modelos predictivos*
   - Machine Learning (ej: Random Forest, XGBoost, etc.)
   - Deep Learning (ej: LSTM, GRU, arquitecturas híbridas)

6. *Evaluación de resultados*
   - Métricas out-of-sample
   - Comparación entre modelos
   - Selección del mejor modelo por horizonte

7. *Producción*
   - Pipeline final para generación de predicciones

---

## 🗂️ Estructura del Repositorio


📁 Base_de_datos/
📁 Flujo/
📁 Produccion/


### 📁 Base_de_datos
Contiene la base consolidada y los inputs originales utilizados en el proyecto.

### 📁 Flujo
Pipeline completo del proyecto dividido en notebooks secuenciales.

### 📁 Produccion
Notebook final orientado a la generación de predicciones en un entorno productivo.

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

1. Clonar el repositorio:

```bash
git clone <repo-url>
cd <repo-name>

Instalar dependencias:

pip install -r requirements.txt

Ejecutar notebooks en orden:

Flujo/
N00 → N01 → N02 → N03 → N04 → N05 → N06

Ejecutar producción:

Produccion/N07_produccion.ipynb
