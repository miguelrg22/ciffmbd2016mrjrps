# ciffmbd2016mrjrps
Automatización de procesos con python

## INSTALACIÓN

import install bdusers

## DESCRIPCIÓN

En este paquete python consta de 3 funciones:

- Una función de Data Cleaning.
  Limpieza de datos, detección y reemplazo de valores anómalos y perdidos, transformación de variables no numéricas y eliminación de valores duplicados.
  Ejemplos:
      maindos(my_data_train_cv,my_data_test_cv)
      mainuno(my_data_train_cv)

- Una función de creación y selección de variables mediante PCA y Decision Tree.
  Se aplica la función a dos csv, uno de train y otro de test que te devolverán otros dos con la creación y selección de las variables.
  Y la otra función se aplica a un csv sólamente y te devuelve a otro con las variables generadas y seleccionadas.
  Ejemplos:
      create_good_2var(my_data_train_cv,my_data_test_cv)
      create_good_1var(my_data_train_cv)

- Una función que aplica 6 tipos de modelos y te devuelve cuál es el que se ajusta más.
  En la función "seleccion" se parte de dos data frames: 
  data frame de entrenamiento (df_train) y el data frame de testeo (df_test). También hay que declarar la variable objetivo (y_train).
  La función "seleccion" ejecuta 6 algoritmos de aprendizaje automático: Logistic Regression, Decission Tree Regressor, Naive Bayes, Random Forest, Support Vector Machine y Redes Neuronales. 
  Una vez ejecutados los algoritmos, calculamos el RMSE y el Gini del modelo para evaluar el mejor modelo, en caso de no concurrencia, se determina el mejor modelo a través de Gini.
  Ejemplos:
      Seleccion(DataSetTrain,DataSetTest)
