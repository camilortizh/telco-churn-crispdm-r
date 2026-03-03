# Telco Churn Prediction (AUC) — ML in R
*Churn modeling for a Telco CRM/Kaggle-style challenge: clean → engineer → train → validate → compare models (R).*

## Project summary
This project builds and evaluates binary classification models to predict **customer churn** for a telecom operator, using **AUC-ROC** as the main evaluation metric. The repository focuses on experimentation in R: data preparation, feature engineering, model training, validation, and comparison across approaches.

> **Important scope note:** This repo **does not include** the complete Kaggle submission pipeline. The final submission was performed in a separate notebook because it depended on importing an Excel file and preparing a specific output format; the final score was only validated at upload time. This repository documents the training + validation workflow and the rationale behind the chosen modeling approach.

---

## Problem description (Kaggle / business context)
Cellphone communications markets are typically saturated and highly competitive, often with only a few operators. Retention becomes critical because acquiring a new customer can be substantially more expensive than retaining an existing one, and churn rates are commonly tracked monthly. Under a CRM/analytics perspective, two key efforts are:
1) **Predict churn** accurately.
2) Define the most **cost-effective retention strategy** (including the option of doing nothing).

A telecom operator hires you to address both:
- **Part 1:** Produce the best possible churn prediction for a Kaggle-style test set, evaluated via **AUC-ROC**.
- **Part 2:** Deliver a CRISP-DM methodology report (max 12 pages) and propose a retention strategy (cutoffs, costs, and potential gains).

**Data context**
- Training data is a simple random sample of customers with churn outcomes from the last six months.
- Usage variables represent the last six months of customer activity.
- All customers are postpaid subscribers.
- Test data is an additional non-random sample; the churn label is not provided.

---

## What this repository covers (and what it doesn’t)
### Included here
- Data cleaning and type handling (e.g., dates)
- Feature engineering
- Train/test split and (optional) cross-validation
- Model training and comparison in R
- Evaluation with AUC-ROC (and threshold-based metrics)

### Not included here
- The **full Kaggle submission pipeline** (final notebook + last-mile formatting and upload-only validation)
# Predicción de Churn Telco (AUC) — ML en R
*Modelado de churn para un reto tipo Kaggle/CRM: limpiar → crear features → entrenar → validar → comparar modelos (R).*

## Resumen del proyecto
Este proyecto construye y evalúa modelos de clasificación binaria para predecir la **deserción (churn)** de clientes de un operador de telecomunicaciones, utilizando **AUC-ROC** como métrica principal de evaluación. El repositorio se enfoca en la experimentación en R: preparación de datos, *feature engineering*, entrenamiento de modelos, validación y comparación de enfoques.

> **Nota importante de alcance:** Este repositorio **no incluye** el pipeline completo de *Kaggle submission*. La *submission* final se realizó en un cuaderno/notebook aparte porque dependía de importar un Excel y preparar los datos en un formato específico; el desempeño final solo se validaba al momento de subirlo a Kaggle. Este repositorio documenta el flujo de entrenamiento + validación y el sustento del enfoque de modelado elegido.

---

## Descripción del problema (Kaggle / contexto de negocio)
Los mercados de comunicaciones por teléfono celular suelen estar saturados y ser altamente competitivos, muchas veces con pocos operadores. Por ello, la **retención** se vuelve crítica, ya que adquirir un nuevo cliente puede ser sustancialmente más costoso que retener uno existente, y las tasas de deserción suelen monitorearse mensualmente. Desde una perspectiva de CRM/analítica, hay dos esfuerzos clave:
1) **Predecir el churn** con precisión.
2) Definir la estrategia de **retención más costo-efectiva** (incluyendo la opción de no hacer nada).

Un operador de telecomunicaciones los contrata para abordar ambas necesidades:
- **Parte 1:** Producir la mejor predicción posible de churn para un set de prueba tipo Kaggle, evaluado mediante **AUC-ROC**.
- **Parte 2:** Entregar un reporte metodológico tipo CRISP-DM (máx. 12 páginas) y proponer una estrategia de retención (puntos de corte, costos y posibles ganancias).

**Contexto de datos**
- La base de entrenamiento es una muestra aleatoria simple de clientes con resultados de churn de los últimos seis meses.
- Las variables de consumo representan los últimos seis meses de actividad del cliente.
- Todos los clientes son pospago (suscripción).
- La base de prueba es una muestra adicional no aleatoria; la etiqueta de churn no está incluida.

---

## Qué cubre este repositorio (y qué no)
### Incluido aquí
- Limpieza de datos y manejo de tipos (p. ej., fechas)
- *Feature engineering*
- Split train/test y (opcional) validación cruzada
- Entrenamiento y comparación de modelos en R
- Evaluación con AUC-ROC (y métricas por umbral)

### No incluido aquí
- El pipeline completo de **Kaggle submission** (notebook final + formato “última milla” y validación solo al subir)
