# EDA_LINEAR-REGRESSION_HYPOTHESIS_AlanJafetLeonLoeza

#En el presente docuemnto se detalla la informacion general sobre el proyecto

Los objetivos del proyecto son :
• Utilizar Git para llevar a cabo el control de versiones.
• Realizar el análisis exploratorio de los datos completo sobre un dataset real.
•	Poner en práctica conocimientos teóricos y ejercitar lacapacidad de análisis.
•	Desmostrar habilidades al crear un modelo de regresión lineal multivariable.
• Familiarizarse con las pruebas de hipótesis.

El proceso General es el siguiente :
1.	Exploración de los datos.
2.	Manipulación y tratamiento de los datos.
3.	Construcción de un modelo de regresión lineal.
4.	Hipótesis.
5.	Publicación del proyecto.

Etapas y su Justificacion :
ETAPA 1: Exploración de los datos
  Paso 1: Cargue el dataset ("Retrasos.csv") en un dataframe, muestre información básica, enliste las columnas numéricas y las columnas objeto.
  Paso 2: Haga conteo de datos nulos (ordene de forma descendente); de las variables numéricas, muestre datos estadísticos; de las variables de tipo objeto, 
  determine cuáles sí son factibles para convertir en categóricas y el porqué.
  Paso 3: Identifique si las columnas numéricas cuentan con anomalías, para ello puede apoyarse de gráficos; identifique si las columnas objeto tienen 
  inconsistencias, para ello puede apoyarse de gráficos.
  Paso 4: Muestre las correlaciones (pearson y spearman) que hay en general (valores numéricos), puede utilizar gráficos, ¿cambian mucho los valores entre 
  cada 
  tipo de coeficiente de correlación?
  Paso 5: Muestre los gráficos de distribución de las columnas, elija el tipo de gráfico adecuado para el tipo de variable que está analizando.
ETAPA 2: Manipulación y tratamiento de los datos.
  Paso 1: Trate los datos nulos, emplee las técnicas que considere más adecuadas de acuerdo al caso específico. Justifique el porqué de la técnicas que 
  escogió.
  Paso 2: Convierta en categorías las variables objeto que considere adecuadas, en caso de ser necesario, trate las inconsistencias.
  Paso 3: Utilice el coeficiente de variación para determinar qué columnas (variables) numéricas tienen mayor dispersión.
  Paso 4: De las variables con mayor dispersión, presente su distribución, su gráfico boxplot, y describa a qué se debe que haya tanta dispersión.
  Paso 5: Conteste las siguientes preguntas acorde a la información obtenida de los datos.
  ¿Considera que con los datos numéricos actuales se pueden realizar predicciones para la columna "line_item_insurance_usd"?
  ¿Considera que con los datos numéricos actuales se pueden realizar predicciones para la columna "late_delivery"?
  ¿Cree que alguna otra columna (objeto o categórica) se pueda correlacionar fuertemente con "late_delivery"?
ETAPA 3: Construcción de un modelo de regresión lineal.
  Paso 1: Seleccionar las columnas que estén más correlacionadas con "line_item_insurance_usd" y asígnelas en la variable "X", seleccione la columna 
  "line_item_insurance_usd" y asignela a la variable "y".
  Paso 2: Divida en dos muestras los dos dataframes creados anteriormente (X,y), debe tener una muestra para entrenamiento y otra para pruebas, el tamaño de 
  la muestra de entrenamiento debe ser del 80%, asigne una semilla aleatoria con valor de 2033 para poder brindar reproducibilidad.
  Paso 3: Importe el modelo de regresión lineal (multivariable) de sklearn, entrene el modelo con el set de datos de entrenamiento, posteriormente haga 
  predicciones con el set de pruebas (X_train).
  Paso 4: Evalúe el modelo con la métrica "accuracy_score" y la métrica "f1_score" (ambas disponibles con sklearn).
  Paso 5: Responda.
  ¿Su modelo fue capaz de realizar predicciones con precisión?
  ¿A qué cree que se deba el rendimiento de su modelo?
  Si selecciona todas las variables y las asigna en X, en lugar de las que tienen correlación más fuerte, ¿cree que el modelo mejore o empeore?
ETAPA 4: Hipótesis.
  Paso 1: Defina la hipótesis nula a partir de la siguiente pregunta:
  ¿La proporción de entrega tarde ("late_delivery") es mayor a 0.06 (6%)?, asigne el valor de la hipótesis nula a la variable "Ho".
  Considere un nivel de significación del 5%.
  Paso 2: Defina la hipótesis alternativa según la pregunta anterior, solo escríba cómo quedaría y qué tipo de prueba de hipótesis se utilizará.
  Paso 3: Haga una distribución bootstrap de la columna "late_delivery" y calcule el error estándar, guárdelo en una variable. El tamaño de la lista de la 
  distribución de boostrap queda a libre elección, muestre un histograma de la distribución bootstrap.
  Paso 4: Calcule la puntuación Z y guárdela en una variable.
  Paso 5: Dependiendo del tipo de prueba, calcule el valor de P (p-value) y diga si puede rechazar (o falla al rechazar) la hipótesis nula.
  Calcule el intervalo de confianza, utilice los cuantiles adecuados dado el nivel de significación establecido previamente.

Conclusiones a grandes rasgos, los resultados fueron satisfactorias respecto a los objetivos propuestos, por ejemplo el modelo de regresion predice de manera satisfactoria la variabkle objetivo , tambien se logro aceptar la hipotesis nula; ademas de que el analisis exploratorio realizado es tambien satisfactorio ya que gracias a el, se obtuvieron los resultados deseados.

  
