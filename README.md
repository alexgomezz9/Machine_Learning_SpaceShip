# 🚀 Machine_Learning_SpaceShip

Este repositorio contiene el trabajo realizado para la competencia de **Spaceship Titanic** en Kaggle. El objetivo es predecir si los pasajeros fueron **transportados a otra dimensión** usando un conjunto de datos de características de los pasajeros, como su edad, gastos a bordo, destino y otras variables. Se han utilizado diferentes modelos de aprendizaje automático para abordar este problema de clasificación, y finalmente se ha optimizado un modelo de **Gradient Boosting** con los mejores hiperparámetros encontrados.

## 📄 Tabla de contenidos
1. [Descripción del Proyecto](#descripción-del-proyecto)
2. [Modelos Utilizados](#modelos-utilizados)
3. [Evaluación](#evaluación)
4. [Predicciones Finales](#predicciones-finales)
5. [Contribuciones](#contribuciones)
6. [Licencia](#licencia)

## 📚 Descripción del Proyecto
Este proyecto busca predecir si los pasajeros a bordo del **Spaceship Titanic** fueron transportados a otra dimensión. Para lograrlo, hemos procesado y analizado un conjunto de datos que contiene información sobre los pasajeros y su experiencia en el viaje. Los principales pasos incluyen:

- Limpieza de datos (gestión de valores nulos y codificación de variables categóricas).
- Ingeniería de características (creación de nuevas variables como el tamaño del grupo).
- Entrenamiento de diferentes modelos de clasificación.
- Optimización del mejor modelo utilizando **RandomizedSearchCV**.
- Visualización de los resultados mediante curvas de aprendizaje, matriz de confusión y gráficas de importancia de características.

## 🤖 Modelos Utilizados
Probamos varios modelos de clasificación para abordar el problema de predicción binaria:

- **Random Forest**: Un modelo de ensamble basado en múltiples árboles de decisión.
- **Gradient Boosting** (Mejor Modelo): Un modelo de boosting que mejora secuencialmente para minimizar los errores de los modelos anteriores.
- **Regresión Logística**: Un modelo lineal utilizado para clasificación.
- **Support Vector Classifier (SVC)**: Un modelo de clasificación que maximiza los márgenes entre clases.
- **K-Nearest Neighbors (KNN)**: Un modelo basado en la proximidad a los vecinos más cercanos.

Utilizamos **RandomizedSearchCV** para optimizar los hiperparámetros del modelo de **Gradient Boosting**, que resultó ser el modelo con mejor rendimiento en términos de precisión.

## 📊 Evaluación
El modelo fue evaluado usando **5-Fold Cross-Validation** y las siguientes métricas:

- **Precisión (Accuracy)**: El modelo final alcanzó una precisión de **80.33%** durante la validación cruzada.
- **Curva ROC**: El área bajo la curva (AUC) fue **0.8935**, indicando un buen rendimiento general.
- **Matriz de Confusión**: Proporciona una visión clara de las predicciones correctas e incorrectas para las clases de "transportado" y "no transportado".

![Curva ROC](ruta/a/imagen_roc.png)  
![Importancia de Características](ruta/a/imagen_importancia.png)  
![Matriz de Confusión](ruta/a/imagen_confusion.png)

## 📈 Predicciones Finales
Las predicciones finales para los pasajeros del conjunto de test se generaron utilizando el modelo **Gradient Boosting** optimizado.

## 📄 Licencia
Este proyecto está licenciado bajo la Licencia MIT. Consulta el archivo [LICENSE](LICENSE) para más detalles.
