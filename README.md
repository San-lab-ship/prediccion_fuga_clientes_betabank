# Predicción de Fuga de Clientes – Beta Bank

Este proyecto de ciencia de datos busca predecir si un cliente del Beta Bank abandonará el servicio, utilizando datos históricos de comportamiento. El modelo ha sido entrenado y validado con métricas exigentes como F1 y AUC-ROC, superando el umbral mínimo requerido de 0.59 en F1-score. Además, se incluyen simulaciones, regresión lineal y visualizaciones interactivas para facilitar la comprensión del comportamiento del cliente.

## Metodología

-Análisis Exploratorio de Datos (EDA): revisión de la distribución de variables numéricas y categóricas, identificación de valores atípicos y análisis de correlaciones.

-Preprocesamiento de datos: imputación de valores faltantes, codificación de variables categóricas y escalado de variables numéricas.

-Entrenamiento de modelos: implementación de modelos de árbol de decisión y random forest, incluyendo validación cruzada y ajuste de hiperparámetros.

-Evaluación: uso de métricas como F1-score y AUC-ROC. También se incluyen ejemplos comparativos de métricas inadecuadas para clasificación como MAE y R².

-Simulación y visualización: creación de un conjunto de datos sintético para ilustrar el mal uso de métricas de regresión en clasificación. Visualizaciones interactivas con Plotly para facilitar la interpretación del modelo.


## Parámetros del Modelo

| Parámetro                        | Valor / Descripción                                                          |
| -------------------------------- | ---------------------------------------------------------------------------- |
| División de datos                | 60 % entrenamiento, 20 % validación, 20 % prueba                             |
| Random State                     | `12345` (para garantizar la reproducibilidad de resultados)                  |
| Métrica principal optimizada     | F1-score ≥ `0.59`                                                            |
| Criterio de selección del modelo | Mejor desempeño validado y capacidad de generalización sobre datos de prueba |


## Visualizaciones

-Curva ROC: muestra la sensibilidad frente a la tasa de falsos positivos

![image](https://github.com/user-attachments/assets/8f3f189e-21e5-4059-9db8-2101c9be8329)


-Matriz de Confusión Interactiva: análisis detallado por categoría

![image](https://github.com/user-attachments/assets/8c94b20c-eae9-4d91-a17a-0ae8cfae74ba)



https://san-lab-ship.github.io/prediccion_fuga_clientes_betabank/matriz_confusion.html

-Dispersión de Clases (Conjunto de Prueba)

![image](https://github.com/user-attachments/assets/bd2b1895-30e6-434e-8a0a-3785bfad0340)


## Tecnologías Utilizadas

✔️ Python 3.10 / 3.11
✔️ Pandas
✔️ NumPy
✔️ Scikit-learn
✔️ Plotly
✔️ Seaborn
✔️ Jupyter Notebook / Google Colab
✔️ Joblib
✔️ Draw.io (para arquitectura y flujos)
✔️ Streamlit (en desarrollo para versión web del modelo)


## Métricas Clave

| Métrica  | Valor                   | Observación                                                             |
| -------- | ----------------------- | ----------------------------------------------------------------------- |
| F1-score | ≥ 0.59 ✅               | Supera el umbral mínimo requerido                                       |
| AUC-ROC  | ✓ calculada             | Buen desempeño en discriminación de clases                              |
| R² y MAE | ✖️ (solo en simulación) | Usadas solo en un contexto ilustrativo para explicar su inaplicabilidad |


## Conclusión

Este proyecto demuestra un enfoque completo de ciencia de datos aplicado al sector financiero, desde el preprocesamiento hasta la evaluación crítica de métricas. A través de simulaciones y visualizaciones interactivas, se facilita la interpretación del modelo y sus limitaciones, destacando el valor de un análisis bien fundamentado. Esta base permite futuras extensiones hacia aplicaciones reales, dashboards interactivos o integraciones con plataformas de retención de clientes.

## Estructura del Proyecto
```
├── modelo_fuga_clientes.ipynb
├── simulacion_regresion_lineal.ipynb
├── graficas_interactivas.ipynb
├── README.md
├── requirements.txt
├── visuals/
│   ├── matriz_confusion.png
│   └── curva_roc.png
├── simulacion/
│   └── datos_regresion.csv
└── utils/
    └── funciones_metricas.py
