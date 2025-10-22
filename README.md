# Megaline Plan Classifier — Smart vs Ultra

Clasificador que recomienda plan **Smart** o **Ultra** con datos de uso (`calls`, `minutes`, `messages`, `mb_used`).

## Resultados
- **Mejor modelo:** RandomForest
- **Accuracy (VALID):** ~0.80+
- **Accuracy (TEST):** ≥ 0.75 (umbral alcanzado)
- Sanity check: supera `Dummy(uniform)` y `Dummy(most_frequent)`
- Métricas + matriz de confusión incluidas en el notebook

## Datos
- Dataset: `/datasets/users_behavior.csv` (entorno TripleTen)
- Objetivo: `is_ultra` (1=Ultra, 0=Smart)

## Metodología
- Split **60/20/20** (train/valid/test) con `stratify`
- Modelos: Logistic Regression, Decision Tree, RandomForest, Dummy
- Métrica: `accuracy`

## Notebook
- [`Proyecto9_Megaline.ipynb`](./Proyecto9_Megaline.ipynb)

## Vista
- GitHub renderiza el `.ipynb` directo.
- **nbviewer (recomendado):**  
  https://nbviewer.org/github/christiansandovalgarcia01-creator/megaline-plan-classifier/blob/main/Proyecto9_Megaline.ipynb

## Ejecutar (opcional)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/christiansandovalgarcia01-creator/megaline-plan-classifier/blob/main/Proyecto9_Megaline.ipynb)

## Stack
Python · Pandas · scikit-learn · Matplotlib · Jupyter
