Universidad del Valle de Guatemala  
Facultad de Ingeniería  
Departamento de Ciencias de la Computación  
CC3074 – Minería de Datos  
Semestre I – 2026  

# Laboratorio 3
## Modelos de Regresión Lineal

## INTRODUCCIÓN:

La empresa SmartStay Advisors es una firma intermediaria que facilita la búsqueda y selección de propiedades en Airbnb para clientes corporativos y particulares.

El modelo operativo es el siguiente:

• El cliente proporciona requerimientos específicos (ciudad, presupuesto, tipo de propiedad, capacidad, duración de estancia).  
• SmartStay analiza la oferta disponible y propone propiedades que optimicen precio, calidad y disponibilidad.  
• Airbnb ofrece incentivos económicos a SmartStay cuando logra incrementar el nivel de ocupación de propiedades con bajo desempeño.

La empresa desea implementar modelos de minería de datos que le permitan:

1. Estimar precios competitivos.  
2. Identificar propiedades con baja ocupación.  
3. Comprender qué factores influyen en la ocupación y los ingresos.  
4. Diseñar estrategias basadas en datos para aumentar la rentabilidad.

## Conjunto de datos a utilizar

- listings.RData

## Descripción de la Consultoría:

La consultoría se dividirá en varias etapas. Cada semana deberá entregar resultados de la aplicación de un algoritmo de predicción y/o clasificación. La conclusión será la elección del mejor algoritmo predictivo para estimar el valor o la ocupación de una vivienda.

Se le provee un diccionario de variables con el nombre y la descripción de cada una de las variables.

## Resultados esperados en la Primera Entrega Consultoría:

Se espera la entrega de un informe detallado donde incluya el análisis exploratorio del conjunto de datos (incluyendo agrupamiento) y la evaluación de varios modelos de regresión lineal simple y múltiple. Debe seleccionar el mejor modelo de los construidos para predecir el precio de la vivienda.

## Notas:

- La consultoría es en grupo, por lo que solo se tendrán en cuenta los grupos conformados por más de un especialista.
- Cada individuo será evaluado de forma individual basado en sus aportes al trabajo grupal, por lo que deben versionar el código para poder revisar las contribuciones de cada uno.

---

Universidad del Valle de Guatemala  
Facultad de Ingeniería  
Departamento de Ciencias de la Computación  
CC3074 – Minería de Datos  
Semestre I – 2026  

# INSTRUCCIONES

- Utilice el conjunto de datos que se le provee. Debe hacer un análisis exploratorio para entender mejor los datos, sabiendo que el objetivo final es predecir los precios de las casas. Recuerde explicar bien cada uno de los hallazgos que haga. La forma más organizada de hacer un análisis exploratorio es generando ciertas preguntas de las líneas que le parece interesante investigar. Genere un informe con las explicaciones de los pasos que llevó a cabo y los resultados obtenidos. Recuerde que la investigación debe ser reproducible por lo que debe guardar el código que ha utilizado para resolver los ejercicios.

# ACTIVIDADES

1. Descargue el conjunto de datos.

2. Haga un análisis exploratorio extenso de los datos. Explique bien todos los hallazgos. No ponga solo gráficas y código. Debe llegar a conclusiones interesantes para poder predecir. Explique el preprocesamiento que necesitó hacer.

3. Incluya un análisis de grupos en el análisis exploratorio. Explique las características de cada uno.

4. Divida el set de datos preprocesados en dos conjuntos: Entrenamiento y prueba. Describa el criterio que usó para crear los conjuntos: número de filas de cada uno, estratificado o no, balanceado o no, etc.

5. Haga ingeniería de características, ¿qué variables cree que puedan ser mejores predictores para el precio de las casas? Explique en que basó la selección o no de las variables.

6. Todos los resultados deben ser reproducibles por lo que debe fijar que los conjuntos de entrenamiento y prueba sean los mismos siempre que se ejecute el código.

7. Seleccione una de las variables y haga un modelo univariado de regresión lineal para predecir el precio de las casas. Analice el modelo (resumen, residuos, resultados de la predicción). Muéstrelo gráficamente.

8. Haga un modelo de regresión lineal con todas las variables numéricas para predecir el precio de las casas. Analice el modelo (resumen, residuos, resultados de la predicción). Muestre el modelo gráficamente.

9. Analice el modelo. Determine si hay multicolinealidad entre las variables, y cuáles son las que aportan al modelo. Haga un análisis de correlación de las características del modelo y especifique si el modelo se adapta bien a los datos. Explique si hay sobreajuste (overfitting) o no. En caso de existir sobreajuste, haga otro modelo que lo corrija.

10. Si tiene multicolinealidad o sobreajuste, haga un modelo con las variables que sean mejores predictoras del precio de las casas. Determine la calidad del modelo realizando un análisis de los residuos. Muéstrelo gráficamente.

11. Elabore un modelo en el que utilice al menos una de las técnicas de regularización (Ridge, Lasso, ElasticNet) compare los resultados con los otros modelos.

12. Utilice cada modelo con el conjunto de prueba y determine la eficiencia del algoritmo para predecir el precio de las casas. ¿Qué tan bien lo hizo? ¿Qué medidas usó para determinar la calidad de la predicción?

13. Discuta sobre la efectividad de los modelos. ¿Cuál lo hizo mejor? ¿Cuál es el mejor modelo para predecir el precio de las casas? Haga los gráficos que crea que le pueden ayudar en la discusión.

# EVALUACIÓN

Nota: Tiene que poderse comprobar su aporte al trabajo grupal a través de commits. Si no existen al menos 3 commits con su aporte significativo no va a poder ser evaluado en la entrega. Utilice una herramienta que permita registrar los aportes de cada uno.

---

Universidad del Valle de Guatemala  
Facultad de Ingeniería  
Departamento de Ciencias de la Computación  
CC3074 – Minería de Datos  
Semestre I – 2026  

- (25 puntos) Análisis exploratorio de los datos. Se hizo un análisis exploratorio lo suficientemente extenso que permita explicar las variables que pudieran estar influyendo en la variable respuesta, que es el precio de las casas. Análisis de las variables a incluir en el modelo. Pruebas de normalidad, correlación, etc.

- (25 puntos) Análisis de los modelos generados, incluyendo los residuos. Recuerde explicar los razonamientos (modelo de regresión lineal simple, múltiple y con regularización).

- (10 puntos) Aplicación de los modelos al conjunto de prueba.

- (20 puntos) Explicación de los resultados obtenidos incluyendo el desempeño de los modelos.

- (20 puntos) Comparación entre los modelos elaborados y selección del mejor de todos para predecir el precio de las casas.

# MATERIAL A ENTREGAR

- Archivo `.rmd`, `.ipynb` o Google docs con el informe con lo solicitado en las instrucciones  
- Script de R o de Python que utilizó debidamente organizado y comentado (Si utilizó rmd debe añadir el html que se genera)  
- Link de controlador de versiones utilizado  

# FECHAS DE ENTREGA

- PASAPORTE: Descripción de las variables, análisis exploratorio, análisis de relaciones con la variable respuesta: viernes 13 de marzo 17:20.

- ENTREGA FINAL: Domingo 15 de marzo a las 23:59

# NOTA:

- No se aceptará un análisis exploratorio sin explicaciones de los hallazgos.
- Para poder tener nota completa debe entregar las asignaciones en el tiempo adecuado. No se calificará el avance (pasaporte) de la entrega si no fue subido en tiempo, aunque esté en el repositorio.
- Si alguno de los miembros del grupo de trabajo no llega al trabajo colaborativo en clase, no tendrá derecho a la nota del laboratorio.
- La descripción y explicación de resultados es crucial en el análisis de los datos por lo que no se tomarán en cuenta gráficos o tablas que no estén explicadas ni para avances ni para entrega final.
- Se tomarán en cuenta las contribuciones individuales para calificar el trabajo de cada uno, si no tiene suficientes contribuciones significativas en código y en análisis no tiene derecho a nota.
