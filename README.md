## Etapa 2: Reducción de Dimensionalidad mediante Análisis de Componentes Principales (PCA)

En esta segunda etapa del proyecto se aborda el problema de la alta dimensionalidad del dataset, el cual contiene múltiples variables macroeconómicas, demográficas y sociales. Con el fin de simplificar la estructura de los datos y capturar los principales patrones subyacentes, se aplica el **Análisis de Componentes Principales (PCA)** como técnica de reducción de dimensionalidad.

### Selección y preparación de variables

En primer lugar, se seleccionan exclusivamente las **variables numéricas**, dado que el PCA requiere datos cuantitativos continuos. Posteriormente, todas las variables seleccionadas son **estandarizadas**, de modo que cada una tenga media cero y desviación estándar igual a uno. Este paso es fundamental para evitar que variables medidas en distintas escalas dominen la construcción de las componentes principales.

### Aplicación del PCA

Una vez estandarizados los datos, se aplica el Análisis de Componentes Principales al conjunto de variables numéricas. Se analiza la **varianza explicada por cada componente**, así como la varianza acumulada, con el objetivo de evaluar cuánta información del dataset original es capturada por un número reducido de componentes.

Este análisis permite identificar las componentes más relevantes y comprender la estructura interna de los datos, reduciendo la redundancia existente entre variables altamente correlacionadas.

### Selección del número de componentes

Se selecciona el número de componentes principales necesarias para explicar entre un **70% y un 90% de la varianza total** del dataset. Este rango se considera un equilibrio adecuado entre:

* La reducción efectiva de la dimensionalidad.
* La preservación de información relevante para la tarea de clasificación posterior.

La elección final del número de componentes se justifica en función de la varianza acumulada explicada y del principio de parsimonia, priorizando modelos más simples sin una pérdida significativa de información.
