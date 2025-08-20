Informe Final del Análisis de Evasión de Clientes (Churn)
Introducción
El objetivo de este análisis es comprender los factores que contribuyen a la evasión de clientes en Telecom X. La empresa enfrenta una alta tasa de cancelaciones y, mediante el análisis exploratorio de datos, buscamos identificar patrones y obtener insights que ayuden a reducir el 'churn'.

Limpieza y Tratamiento de Datos
Extracción: Se cargaron los datos directamente desde una API pública en formato JSON y se convirtieron a un DataFrame de Pandas.

Normalización: Se normalizaron las columnas anidadas ('customer', 'phone', 'internet', 'account') para crear una estructura de DataFrame plana y más fácil de analizar.

Inconsistencias: Se identificaron y trataron los valores ausentes y los formatos incorrectos en la columna 'Charges.Total', convirtiéndolos a tipo numérico y rellenando los valores faltantes con cero.

Nuevas Variables: Se creó la columna 'Cuentas_Diarias' a partir de 'Charges.Total' y 'tenure' para obtener una visión más detallada del gasto diario.

Análisis Exploratorio de Datos (EDA)
Distribución de Evasión: El análisis inicial mostró la proporción de clientes que se han dado de baja, proporcionando una base para el estudio.

Variables Categóricas: Los gráficos por variables como 'Contract' y 'PaymentMethod' revelaron que los clientes con contratos mensuales y ciertos métodos de pago tienen una mayor tendencia a la evasión. Esto sugiere que la flexibilidad del contrato y la facilidad de pago son factores cruciales.

Variables Numéricas: Los histogramas de 'tenure' y 'Charges.Total' indicaron que los clientes que evaden tienden a tener un tiempo de contrato más corto y un total gastado menor. Esto refuerza la idea de que los clientes de corto plazo son más propensos a cancelar el servicio.

Conclusiones e Insights
Los principales hallazgos sugieren que la evasión está fuertemente relacionada con el tipo de contrato, la antigüedad del cliente y los métodos de pago. Los clientes con contratos de mes a mes, un menor tiempo de permanencia y un gasto total más bajo son los perfiles con mayor riesgo de evasión. Esto nos da una idea clara de a qué segmentos de clientes se debe prestar mayor atención.

Recomendaciones
Programas de Lealtad: Ofrecer incentivos y programas de lealtad a los clientes que han estado con la empresa por un corto período de tiempo para fomentar su permanencia.

Planes de Contrato: Promover planes de contrato más largos, como contratos anuales, a través de beneficios exclusivos, como descuentos o servicios adicionales, para reducir la tasa de 'churn' mensual.

Análisis de Métodos de Pago: Investigar si hay problemas o fricciones con ciertos métodos de pago que están asociados con la evasión y buscar formas de simplificar el proceso.

Estos insights pueden ser utilizados por el equipo de marketing y ventas para desarrollar estrategias de retención más efectivas y personalizadas.
