### La investigación está enfocada en un hospital que necesita automatizar el proceso de detección y clasificación de las enfermedades de pulmón. De esta forma, reducir el coste y tiempo en la detección de enfermedades para ello la base de datos está compuesta por 133 imágenes que pertenecen a 4 categorías:
* Sano
* Covid-19
* Pneumoniá Bacterial
* Pneumoniá Vírica
  La base de datos pesa 1.69 gb por lo que no podra ser subida a Github.
### Cargamos la base de datos en nuestro Jupyter Notebook con Python [Code](https://github.com/bastianastudillo98/Projects-Data-Science-/blob/main/Pulmonary%20Diseases/Code/Pulmonary%20Diseases%20Deep%20Learning.ipynb)  y se obtiene lo siguiente:

![Entrada Imagenes](https://github.com/bastianastudillo98/Projects-Data-Science-/blob/main/Pulmonary%20Diseases/Image/Entrada.png)
### Se entrena un modelo de redes neuronales y el resultado es el sigueinte:

![Salida Imagenes](https://github.com/bastianastudillo98/Projects-Data-Science-/blob/main/Pulmonary%20Diseases/Image/Salida.png)
### Evaluamos el modelo por los siguientes criterios:

![Resultados](https://github.com/bastianastudillo98/Projects-Data-Science-/blob/main/Pulmonary%20Diseases/Image/Resultados.png)
### En base a los resultados obtenidos, podemos concluir que:
#### Clases 0: 'COVID-19', 1: 'Normal', 2: 'Pneumonia Virica', 3: 'Pneumonia Bacteriana'

- Precisión: El modelo tiene una precisión promedio de alrededor de 0,70 en la clasificación. Esto significa que, en promedio, el 70% de las predicciones del modelo son correctas.
- Recall: El modelo muestra diferentes niveles de Recall para cada clase. Las clases 0 y 1 tienen un Recall relativamente alto, y las clases 2 y 3 tienen un Recall bajo. Esto muestra que el modelo es bueno para reconocer las clases 0 y 1, pero tiene dificultad para clasificar las clases 2 y 3 correctamente.
- F1-score: la puntuación F1 es una combinación de precisión y memoria, lo que indica un rendimiento general moderado en todas las clases. Las clases 0 y 1 tienen valores altos de F1 y las clases 2 y 3 tienen valores bajos de F1.
- Accurracy: La precisión del modelo es del 70%. Esto significa que el 70% de las muestras de prueba se clasifican correctamente.

En general, los modelos se desempeñan bastante bien en la clasificación, aunque su capacidad para discriminar cada clase varía. Se pueden realizar refinamientos en el modelo para mejorar la precisión y la capacidad de clasificación de las clases con los puntajes F1 y de recuperación más bajos.

![Matriz](https://github.com/bastianastudillo98/Projects-Data-Science-/blob/main/Pulmonary%20Diseases/Image/Matriz.png)

* Clase 0: 10 verdaderas positivos
* Clase 1: 8 verdaderos positivos y 2 negativos
* Clase 2: 5 Verdaderos positivos y 5 negativos
* Clase 3: 5 verdaderos positivos y 5 negativos
