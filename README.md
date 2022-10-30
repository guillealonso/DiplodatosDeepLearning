# DiplodatosDeepLearning
Repo para entrega de trabajos prácticos de la materia

## Módulo optativo de la diplomatura en ciencia de datos del FaMAF - Universidad Nacional de Córdoba. 2022

**Ingerantes del grupo:**
- Alonso, Guillermo 
- Pfluger, Santiago
- Perez, Lucas
- Serrantes, Sebastián

**Profesores:** 
- Johanna Frau 
- Mauricio Mazuecos

### Conclusiones TP1

- El experimento llevó gran esfuerzo y tiempo para lograr ejecutarlo ya que es una gran cantidad de datos y las pruebas de entrenamiento del modelo se hacen bastante extensas en el tiempo. Se trabajó con el modelo y los datos en GPU para el entrenamiento haciendo uso del hardware **nabucodonosor** del Centro de Computación de Alto Desempeño de la UNC. 
- Para las pruebas y construcción del modelo se utilizó una muestra del dataset. Inicialmente de 5 categorias y luego de 20. Para esto se filtraron en todos los datasets (train, validation y test) y se conservaron todos los registros de las categorias seleccionadas reduciendo considerablemente el tamaño y el tiempo de procesamiento.
- Como se puede observar en los registros del experimento se probaron diferentes números de capas ocultas y de diferentes valores, diferentes tipos de capa de salida, distinta cantidad de epochs en el entrenamiento y valores de learning rate. A partir de las pruebas se eligieron los parametros que dieron mejores resultados y luego se entrenó el modelo con el dataset completo. Afortunadamente esto no hizo variar los resultados obtenidos que se mantuvieron aproximadamente en los mismos valores.
    - En relacion al número de capas, en las pruebas no se notó mejora aumentando el número, razon por la cual se mantovo en 2.
    - En relación al valor de las capas, se comenzo con valores bajo y se fue aumentando logrando mejores resultados. Se conservaron los últimos valores que produjeron mejoras en los resultados.
    - En relación al número de epochs y learning rate, con el fin de reducir el tiempo de entrenamiento con el dataset completo, se probó aumentar levemente el lr para lograr llegar con menos epochs a los resultados deseados y se consiguió efectivamente.
