# XGBoost para Análisis de Sentimiento (PLN)

Proyecto de clasificación de texto aplicado a reseñas de películas (IMDB), utilizando **XGBoost** sobre una representación documento-término, con el objetivo de predecir el sentimiento (positivo / negativo).

El trabajo cubre todo el pipeline de Procesamiento del Lenguaje Natural (PLN), desde la limpieza del texto hasta la evaluación del modelo.

---

## Contenido del proyecto

- Limpieza y normalización del corpus textual
- Eliminación de stopwords estándar y personalizadas
- Visualización mediante nubes de palabras
- Construcción de una matriz documento-término (DTM)
- Reducción de dimensionalidad por frecuencia mínima
- Entrenamiento de un clasificador **XGBoost**
- Búsqueda de hiperparámetros con validación cruzada
- Evaluación en conjunto de prueba independiente
- Análisis de importancia de términos

---

## Metodología

- Representación textual basada en **recuentos de términos**
- Modelo de boosting de árboles (XGBoost)
- Optimización mediante **5-fold Cross-Validation**
- Métrica principal: **logarithmic loss (mlogloss)**
- Evaluación final con matriz de confusión y accuracy

---

## Resultados principales

- Accuracy en test ≈ **80%**
- Buen equilibrio entre falsos positivos y falsos negativos
- Las palabras con mayor importancia presentan carga semántica claramente positiva o negativa (e.g. *best*, *worst*, *bad*, *waste*)
- El modelo muestra buena capacidad de generalización sin signos claros de sobreajuste

---

## Tecnologías utilizadas

- **R**
- PLN: `tm`, `wordcloud`
- Modelado: `xgboost`, `caret`
- Manipulación de datos: `dplyr`
- Matrices dispersas: `Matrix`

---

## Autora

**Lucía Muñiz Presno**  
Grado en Estadística y Empresa  
Intereses: Data Science, Machine Learning, PLN, Big Data
