# Callenge-TelecomX_LATAM-alura
Este proyecto integró de manera práctica los conceptos de ETL y Análisis Exploratorio de Datos, permitiendo transformar datos crudos en información relevante para la toma de decisiones.

1. Extracción de Datos (E – ETL)
En esta etapa se realizó la obtención de los datos desde un archivo JSON alojado en un repositorio de GitHub.
* Se accedió al archivo mediante su URL en formato **RAW**, simulando el consumo de una API.
* Se utilizó la librería `requests` para realizar la solicitud HTTP.
* Los datos fueron recibidos en formato JSON y posteriormente normalizados utilizando `pandas.json_normalize`.
**Objetivo:**
Transformar los datos crudos provenientes de la API en un DataFrame estructurado, apto para su análisis.

2. Exploración Inicial de los Datos

Una vez cargados los datos:
* Se inspeccionó la estructura del DataFrame (`head`, `info`, `columns`).
* Se analizaron los tipos de datos y la presencia de valores nulos.
* Se identificaron columnas anidadas y variables que requerían transformación.
**Objetivo:**
Comprender la estructura del dataset antes de aplicar procesos de limpieza y transformación.

3. Transformación y Limpieza de Datos (T – ETL)

Durante esta etapa se realizaron las siguientes acciones:
* Normalización y renombrado de columnas para mejorar la legibilidad.
* Conversión de variables numéricas (`monthly_charges`, `total_charges`) que originalmente estaban en formato texto.
* Identificación y eliminación de registros con valores nulos en variables clave.
* Validación del dataset final para asegurar consistencia y calidad.
**Objetivo:**
Garantizar un conjunto de datos limpio, consistente y confiable para el análisis exploratorio.

4. Análisis Exploratorio de Datos (EDA)

Se realizó un análisis exploratorio con el fin de identificar patrones y relaciones entre las variables:
* Análisis de la distribución general de la evasión de clientes (`Churn`).
* Evaluación del churn en función del tipo de contrato.
* Análisis de la evasión según la antigüedad del cliente.
* Relación entre el gasto mensual y la probabilidad de evasión.
* Exploración del impacto de servicios contratados y métodos de pago.
Se utilizaron visualizaciones con `Matplotlib` y `Seaborn` para facilitar la interpretación de los resultados.
**Objetivo:**
Detectar factores relevantes asociados a la evasión de clientes.

5. Generación de Insights

A partir del EDA se identificaron los siguientes puntos clave:
* Los contratos mensuales presentan mayores tasas de evasión.
* Los clientes con menor antigüedad son más propensos a abandonar el servicio.
* Un mayor gasto mensual está asociado a una mayor probabilidad de churn.
* La combinación de estos factores sugiere oportunidades de mejora en las estrategias de fidelización.
**Objetivo:**
Extraer conclusiones accionables que sirvan de base para decisiones estratégicas y futuros modelos predictivos.

6. Conclusiones Finales

El análisis permitió comprender los principales factores que influyen en la evasión de clientes en Telecom X.
Los resultados obtenidos brindan información clave para el desarrollo de estrategias de retención y la construcción de modelos de predicción de churn.




