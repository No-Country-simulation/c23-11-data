DESCRIPCIÓN
Este proyecto es parte de una simulación laboral de Not Country. Se empleó un dataset que posee más de 6.3 millones de transacciones bancarias simuladas. Nuestro objetivo es desarrollar un modelo predictivo robusto para detección de fraude usando técnicas de machine learning.
El análisis y construcción del modelo se realizó en tableau y python.


OBJETIVOS DEL PROYECTO:
Crear un modelo predictivo que detecte transacciones fraudulentas para lograr reducir pérdidas económicas y proteger a los clientes.
Crear un dashboard accesible para que los analistas y/o el equipo de seguridad monitoreen de manera continua y en tiempo real las transacciones 


CARACTERÍSTICAS PRINCIPALES:
Fuente de datos: Financial Fraud Detection Dataset
Cantidad de registros: 6 362 620
Cantidad de variables: 11
Tipos de datos: 
Variable	         Tipo de Dato
step	                        int64
type	                      object
amount	           float64
nameOrig	           object
oldbalanceOrg	float64
newbalanceOrig	float64
nameDest	           object
oldbalanceDest	float64
newbalanceDest	float64


PROBLEMAS IDENTIFICADOS
Outliers: Se han identificado varios outliers en las columnas numéricas, como amount, oldbalanceOrg, newbalanceOrig, oldbalanceDest, y newbalanceDest. Estos valores extremos pueden afectar la precisión de los modelos predictivos y requieren un tratamiento adecuado.


ESTRUCTURA DEL PROYECTO:


DATASET
Origen: Kaggle Dataset
Tamaño: Más de 6.3 millones de registros.


DICCIONARIO DE DATOS
step: Unidad de tiempo (1 paso = 1 hora, total de 744 pasos).
type: Tipo de transacción (CASH-IN, CASH-OUT, DEBIT, PAYMENT, TRANSFER).
amount: Monto de la transacción.
nameOrig: Cliente que inició la transacción.
oldbalanceOrg: Saldo inicial antes de la transacción.
newbalanceOrig: Saldo final después de la transacción.
nameDest: Cliente receptor de la transacción.
oldbalanceDest: Saldo inicial del receptor antes de la transacción.
newbalanceDest: Saldo final del receptor después de la transacción.
isFraud: Identifica si la transacción es fraudulenta (1) o no (0).
isFlaggedFraud: Marca intentos ilegales de transferir más de 200,000 en una transacción.
VARIABLES OBJETIVO
isFraud 
isFlaggedFraud


TECNOLOGÍAS
Google Colab 
Python
Librerías:
Pandas
Seaborn
Scikit-learn
Matplotlib
Sklearn
Tableau


EJECUCIÓN DEL PROYECTO
1. Copia el link de git https://github.com/No-Country-simulation/c23-11-data
2. Navega al directorio donde quieres alojar el proyecto  
3. Doble click y abrir con la terminal
4. colocar git clone https://github.com/No-Country-simulation/c23-11-data
5. Desde el IDE de tu preferencia abre el proyecto y ejecútalo
5. Carga un archivo .csv comprimido en formato .zip desde la página web para obtener predicciones en tiempo real.

PASOS DESARROLLADOS
Exploración de Datos
El dataset contiene 6,362,620 transacciones.
Donde solo el 0.13% de las transacciones son fraudulentas.
Tipo de transacciones más comunes: CASH-IN y CASH-OUT.
Modelos
Se probaron los siguientes modelos:
Logistic Regression
Decision Tree
Random Forest
Resultados principales :
1. Logistic Regression
Accuracy: 0.9988
Precision: 0.9988
Recall: 0.9988
F1 Score: 0.9988
2. Decision Tree
Accuracy: 0.9997
Precision: 0.9997
Recall: 0.9997
F1 Score: 0.9997
3. Random Forest
Accuracy: 0.9997
Precision: 0.9997
Recall: 0.9997
F1 Score: 0.9997
RESULTADOS
Random Forest tiene el mejor desempeño con respecto a los demás modelos.
