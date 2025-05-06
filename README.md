# Proyecto Grado MIAD – Detección de Anomalías en Consumo de Gas

Este repositorio contiene el desarrollo del proyecto de grado para el curso de Proyecto Aplicado en Analítica de Datos (MIAD), centrado en la detección de anomalías en el consumo de gas en clientes de Contugas.

## Objetivo

Diseñar e implementar un prototipo de sistema de detección automática de anomalías que permita identificar comportamientos inusuales en series temporales de consumo de gas, temperatura y presión, utilizando modelos de machine learning con enfoque supervisado y no supervisado.

---

## Estructura del Repositorio

- `Fase1_notebook.zip`: Notebook correspondiente a la primera fase del proyecto, con pruebas exploratorias utilizando modelos clásicos no supervisados (Isolation Forest, LOF, One-Class SVM).
- `Fase2_notebook.ipynb`: Notebook con los modelos avanzados implementados en la segunda fase, incluyendo MLP con lags e LSTM Autoencoder, validación mediante inyección de anomalías artificiales y evaluación de desempeño con métricas estándar.

---

## Metodología

### Fase 1 – Exploración inicial

- Análisis exploratorio de las variables.
- Pruebas con modelos de detección no supervisados.
- Establecimiento de línea base.

### Fase 2 – Modelamiento avanzado

- Incorporación de dependencia temporal mediante generación de rezagos (lags).
- Entrenamiento de modelos MLP y LSTM con validación cruzada.
- Evaluación con F1-score, precision y recall.

---

## Resultados

- El modelo **MLP con lags** obtuvo un **F1-score promedio de 0.91**, siendo la opción más equilibrada en precisión y eficiencia computacional.
- El sistema es apto para ser integrado con dashboards operativos y sistemas de monitoreo en producción.

---

## Requisitos

- Python 3.8+
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, `scikit-learn`, `keras`, `tensorflow`

---

## Autores

Proyecto desarrollado por el equipo del curso MIAD 2025.

---

## Licencia

Uso académico únicamente.
