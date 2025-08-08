# challenge_telecomX_analisis_evasion_de_clientes_ONE_G8_Part2
Este proyecto tiene como objetivo analizar y predecir la pérdida de clientes (Churn) en la empresa Telecom X utilizando modelos de Machine Learning.  Se desarrollaron dos modelos principales: Regresión Logística y Random Forest, con el fin de comparar su desempeño y determinar cuál es más efectivo para la predicción.
Objetivos del Proyecto
Analizar datos históricos de clientes para identificar patrones asociados al Churn.

Entrenar y evaluar modelos de clasificación supervisada.

Comparar métricas clave de rendimiento entre los modelos.

Proporcionar conclusiones y recomendaciones para la empresa.

- Contenido del Proyecto
Exploración y limpieza de datos:

Análisis exploratorio (EDA).

Tratamiento de valores faltantes.

Codificación de variables categóricas.

Eliminación de variables que filtraban la respuesta (ej. Churn_No).

Entrenamiento de modelos:

Regresión Logística.

Random Forest.

Evaluación de modelos:

Accuracy.

Precision.

Recall.

F1-score.

Matriz de confusión.

Análisis crítico y conclusiones.

- Resultados de Evaluación
Regresión Logística
Accuracy: 0.85

Precision: 0.85

Recall: 0.85

F1-score: 0.85

Matriz de Confusión:


[[1332  221]
 [ 239 1313]]
Random Forest
Accuracy: 0.81

Precision: 0.82

Recall: 0.81

F1-score: 0.81

Matriz de Confusión:


[[1167  386]
 [ 193 1359]]

 
- Análisis Crítico
La Regresión Logística mostró un rendimiento más equilibrado entre precisión y recall para ambas clases, siendo más estable en la predicción.

El Random Forest presentó un mejor recall para clientes que abandonan (clase 1), pero sacrificó algo de precisión, lo que puede llevar a más falsos positivos.

Ninguno de los modelos mostró signos claros de overfitting en esta fase, ya que no se ajustaron hiperparámetros.

La eliminación de la variable Churn_No fue clave para evitar fuga de información (data leakage).

🏁 Conclusiones
La Regresión Logística es el modelo más balanceado y confiable en este caso, adecuado para una primera implementación.

El Random Forest podría superar a la regresión logística si se ajustan sus hiperparámetros (número de árboles, profundidad máxima, etc.).

Es recomendable realizar un ajuste de hiperparámetros y validación cruzada para ambos modelos antes de una implementación final.

El análisis permitió entender mejor las variables que impactan en la pérdida de clientes, lo que es clave para estrategias de retención.

- Tecnologías Utilizadas
Python 3.x

Pandas, NumPy

Scikit-learn

Matplotlib, Seaborn

Jupyter Notebook

- Próximos Pasos
Ajuste de hiperparámetros con GridSearchCV o RandomizedSearchCV.

