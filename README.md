## Etapa 3: Implementación y Comparación de Modelos de Clasificación

La etapa final del proyecto se centra en la implementación y evaluación de modelos de clasificación, con el objetivo de analizar el impacto de la reducción de dimensionalidad sobre el desempeño predictivo y la estructura del problema. En esta fase se integran los resultados obtenidos en las etapas previas y se contrastan distintos enfoques de modelación.

### Modelos de clasificación con variables originales

En primer lugar, se entrenan dos modelos de clasificación utilizando el **conjunto de datos original**, es decir, considerando la totalidad de las variables explicativas disponibles y sin aplicar técnicas de reducción de dimensionalidad. Este enfoque permite establecer una **línea base (baseline)**, que sirve como punto de referencia para evaluar el desempeño de los modelos en un contexto de alta dimensionalidad.

### Modelos de clasificación con componentes principales

Posteriormente, se implementan los mismos modelos de clasificación utilizando como variables de entrada las **componentes principales obtenidas mediante PCA** en la etapa anterior. Este enfoque permite evaluar si la representación reducida de los datos es capaz de preservar la información relevante necesaria para predecir correctamente el nivel de PIB per cápita de los países.

### Criterios metodológicos y evaluación

Ambos enfoques se desarrollan bajo **condiciones metodológicas comparables**, manteniendo criterios consistentes de partición de los datos en conjuntos de entrenamiento y prueba, así como el uso de métricas de evaluación apropiadas para problemas de clasificación. Esto asegura que las diferencias observadas en el desempeño de los modelos puedan atribuirse al uso (o no) de la reducción de dimensionalidad, y no a cambios en la metodología.

El desempeño de los modelos se analiza mediante indicadores estándar de clasificación, permitiendo contrastar de forma objetiva los resultados obtenidos con datos originales y con datos reducidos.
