📊 Predicción de Cancelación de Clientes en Telecomunicaciones
🎯 Objetivo del Proyecto

El propósito de este proyecto es predecir la cancelación (churn) de clientes en una empresa de telecomunicaciones.
El análisis busca:

Identificar patrones de comportamiento de clientes que cancelan el servicio.

Evaluar las variables más influyentes en la predicción de cancelación.

Entrenar y comparar modelos de machine learning para determinar el más adecuado.

🛠️ Herramientas y Librerías Utilizadas

El proyecto fue desarrollado en Python utilizando principalmente:

Pandas → Manipulación y limpieza de datos.

NumPy → Operaciones numéricas y cálculos eficientes.

Matplotlib / Seaborn → Visualización de datos y gráficos exploratorios.

Scikit-learn (sklearn) → Preprocesamiento, modelos de machine learning y métricas.

Imbalanced-learn (imblearn) → Aplicación de SMOTE para balancear las clases.

Google Colab → Entorno de desarrollo en la nube.

ChatGPT (OpenAI) → Asistencia en la estructuración, explicación de conceptos y redacción de código.

📂 Estructura del Proyecto

Exploración y Preparación de Datos

Carga de dataset.

Limpieza y tratamiento de valores nulos.

Codificación de variables categóricas (OneHotEncoder).

Análisis exploratorio con visualizaciones.

Análisis de Correlaciones y Visualización

Matriz de correlación con la variable objetivo (churn).

Boxplots y scatterplots de variables clave (ej. gasto total, tiempo de contrato).

División de Datos y Balanceo

Separación en train/test con train_test_split.

Balanceo de clases con SMOTE aplicado únicamente en el conjunto de entrenamiento.

Entrenamiento de Modelos

Random Forest Classifier: Modelo basado en árboles con evaluación de importancia de variables.

Regresión Logística: Modelo lineal con análisis de coeficientes para interpretar el efecto de cada variable.

Evaluación de Modelos

Métricas utilizadas: Matriz de Confusión, Accuracy, Precision, Recall, F1-score.

Comparación visual de métricas entre modelos.

Análisis de Importancia de Variables

Random Forest: Importancia de características basada en la reducción de impureza.

Regresión Logística: Magnitud y signo de los coeficientes como medida de influencia en la predicción.

📈 Resultados Principales

Ambos modelos presentaron desempeños competitivos, con un balance razonable entre precisión y recall.

Las variables relacionadas con tipo de contrato, servicios adicionales (ej. fibra óptica, streaming) y gasto total fueron las más determinantes para la predicción de cancelación.

El uso de SMOTE permitió mejorar el recall en comparación con modelos entrenados en datos desbalanceados.

🤝 Reconocimientos

Este proyecto fue desarrollado con el acompañamiento y apoyo de ChatGPT (OpenAI), que sirvió como guía para:

Explicación de conceptos técnicos.

Desarrollo de fragmentos de código.

Revisión de métricas y resultados.

Apoyo en la redacción del README y conclusiones.

🚀 Próximos Pasos

Probar métricas adicionales como ROC-AUC y PR-AUC.

Evaluar modelos adicionales basados en distancia como KNN, aplicando estandarización.

Implementar optimización de hiperparámetros con GridSearchCV o RandomizedSearchCV.