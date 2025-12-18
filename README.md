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


