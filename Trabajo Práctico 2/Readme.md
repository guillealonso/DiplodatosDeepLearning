# Diplodatos Deep Learning - Trabajo Páctico 2
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

### Conclusiones TP2

- El experimento llevó gran esfuerzo y tiempo para lograr ejecutarlo ya que es una gran cantidad de datos y las pruebas de entrenamiento del modelo se hacen bastante extensas en el tiempo. Se trabajó con el modelo y los datos en GPU para el entrenamiento haciendo uso del hardware **nabucodonosor** del Centro de Computación de Alto Desempeño de la UNC. 
- Para las pruebas y construcción del modelo se utilizó, al igual que en el práctico 1, una muestra del dataset de 20 categorias. Para esto se filtraron en todos los datasets (train, validation y test) y se conservaron todos los registros de las categorias seleccionadas reduciendo considerablemente el tamaño y el tiempo de procesamiento.
- Como se puede observar en los registros del experimento se probaron diferentes configuraciónes y valores de capas en la red, diferentes tipos de capa de salida, `dropout`, cantidad de `epochs` en el entrenamiento y valores de `learning rate`. A partir de las pruebas se eligieron los parametros que dieron mejores resultados y luego se entrenó el modelo con el dataset completo. Esto causó una leve variación de los resultados obtenidos pasando de un 97% con 20 categorías a un 92% con el dataset completo(632) en balanced acuracy score evaluado sobre `test_dataset`. 
- En relacion al tiempo de entrenamiento fue mayor al de perceptron multicapa.
- En relación al número de `epochs` y `learning rate`, con el fin de reducir el tiempo de entrenamiento con el dataset completo, se probó aumentar levemente el lr para lograr llegar con menos epochs a los resultados deseados y se consiguió efectivamente.
- 
![MLFlow Runs-Experimento](https://github.com/guillealonso/DiplodatosDeepLearning/blob/main/Trabajo%20Pr%C3%A1ctico%202/CapturaMLFlow.JPG?raw=true)
![MLFlow ModeloFinal Parámetros](https://github.com/guillealonso/DiplodatosDeepLearning/blob/main/Trabajo%20Pr%C3%A1ctico%202/MLFlowTP2_Param.JPG?raw=true)
![MLFlow ModeloFinal Métricas](https://github.com/guillealonso/DiplodatosDeepLearning/blob/main/Trabajo%20Pr%C3%A1ctico%202/MLFlowTP2_Metrics.JPG?raw=true)
