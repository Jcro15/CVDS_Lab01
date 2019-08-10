
### Hoja de vida

## datos basicos

* **nombre**: _Juan Camilo Angel Hernandez_
* **edad** : 19 años
* **ciudad** : Zipaquira

## intereses
mis intereses son:

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

![](https://lh3.googleusercontent.com/lERJYIIOvFQrGgQgxHk7YlNTmTo3GhRgC6LDt759yPqTqNGfXdcMCldDxUX1QGgfzJOAGB9qf88KEL4zj1aOM-YJWY6ILVw0vFgPevApaA49SOPOSQKF3_gKO5qIt7SDX1Tw-moxp-amFPFCjlXhnrqWiM7ssIG6AL0CYW3YwHmtb_k0w-otIjFqllOU65NybNLOtbt8uTgZeiMDNVx9msJIF2U7TQ3WGBVRsIzSb6A_3uYFBywIbRixYZ5r5cg54dTx3m9l3hdU_SMBZPGegFaL_WhXbF9Bk4-HRP6rr2603NLzd5Uz6bApwDZo5JQCSx3sA4a1-lJAerWTWX0fTefFh6MeZ5zoFOQDJhy1noAHTKSeP4T0gj52b-vR01Uo6pc9tknPBi5TkoG6oq0ZfM0A9gw1dZ62eVMZi1Lp5DmyiCgoAzP3Ir6YoWPcfdihc4XR54EEScO0NqmnCEnfGNGl1ekbmFII9S5KtnlumUZhXt1xYLNr-9DZ94YBmolqpmFtp0i4-BdaWlVGhZ3nSG4yYvVyBCUq6PCycU4HJqzca7IXzDmJwEvxf_xeYd4GQuTrCH1lPoIoGDPEeoSAvkLLqmWEByYbiwWyFCG0huEaw7U9xH-0m7v4eFtIsrjW0wftep99F9rMZnwYDhhqylI5Yd-aDv8=w818-h610-no)
![](https://lh3.googleusercontent.com/QhVk7bFO18OQARNnOqiEnzenLj9LEidnbc9rIK9bCMeq2aEDlN2dPoGWJFs9N54hUJfI-uX_h6RwVF351Fle1tmmzcqc8K7dksnNtESi0IXIpYymP1pqu8qeBib-SVSug9L6re_6-8uJALwCR_k6dVGLUN3V7hrFxDhFF5IrDA924F449EYdez-ZAQreZ03JjD1M4q8gL96CxgAoZO466nJND7pHBDhmLBuKR5XvWeyVZEHvBZAFG67NSnOK6Pf0NliZkdrSY5qiKL28Bmv6JB_4fbyZUvZ4jw0xz98zFIH6OjjrBsMQpqaloSM0NK553cvdgJM3jx2EgQFgrumTa7bDYBnwfzfukqtorKiCpdTmj3-CqBnh5kII_xMGQy_DZLpzNwqoaaXln6T5ovWqmB_7ICxbdodCiToUfE0KIDtp-WIMoR2cLICqU49U-lxuB3RQDJ0Nq85gAH5e2dKBoPGWb0DEWaC5oBgRoOvTfhUhbSV_9IR2MOAhybgzO7Kkm7KOHDCUjsofold4H-REp6XEBLNesjsrzXF33AQumf-ClbNlspgbJdt7PopCfkQKygNALCGjondzmmiMsPoPNKi2gKjN_0WYUCbJwN54RlaWcL0H1pEWLF9JD1btRF2hHk-fMLg4LT-sAZVqXaf_sr1JcFMZLbc=w754-h422-no)
