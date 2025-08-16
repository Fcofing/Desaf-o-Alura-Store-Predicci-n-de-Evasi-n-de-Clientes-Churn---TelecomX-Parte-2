# 🚀 Proyecto: Predicción de Evasión de Clientes (Churn) - TelecomX Parte 2

### 📝 Introducción

[cite_start]Este proyecto representa la segunda fase del desafío de **TelecomX**, donde he sido promovido al rol de **Analista de Machine Learning**[cite: 50]. [cite_start]El objetivo principal es ir más allá del análisis exploratorio inicial y construir **modelos predictivos** capaces de anticipar qué clientes tienen la mayor probabilidad de cancelar sus servicios[cite: 39].

### 🎯 Misión

[cite_start]Mi misión es desarrollar un *pipeline* robusto para el modelado predictivo, lo cual permitirá a la empresa adelantarse al problema de la evasión y tomar medidas proactivas de retención[cite: 40, 13].

### 🛠️ Objetivos del Desafío

[cite_start]Este proyecto aborda los siguientes objetivos, según las directrices proporcionadas[cite: 41]:

* [cite_start]**Preparación de Datos**: Tratar, codificar y normalizar los datos para que sean compatibles con los algoritmos de Machine Learning[cite: 42].
* [cite_start]**Análisis de Correlación**: Identificar relaciones entre las variables, prestando especial atención a su correlación con la evasión[cite: 43, 73].
* [cite_start]**Modelado Predictivo**: Entrenar al menos **dos modelos de clasificación** diferentes, uno que requiera normalización (ej. Regresión Logística) y otro que no (ej. Random Forest)[cite: 44, 84, 85, 86].
* [cite_start]**Evaluación de Modelos**: Medir el rendimiento de los modelos utilizando métricas clave como **Precisión, Recall, F1-score y la Matriz de Confusión**[cite: 45, 94].
* [cite_start]**Interpretación de Resultados**: Analizar e interpretar los resultados de los modelos, incluyendo la **importancia de las variables** para la predicción del `churn`[cite: 46, 107].
* [cite_start]**Conclusiones Estratégicas**: Entregar un informe con conclusiones claras y recomendaciones basadas en el análisis de los datos[cite: 47, 119].

### 📂 Estructura del Repositorio

* `TelecomX_LATAM.ipynb`: Cuaderno de Jupyter que contiene todo el código para la preparación de datos, entrenamiento de modelos, evaluación y el informe final.
* `TelecomX_Data.json`: El conjunto de datos original de los clientes.
* `TelecomX_diccionario.md`: El diccionario de datos que describe cada una de las variables.
* `Instrucciones.docx`: Documento con las directrices completas del desafío.
* `README.md`: Este archivo, que proporciona una visión general del proyecto.

### 📊 Metodología y Hallazgos Principales

1.  **Limpieza y Preprocesamiento**: Los datos se cargaron, se aplanó su estructura y se realizaron las limpiezas iniciales. [cite_start]Para el modelado, se eliminó la columna de identificación del cliente (`customerID`) y se codificaron las variables categóricas utilizando `OneHotEncoder`[cite: 55, 59, 60].
2.  [cite_start]**Modelado y Evaluación**: Se dividieron los datos en conjuntos de entrenamiento y prueba (80/20)[cite: 81]. Se entrenaron dos modelos: **Regresión Logística** y **Random Forest**. El modelo de **Random Forest** demostró un mejor rendimiento en la predicción del `churn`.
3.  **Factores Clave de Evasión**: El análisis de la importancia de las variables reveló que los factores más influyentes en la evasión son:
    * **Tipo de contrato**: Los contratos de mes a mes tienen una mayor correlación con la evasión.
    * **Antigüedad (`tenure`)**: Los clientes con menos tiempo en la empresa son más propensos a irse.
    * **Cargos mensuales**: Los gastos mensuales del cliente influyen significativamente en la decisión de cancelar.

### 💡 Conclusión Estratégica

La capacidad de predecir el `churn` es un activo valioso para TelecomX. Los modelos desarrollados permiten identificar a los clientes en riesgo y las variables que impulsan este comportamiento. Se recomienda a la empresa enfocar sus esfuerzos de retención en los clientes con contratos de corto plazo y en aquellos que llevan poco tiempo en el servicio, ofreciéndoles incentivos para fortalecer su compromiso a largo plazo.
