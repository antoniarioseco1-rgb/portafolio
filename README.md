## Etapa 1: Análisis Descriptivo e Imputación de Datos

La primera etapa del proyecto tiene como objetivo comprender la estructura general del conjunto de datos y preparar la información para las etapas posteriores de reducción de dimensionalidad y modelación. Para ello, se realiza un análisis descriptivo exhaustivo y un tratamiento sistemático de los datos faltantes, asegurando la coherencia y calidad del dataset.

### Revisión general del dataset

En primer lugar, se explora el conjunto de datos obtenido desde el Banco Mundial, identificando:

* El número total de países incluidos en el análisis.
* El rango de años disponibles.
* La cantidad total de variables socioeconómicas.
* El número total de observaciones del dataset.

Esta revisión inicial permite dimensionar el alcance del análisis y detectar posibles limitaciones asociadas a la cobertura temporal o geográfica de los datos.

### Análisis de datos faltantes

Posteriormente, se calcula el porcentaje de valores faltantes (NA) para cada variable. En base a este análisis, se adopta el siguiente criterio metodológico:

* Variables con menos de un **15% de datos faltantes** son imputadas, con el fin de preservar la mayor cantidad de información posible.
* Variables que superan este umbral son eliminadas, ya que su alto nivel de ausencia podría introducir sesgos o ruido en el análisis posterior.

Este criterio busca equilibrar la calidad del dataset con la conservación de información relevante para el estudio del desarrollo económico.

### Identificación de outliers

Se identifican valores atípicos relevantes mediante análisis exploratorio, considerando estadísticas descriptivas y visualizaciones. La detección de outliers permite evaluar si estos corresponden a errores de medición o a características estructurales propias de ciertos países, particularmente en variables como el PIB.

### Estadísticas descriptivas

Se genera una tabla de estadísticas descriptivas para las principales variables numéricas, incluyendo:

* Media
* Mediana
* Desviación estándar
* Valor mínimo
* Valor máximo

Este análisis proporciona una visión general del comportamiento y dispersión de los indicadores socioeconómicos considerados.

### Análisis de la variable objetivo: PIB

Dado que el PIB per cápita es la variable objetivo del proyecto, se analiza su distribución mediante visualizaciones como histogramas y/o boxplots. Este paso es clave para comprender su asimetría, dispersión y la presencia de valores extremos entre países.

Adicionalmente, se construye un **mapa con la distribución del PIB**, permitiendo observar patrones geográficos y diferencias regionales en el nivel de desarrollo económico.

### Discretización del nivel de PIB

Con el fin de formular el problema como una tarea de clasificación, la variable dependiente **NY.GDP.MKTP.PP.KD** es discretizada en cinco categorías de igual frecuencia utilizando cuantiles:

* Low
* Medium-Low
* Medium
* Medium-High
* High

Esta transformación permite clasificar a los países según su nivel relativo de ingreso y facilita la aplicación de modelos de clasificación supervisada en las etapas posteriores.

### Resultados de la etapa

Finalmente, el notebook correspondiente a esta etapa —con todos los análisis, visualizaciones y justificaciones— es ejecutado y enviado al repositorio de GitHub en la rama asociada a la **Etapa 1**, cumpliendo con las indicaciones de control de versiones del proyecto.
