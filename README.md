# Analisis_exploratorio_de_tweepy
Se realiza el análisis exploratorio de datos y sentimientos de comentarios de twitter

En una primera parte se aplica un puntaje a cada tweet, con la librería sentiment_análisis, con el fin de ver la dispersión de sentimientos de los mismos.

Se categorizan los tweets como:

1- Muy malos
2- Malos
3- Buenos
4- Muy buenos
5- Excelentes

A cada categoría le corresponde un rango de puntaje, en carácter de sentimientos:

* A Muy malos de 0 a 0.2.

* Malos de 0.2 a 0.4.

* Buenos de 0.4 a 0.6

* Muy buenos de 0.6 a 0.8

* Excelentes de 0.8 a 1.

Una vez vista la dispersión se procede a derivar los tweets.

## Que es derivar tweets?: 

Es un proceso que se lo denomina así porque, se eliminan partes de él.
Por ejemplo: las urls que contienen, los RT y los arrobas. Esto se realiza, porque en principio no se sabía cuanto afectaba en el puntaje del comentario.

Luego de ver la dispersión, se eliminan los outliers. 

Es decir que a cada categoría previamente asignada, si vemos que tiene una gran dispersión de puntajes. Dichos comentarios se eliminan del dataset, porque no
coincide con la etiqueta, y esto puede afectar a nuestro modelo. Basandonos en la teoría "Garbage in, garbage out".

# Se concatenan los datasets, el de Amazon con los Tweets.
# Se entrenan a los modelos.
# Se elige al mejor modelo de predicción.
