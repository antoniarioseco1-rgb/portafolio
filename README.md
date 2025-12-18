
## Etapa 3: Implementación y Comparación de Modelos de Clasificación

La etapa final del proyecto se centra en la implementación y evaluación de modelos de clasificación, con el objetivo de analizar el impacto de la reducción de dimensionalidad sobre el desempeño predictivo y la estructura del problema. En esta fase se integran los resultados obtenidos en las etapas previas y se contrastan distintos enfoques de modelación.

### Modelos de clasificación con variables originales

En primer lugar, se entrenan dos modelos de clasificación utilizando el **conjunto de datos original**, es decir, considerando la totalidad de las variables explicativas disponibles y sin aplicar técnicas de reducción de dimensionalidad. Este enfoque permite establecer una **línea base (baseline)**, que sirve como punto de referencia para evaluar el desempeño de los modelos en un contexto de alta dimensionalidad.

### Modelos de clasificación con componentes principales

Posteriormente, se implementan los mismos modelos de clasificación utilizando como variables de entrada las **componentes principales obtenidas mediante PCA** en la etapa anterior. Este enfoque permite evaluar si la representación reducida de los datos es capaz de preservar la información relevante necesaria para predecir correctamente el nivel de PIB per cápita de los países.

### Criterios metodológicos y evaluación

Ambos enfoques se desarrollan bajo **condiciones metodológicas comparables**, manteniendo criterios consistentes de partición de los datos en conjuntos de entrenamiento y prueba, así como el uso de métricas de evaluación apropiadas para problemas de clasificación. Esto asegura que las diferencias observadas en el desempeño de los modelos puedan atribuirse al uso (o no) de la reducción de dimensionalidad, y no a cambios en la metodología.

El desempeño de los modelos se analiza mediante indicadores estándar de clasificación, permitiendo contrastar de forma objetiva los resultados obtenidos con datos originales y con datos reducidos.
## Descripción del proyecto portafolio

Este proyecto tiene como finalidad analizar y modelar el nivel de desarrollo económico de distintos países a partir de indicadores socioeconómicos oficiales del Banco Mundial. En particular, se busca predecir el nivel de PIB per cápita de cada país mediante técnicas básicas de ciencia de datos.

El enfoque del proyecto no se limita únicamente a obtener buenos resultados predictivos, sino que pone énfasis en comprender la relación entre variables, tales como salud, educación, estructura productiva, comercio etc, y su vínculo con el nivel de ingreso de los países. De esta forma, se aborda el desarrollo económico como un fenómeno multidimensional y no solo monetario.

## Objetivos

* Analizar descriptivamente los datos del Banco Mundial, identificando patrones generales, valores faltantes y outliers relevantes. Todo esto a travez de la preparacion y limpieza del conjunto de datos mediante imputación y selección de variables. Buscando reducir la dimensionalidad del dataset utilizando Análisis de Componentes Principales (PCA).


## Estructura del Proyecto

El desarrollo del proyecto se organiza en tres etapas, cada una trabajada en una rama independiente de GitHub y posteriormente integrada a la rama principal (`main`):

### Etapa 1: Análisis Descriptivo e Imputación de Datos

* Revisión general del dataset: número de países, años, variables y observaciones.
* Análisis de datos faltantes y decisión de imputación o eliminación de variables.
* Identificación de outliers y patrones relevantes.
* Generación de estadísticas descriptivas.
* Análisis de la distribución del PIB y discretización del nivel de PIB per cápita en cinco categorías.
* Visualizaciones exploratorias, incluyendo histogramas, boxplots y mapas.

### Etapa 2: Reducción de Dimensionalidad con PCA

* Selección de variables numéricas relevantes.
* Estandarización de los datos.
* Aplicación de Análisis de Componentes Principales.
* Evaluación de la varianza explicada y selección del número óptimo de componentes.
* Construcción de un nuevo dataset reducido para su uso en modelación.

### Etapa 3: Modelación y Comparación de Algoritmos de Clasificación

* Entrenamiento de modelos de clasificación utilizando el dataset original (baseline).
* Entrenamiento de los mismos modelos utilizando las componentes principales.
* Evaluación del desempeño mediante métricas estándar de clasificación.
* Comparación de resultados y análisis del impacto del uso de PCA en términos de desempeño, complejidad e interpretabilidad.


