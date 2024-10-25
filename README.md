# Análisis y Predicción de Graduados Estudiantiles.

Este proyecto surge a partir de un trabajo académico en el cual se nos encomendó utilizar diversos modelos de machine learning para predecir si los estudiantes universitarios completarían o no su carrera. El objetivo principal fue medir la perfomance al utilizar multiples modelos para lidiar con el objetivo.

## Descripción del Proyecto

Este análisis se enfoca en aplicar múltiples algoritmos de machine learning para predecir la **deserción estudiantil** en universidades. Se implementaron diversas técnicas para asegurar la robustez de los modelos, incluyendo partición en conjuntos de **entrenamiento y prueba**, así como el uso de **validación cruzada** para la optimización de hiperparámetros.

Se utilizaron diferentes métricas para evaluar el desempeño de los modelos, tanto en los datos de entrenamiento como en los de prueba, junto con **curvas de complejidad** y **técnicas de optimización**. Esto permitió una evaluación precisa y detallada del rendimiento de cada modelo.

## Modelos y Resultados

- Para la predicción del **target binario** (si un estudiante completará la carrera o no), el mejor rendimiento se obtuvo con el modelo de **Regresión Logística**.
- Para la predicción de variables **multiclase** (tipos de abandono o deserción), el modelo más efectivo fue el **Árbol de Decisión**.
- Además, se implementaron técnicas de **ensamble** utilizando modelos como **AdaBoost** y **Bagging KNeighborsClassifier** lo que mejoró significativamente el rendimiento para algunos casos.

## Análisis del Conjunto de Datos

El proyecto se basó en un conjunto de datos proporcionado, el cual fue sometido a un exhaustivo **análisis exploratorio** y **preprocesamiento** antes de aplicar los modelos de machine learning. Se utilizaron técnicas como **One-Hot Encoding** para tratar las variables categóricas y **StratifiedKFold** para asegurar una correcta partición de los datos durante la validación.

## Métricas de Evaluación

Las métricas empleadas para evaluar el rendimiento de los modelos fueron:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**
- **ROC AUC**
- **Log Loss**

Estas métricas permitieron evaluar de manera integral el desempeño de los modelos, asegurando que no solo se maximice la precisión, sino también otros aspectos importantes como la capacidad del modelo para manejar desequilibrios en los datos.

## Técnicas y Algoritmos Utilizados

- **Validación Cruzada**: Se utilizó validación cruzada con **StratifiedKFold** (5 folds) para garantizar una correcta segmentación de los datos de entrenamiento.
- **One-Hot Encoding**: Para variables categóricas con más de dos niveles.
- **Algoritmos**: Se utilizaron modelos como **Regresión Logística**, **Support Vector Machine (SVM)**, **Árboles de Decisión (CART)**, y **K-Nearest Neighbours (KNN)** para la predicción de variables binarias y multiclase.
- **Clasificación Multiclase**: Se implementaron **OneVsRestClassifier (OVRC)** y **OneVsOneClassifier (OVOC)** para problemas de clasificación multiclase.
- **Técnicas de Ensamble**: Se aplicaron modelos de ensamble con **Bagging** (ensamble-KNN) y **Boosting** (AdaBoost).
