# 📊 Machine Learning: Sistemas de Recomendación en Python

[![Python](https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54)](https://www.python.org/)  
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)  
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)  
[![Surprise](https://img.shields.io/badge/Surprise-Library-blue?style=flat)](http://surpriselib.com/)  
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=matplotlib&logoColor=white)](https://matplotlib.org/)  
[![Seaborn](https://img.shields.io/badge/Seaborn-0099CC?style=flat&logo=seaborn&logoColor=white)](https://seaborn.pydata.org/)

Este proyecto se centra en el **desarrollo y evaluación de sistemas de recomendación** aplicando enfoques de **filtrado colaborativo** y métricas específicas para analizar su rendimiento y efectividad.

---

## 🧠 Contenido del Proyecto

### 1️⃣ Preparación de Datos
- Carga y limpieza de datos de usuarios, ítems y valoraciones  
- Creación de la **matriz usuario-ítem**  
- División de datos en conjuntos de entrenamiento y prueba  

### 2️⃣ Entrenamiento de Modelos
- Implementación de algoritmos de recomendación:  
  - **Filtrado colaborativo basado en usuarios**  
  - **Filtrado colaborativo basado en ítems**  
- Cálculo de **similitudes** (coseno, correlación, distancia euclidiana, etc.)

### 3️⃣ Optimización de Parámetros
- Selección del número óptimo de vecinos (*k*)  
- Comparación de distintas métricas de similitud  
- Evaluación de configuraciones para mejorar la precisión de las recomendaciones  

### 4️⃣ Evaluación del Sistema
- Cálculo de métricas de rendimiento, incluyendo:  
  - **RMSE (Root Mean Squared Error)**  
  - **MAE (Mean Absolute Error)**  
  - **Precision@K**  
  - **Recall@K**  
  - **NDCG (Normalized Discounted Cumulative Gain)**  
- Análisis comparativo del rendimiento entre diferentes configuraciones de modelos  

---

## 🛠️ Librerías Utilizadas

| Librería       | Uso principal                               |
|----------------|---------------------------------------------|
| **NumPy**      | Cálculos numéricos y manipulación de arrays |
| **Pandas**     | Manipulación y análisis de datos tabulares  |
| **Scikit-learn** | Implementación de métricas y evaluación de modelos |
| **Surprise**   | Modelado de sistemas de recomendación       |
| **Matplotlib** | Creación de gráficos estáticos              |
| **Seaborn**    | Visualización de datos y análisis exploratorio |

---

## 🎯 Objetivo del Proyecto
Aplicar técnicas de **sistemas de recomendación** para mejorar la personalización y calidad de las sugerencias hacia los usuarios, optimizando los parámetros de los modelos y evaluando su desempeño mediante métricas especializadas.

---

## 📈 Resultados Esperados
- Identificación de los **parámetros óptimos** para los sistemas de recomendación  
- Mejora en la **precisión y relevancia** de las recomendaciones generadas  
- **Visualización clara** de las métricas de evaluación y comparación de modelos  

---

