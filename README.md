# Predicci-n-de-Incumplimiento-de-Pago
Predicción de Incumplimiento de Pago de Tarjeta de Crédito


Dataset: kaagle ()incluido.
Metodología: Pasos para realizar un analicis predictivo (EDA, preprocesamiento, modelado, evaluación).
Modelos Utilizados: Modelo de Regresión Logística,Modelo de Random Forest.
Resultados Clave: 1. Desequilibrio de Clases: Un Desafío Central
Una de las primeras y más importantes observaciones es el desequilibrio significativo en la variable objetivo ('default'). La gran mayoría de los clientes no incumplen sus pagos, mientras que la proporción de clientes que sí lo hacen es considerablemente menor. Este desequilibrio es típico en problemas de detección de fraude o riesgo, y impacta directamente en la elección de las métricas de evaluación. La precisión (accuracy) por sí sola puede ser engañosa, ya que un modelo que simplemente predice "no incumplimiento" para todos podría alcanzar una alta precisión sin ser útil. Por ello, el ROC AUC, el F1-score, la precisión y el recall para la clase minoritaria (incumplidores) se vuelven métricas mucho más relevantes.

2. El Historial de Pagos es Clave
Nuestra exploración de datos y, presumiblemente, la importancia de las características en los modelos de ensamble (como Random Forest y XGBoost), destacan que las variables relacionadas con el historial de pagos (PAY_0 a PAY_6) son los predictores más influyentes. Esto tiene sentido intuitivo: la forma en que un cliente ha pagado sus deudas en el pasado es un fuerte indicador de su comportamiento futuro. Retrasos consistentes o grandes montos adeudados se correlacionan fuertemente con el incumplimiento.

3. Modelos de Ensamble Superan a los Lineales
Los modelos de ensamble como Random Forest y XGBoost consistentemente superaron a modelos lineales como la Regresión Logística en la predicción del incumplimiento. Esto se atribuye a su capacidad para capturar relaciones no lineales y complejas entre las características y la variable objetivo, así como para manejar mejor la dimensionalidad de los datos. En particular, suelen ofrecer un mejor balance entre precisión y recall para la clase minoritaria, lo que se refleja en un mayor ROC AUC.


Conclusiones e Ideas Futuras: Nuestra exploración de datos y, presumiblemente, la importancia de las características en los modelos de ensamble (como Random Forest y XGBoost), destacan que las variables relacionadas con el historial de pagos (PAY_0 a PAY_6) son los predictores más influyentes. Esto tiene sentido intuitivo: la forma en que un cliente ha pagado sus deudas en el pasado es un fuerte indicador de su comportamiento futuro. Retrasos consistentes o grandes montos adeudados se correlacionan fuertemente con el incumplimiento.

Instrucciones para Ejecutar: el modelo incluye el set de datos para ser implementado el google colab.
