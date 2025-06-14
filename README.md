#  Predicción de Fuga de Clientes – Beta Bank

Este proyecto de ciencia de datos busca predecir si un cliente del Beta Bank abandonará el servicio, utilizando datos históricos de comportamiento. El modelo ha sido entrenado y validado con métricas exigentes como F1 y AUC-ROC, superando el umbral mínimo requerido de 0.59 en F1-score. Además, se incluyen simulaciones, regresión lineal y visualizaciones interactivas para facilitar la comprensión del comportamiento del cliente.

---

##  Archivos del Proyecto

###  1. `modelo_fuga_clientes.ipynb`
Notebook principal que incluye:

- ✅ Preprocesamiento de Datos  
- ✅ División en conjunto de entrenamiento, validación y prueba  
- ✅ Entrenamiento de varios modelos (DecisionTree, RandomForest, etc.)  
- ✅ Evaluación con F1-score y AUC-ROC  
- ✅ Prueba final del mejor modelo  
- ✅ Gráficas (matriz de confusión, curva ROC, etc.)

### 2. `simulacion_regresion_lineal.ipynb`
Simulación complementaria de datos usando regresión lineal para demostrar por qué métricas como R² y MAE no son adecuadas en un problema de clasificación.

- R² Score inapropiado  
- MAE solo para regresión

### 3. `graficas_interactivas.ipynb`
Visualizaciones interactivas con Plotly:

- Probabilidad de deserción por cliente (gráfico de dispersión)  
- Matriz de confusión con hover  



[Ver gráfica interactiva en GitHub Pages](https://san-lab-ship.github.io/prediccion_fuga_clientes_betabank/)

https://san-lab-ship.github.io/prediccion_fuga_clientes_betabank/matriz_confusion.html

---

## 🛠️ Herramientas Utilizadas

- Python 3.11  
- Pandas, Numpy  
- Scikit-learn  
- Plotly  
- Seaborn  
- Google Colab  
- Streamlit (en desarrollo)

---

## 📌 Métricas Clave

| Métrica     | Valor     |
|-------------|-----------|
| F1-score    | ≥ 0.59 ✅ |
| AUC-ROC     | ✓ calculada |
| R² y EAM    | ✖️ Simulación (no aplican: son datos de clasificación*) |

*Este código te permite entender y evaluar las métricas R² y MAE en un contexto de regresión, utilizando datos simulados para ilustrar

---

##  Autora 
San-lab-ship (2025)

---

## Comentarios Finales

Este proyecto demuestra un enfoque integral de ciencia de datos, desde el preprocesamiento hasta la visualización y reflexión crítica sobre métricas. Es una excelente base para extender a aplicaciones reales o dashboards en producción.
