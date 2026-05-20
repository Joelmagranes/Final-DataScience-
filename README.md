# README — Factores del Rendimiento Académico
# Proyecto Final — Data Science 2 (Coderhouse)
## Objetivo:
Este proyecto busca predecir el puntaje final de un estudiante en un examen utilizando técnicas de Machine Learning. Se analizan variables conductuales, socioeconómicas y contextuales para identificar qué factores influyen más en el rendimiento académico.

## Dataset:
  6.607 estudiantes

  
  20 variables

  
  Target: Exam Score (0–100)

  
  Incluye información sobre horas de estudio, asistencia, ingresos familiares, educación de los padres, motivación, recursos escolares, entre otros.

## EDA — Principales hallazgos
Asistencia y Horas de Estudio son los predictores más fuertes del puntaje.


Horas de sueño y actividad física muestran correlación casi nula.


Se imputaron pocos valores nulos (<1.5%).

## Feature Engineering
Se generaron tres atributos clave:


Índice de Esfuerzo Académico


Índice Socioeconómico


Rendimiento Ajustado por Motivación


Además, se aplicó encoding y escalado estándar a las variables numéricas.

## Modelado

Se evaluaron varios modelos:

| Modelo           | R2 Test |
|------------------|---------|
| Ridge Regression | 0.607   |
| Elastic Net      | 0.606   |
| XGBoost          | 0.589   |
| Random Forest    | 0.535   |



## Modelo elegido: Ridge Regression
Mejor generalización


Simplicidad e interpretabilidad


Error relativo aproximado: 5%



## Conclusiones
Los datos permiten predecir el rendimiento académico con buena precisión.


Los hábitos del estudiante (asistencia, estudio) pesan más que el entorno socioeconómico.


El dataset presenta estructura lineal, por lo que modelos simples superan a los complejos.


El enfoque podría utilizarse para detectar alumnos en riesgo sin requerir datos sensibles.

## Archivos
Datascience2_Joel_Magranes.ipynb — Notebook principal
