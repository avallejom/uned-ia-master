# Clustering en Apache Spark con distancia coseno

El algoritmo de Clustering de Spark utiliza la distancia euclidea. En contextos dispersos y con elevada dimensionalidad funciona mejor la distancia coseno.
En este repositorio se encuentra la modificación de la clase de scala original KMeans.scala concretamente sobre la versión 1.3.1 de Spark. La modificación del algoritmo ha consistido en sustituir la distancia euclidea por la distancia coseno.

```
distancia_coseno (x,y)= 1 - x·y / (sqrt(x1^2+x2^2+...+xn^2) · sqrt(y1^2+y2^2+...+yn^2)  ) 
```
