# ✈️ Predicción de Retrasos de Vuelos con Árboles de Decisión (PySpark)

## 📌 Descripción

Este proyecto tiene como objetivo predecir si un vuelo sufrirá un retraso utilizando un modelo de Árbol de Decisión en PySpark. Se realiza un análisis de datos de vuelos, aplicando preprocesamiento, transformación de datos y creación de un modelo supervisado. Todo el trabajo se lleva a cabo en Google Colab, utilizando el entorno distribuido de Apache Spark.

## 🧠 Algoritmo

- Árboles de Decisión (Decision Tree Classifier)

## 📁 Estructura del Proyecto

- `flights-larger.csv`: Dataset utilizado para el análisis
- `notebook.ipynb`: Notebook de Google Colab con todo el procesamiento y análisis.
- `README.md`: Descripción del proyecto.

## 🛠️ Herramientas y Tecnologías

- Python
- PySpark
- Google Colab
- Spark DataFrames

## ⚙️ Proceso de Desarrollo

1. **Carga del dataset:** Se usa Apache Spark para cargar un archivo CSV grande.
2. **Preprocesamiento:**
   - Eliminación de columnas innecesarias (`flight`).
   - Eliminación de filas con valores nulos.
   - Conversión de millas a kilómetros.
   - Creación de columna `label` (1 si el vuelo tiene un retraso de 15 min o más, 0 si no).
3. **Preparación del modelo:**
   - Selección de características.
   - Dividir el dataset en entrenamiento y prueba.
   - Entrenamiento del modelo de Árbol de Decisión.
4. **Evaluación del modelo:**
   - Matriz de confusión.
   - Métricas de evaluación como precisión, recall, F1-score.

## 📊 Ejemplo de columnas en el dataset

| mon | dom | dow | carrier | org | depart | duration | delay | km | label |
|-----|-----|-----|---------|-----|--------|----------|-------|----|-------|
| 10  | 10  |  1  | OO      | ORD | 8.18   | 51       | 27    | 252.7 | 1   |
|  2  | 14  |  5  | B6      | JFK | 21.17  | 365      | 60    | 3617.2 | 1   |



**Isaac Cueva**  
Estudiante de Ingeniería en Sistemas  
Pontificia Universidad Católica del Ecuador  

---


