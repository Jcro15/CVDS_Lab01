### Hoja de vida

## datos basicos

* **nombre**: _Juan Camilo Angel Hernandez_
* **edad** : 19 años
* **ciudad** : Zipaquira

## intereses
mis intereses son:\

* escuchar musica como <https://youtu.be/_tcW-j7KFgY>
* programar
* ver cine

## plan de estudios
actualmente mi plan de estudios es:

1. CVDS
2. AUPN
3. FCFI
4. RECO

~~~
#Codigo regresion lineal

import numpy as np
import matplotlib.pyplot as plt

from sklearn.datasets import load_boston

#cargamos la libreria

boston = load_boston()
#print(boston.DESCR) #descripcion de ese dataset


# Formula para minimizar el error cuadratico medio (MCO) $\beta = (X^{T}X)^{-1}X^{T}Y$


X = np.array(boston.data[:,5]) #num_habitaciones

Y = np.array(boston.target) #valor medio

plt.scatter(X,Y,alpha=0.3)

#añadimos columna de unos (terminos independientes)

X = np.array([np.ones(506),X]).T

B = np.linalg.inv(X.T @ X) @ X.T @ Y #matriz de parametros que minimizan el ECM de la nube de puntos

plt.plot([4,9],[B[0]+B[1]*4,B[0]+B[1]*9], c="red")
plt.show()
~~~
![](https://www.researchgate.net/profile/Enrique_Rico-Garcia/publication/262762874/figure/fig2/AS:669959541755915@1536742210539/Figura-3-Regresion-lineal-entre-fotosintesis-medida-y-simulada-con-la-ANN-para-todo-el.png)

El modelo de pronóstico de regresión lineal permite hallar el valor esperado de una variable aleatoria a cuando b toma un valor específico.


 La aplicación de este método implica un supuesto de linealidad cuando la demanda presenta un comportamiento creciente o decreciente, por tal razón, se hace indispensable que previo a la selección de este método exista un análisis de regresión que determine la intensidad de las relaciones entre las variables que componen el modelo.
