# Telecom-X-Alura-#2


Proyecto: Predicción de Cancelación de Clientes en Telecomunicaciones

Descripción
Este proyecto analiza un conjunto de datos de clientes de una empresa de telecomunicaciones con el objetivo de predecir la cancelación de clientes (Churn).

Se aplicaron técnicas de análisis exploratorio de datos (EDA), balanceo de clases, normalización y modelado predictivo usando diferentes algoritmos de Aprendizaje

Flujo de trabajo
Carga y exploración de datos

Identificación de variables relevantes.
Limpieza de datos y tratamiento de valores nulos.
Análisis exploratorio (EDA)

Visualización de la relación entre variables como contrato, método de pago, antigüedad y tipo de servicio con la cancelación.
Identificación de correlaciones más fuertes con churn.
Preparación de los datos

Creación de dos datasets:
df_lineal: normalizado (para modelos sensibles a la escala).
df_arbol: sin normalizar (para árboles de decisión y Random Forest).
Balanceo de clases con SMOTE.
Modelado

Modelo 1: Regresión Logística (df_lineal normalizado)
Buen recall en clientes que cancelan, aunque menor precisión.

Modelo 2: Random Forest (df_arbol sin normalizar)
Resultados más balanceados entre precisión y recall.

Evaluación de modelos

Se compararon métricas de Exactitud, Precisión, Recall, F1-score y Matriz de Confusión.
Se identificó que Random Forest tuvo mejor desempeño general.

Principales hallazgos

Los factores más relevantes para la cancelación de clientes fueron:
Tipo de contrato (mayor cancelación en contratos mensuales).
Método de pago (Electronic Check asociado a mayor churn).
Servicio de internet (Fiber Optic asociado a más cancelaciones).
Antigüedad del cliente (clientes nuevos tienen mayor probabilidad de cancelar).

Estrategias de retención propuestas

Incentivar contratos de mayor duración (ofrecer descuentos por contratos anuales o bianuales).
Optimizar la experiencia de clientes con fibra óptica (mejor soporte técnico y estabilidad).
Revisar políticas de pago electrónico (mayor seguridad, facilidad y transparencia en facturación).
Programas de fidelización para clientes nuevos durante los primeros meses de contrato.


