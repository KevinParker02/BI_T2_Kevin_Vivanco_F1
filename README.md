# Análisis de Consistencia y Rendimiento en Fórmula 1 (1990–2020)

## 📘 Descripción general
Este proyecto analiza el desempeño de pilotos de Fórmula 1 durante el período **1990–2020**, con el objetivo de evaluar cómo la **consistencia en sus posiciones finales** influye en la **acumulación total de puntos por temporada**.  
Se aplican técnicas de **regresión lineal múltiple** y **agrupamiento (K-Means)** para validar la hipótesis y segmentar a los pilotos según su nivel de regularidad.  
El notebook está diseñado para ejecutarse completamente en **Google Colab**, utilizando datos públicos obtenidos desde Kaggle.

---

## 🧱 Estructura del notebook

El trabajo está dividido en **dos partes principales**, lo que facilita su ejecución y reutilización:

### 🔹 Parte 1 — EDA y limpieza de datos

**Entrada:** se deben ingresar 3 csv para empezar su depuración y normalización:
* `drivers.csv`
* `races.csv`
* `results.csv`

Posteriomente comienza:
- La exploración y entendimiento de los datos
- Filtrado de temporadas (1990–2020).  
- Normalización del sistema moderno de puntuación (post-2010).  
- Integración de resultados, carreras y pilotos en un dataset maestro.  
- Exportación del archivo limpio `f1_master_clean_1990_2020.csv`.

📤 **Salida:** se genera automáticamente el archivo  
`f1_master_clean_1990_2020.csv`, que puede descargarse y reutilizarse en la Parte 2.  

---

### 🔹 Parte 2 — Modelado y análisis predictivo
Esta sección puede ejecutarse **de forma independiente** cargando el dataset limpio exportado.  
Incluye:
- Análisis estadístico y correlacional de variables.  
- Modelos de **Regresión Lineal Múltiple, Ridge y Lasso**, con validación cruzada.  
- Evaluación con métricas (MAE, MSE, RMSE, R²).  
- Aplicación de **K-Means** para agrupar pilotos por consistencia y desempeño.  
- Visualizaciones comparativas y conclusiones orientadas a Business Intelligence.  

---
