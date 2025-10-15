
# 🎬 MACHINE LEARNING: SISTEMAS DE RECOMENDACIÓN EN PYTHON

[![Python](https://img.shields.io/badge/Python-3670A0?style=flat&logo=python&logoColor=ffdd54)](https://www.python.org/)  
[![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)  
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)

Este proyecto se centra en la construcción desde cero de un **Sistema de Recomendación**. Utilizando un enfoque de **Filtro Colaborativo**, se desarrollan heurísticas y algoritmos para sugerir películas a un usuario, basándose en el comportamiento de otros usuarios con gustos similares (los "vecinos más próximos"). Es un ejemplo práctico y tangible de cómo plataformas como Netflix generan sugerencias personalizadas.

---

## 🧠 Contenido del Proyecto

### 1️⃣ Conceptos Fundamentales
- **Heurísticas de Recomendación:** Se establecen las bases lógicas sobre cómo funcionan estos sistemas, haciendo una analogía con plataformas populares de *streaming*.
- **Filtro Colaborativo:** El sistema se basa en la colaboración de los usuarios, analizando el perfil del usuario de referencia (lo que ya ha visto) y el comportamiento de otros usuarios.

### 2️⃣ Dataset y Preliminares
- **Dataset:** Se utilizan datos de **MovieLens**, una organización que recopila valoraciones de usuarios sobre películas, lo que es ideal para este tipo de algoritmos.
- **Construcción de la Matriz Usuario-Ítem:** Se requiere preparar la matriz de datos donde cada fila representa un usuario y cada columna una película, con las celdas conteniendo la valoración dada.

### 3️⃣ Desarrollo del Algoritmo KNN
El corazón del proyecto es la implementación de un algoritmo para identificar similitudes:

- **Identificación de Similitud:** El objetivo es encontrar a los **vecinos más cercanos (K-Nearest Neighbors o KNN)** al usuario de referencia.
- **Cálculo de Distancia:** Se utilizan métricas (generalmente la **Distancia Coseno** o **Distancia Euclidiana** en la práctica) para cuantificar qué tan similares son las valoraciones de otros usuarios en comparación con el usuario de referencia.

### 4️⃣ Refinamiento del Sistema de Sugerencias
La sugerencia final pasa por varias etapas de refinación para mejorar la calidad y relevancia:

1.  **Películas Vistas:** Capturar las películas vistas por los **K** vecinos más próximos.
2.  **Descarte por Valoraciones Bajas:** Descartar películas que tengan **menos de 50 valoraciones o votos** para asegurar la popularidad y relevancia en el subgrupo.
3.  **Media de Notas:** Calcular la media de las notas de las películas restantes.
4.  **Sugerencia Final:** Recomendar las **10 películas** con la mayor media de notas que el usuario de referencia aún no ha visto.

---

## 🛠️ Librerías Utilizadas

| Librería | Uso principal |
|:---:|:---:|
| **Pandas** | Carga, manipulación y preparación de los datos de MovieLens |
| **NumPy** | Operaciones numéricas y cálculo de distancias (inferido) |
| **Scikit-learn** | Implementación del algoritmo **K-Nearest Neighbors (KNN)** (inferido/adaptado para filtro colaborativo) |

---

## 🎯 Objetivo del Proyecto
Proporcionar una comprensión práctica y profunda de la lógica que subyace a los **Sistemas de Recomendación**. El proyecto guía al usuario a través del proceso de **transformación de datos de valoraciones** en una matriz utilizable y cómo aplicar **KNN** para identificar similitudes entre usuarios y generar sugerencias de alto valor.

---

## 📈 Resultados Clave
- **Algoritmo KNN Implementado:** Se construye un algoritmo para identificar a los **10 vecinos más próximos** (usuarios con gustos similares) del usuario de referencia.
- **Sugerencias Refinadas:** Se llega a una versión final de la función de sugerencias que considera **popularidad y votos suficientes**, logrando recomendaciones de alta calidad y relevancia.
- **Recomendación Final:** Se genera una lista de **10 películas** recomendadas al usuario, basada en el comportamiento colectivo y con un alto potencial de ser del agrado del usuario.
