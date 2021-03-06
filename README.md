# MCOC2021-P3-Grupo05

INTEGRANTES PROYECTO 3 - GRUPO 5
1. José Tomás Gutierrez
2. José Ignacio Hirmas
3. Isidora Línacre

# Entrega 2

![fig1](https://user-images.githubusercontent.com/70209467/140690702-b66465dd-e3d8-4527-bf5d-229f2e3426ac.png)
![fig2](https://user-images.githubusercontent.com/70209467/140690715-36918f9a-c33a-4005-9beb-3861d33157d3.png)
![fig3](https://user-images.githubusercontent.com/70209467/140690729-6bac38ad-b289-470b-a11e-2b8d29fe84fc.png)
![fig4](https://user-images.githubusercontent.com/70209467/140690735-497fcd7d-5c88-4932-a015-afecfb6485db.png)

# Entrega 3

JOSE IGNACIO HIRMAS

![image](https://user-images.githubusercontent.com/70209467/141397293-959f45ed-390f-49b8-b487-e763225a3dce.png)

ISIDORA LINACRE

![image](https://github.com/isilinacre/MCOC2021-P3-Grupo05/blob/main/P3E3_Linacre.png)

JOSE TOMAS GUTIERREZ

![image](https://user-images.githubusercontent.com/71188483/141407985-5d094753-18bc-4b53-addb-5388df1656e4.png)




# Entrega 4

1) Explique en su Readme.md el código que usó para resolver el problema, comentando las lineas más relevantes. Especial énfasis en el algoritmo usado para asignar los flujos. 

R: Para resolver el problema, se utilizó un algoritmo basado en Djasktras, para obtener el camino mas barato y luego se le asignaba unidades de flujo a este. Esta "unidad"
se repitio varias veces hasta enviar la totalidad del flujo desde los origenes y destinos de la matriz OD. Cabe mencionar que, se llego a obtener una diferencia de flujos,
de aproximadamente 0.3 viajes con la pauta, lo cual es normal por las aproximaciones y arquitectura del algoritmo que quiza difiera en algunos detalles con la pauta.

Una de las secciones mas relevantes del codigo era esta "unidad" anteriormente mencionada que iba enviando las unidades de flujo desde los origenes a los destinos. El
algoritmo se presenta a continuación:

![image](https://user-images.githubusercontent.com/71188483/141882133-982ed4d3-98d8-4bf0-a3fe-0796189146ab.png)

Luego, para verificar el equilibrio de Wardrop, se utilizó un algoritmo que obtenia todos los caminos para un par origen destino, obtenia sus costos y luego definia el minimo 
de los costos como el objetivo, con el cual se comparaban todos los costos. Si el error entre 2 pares de costos era menor que el 1% se tomaba como que los caminos
tenian costos equivalentes y se cumplia el equilibrio (para verificar el equilibrio se recomienda correr el Python y revisar la consola). El algoritmo se presenta a continuación:


![image](https://user-images.githubusercontent.com/71188483/141882395-5342574a-b20f-4089-9d78-c2a25c55d394.png)

2) Graficos:

Costos:

![image](https://user-images.githubusercontent.com/71188483/141882576-e5912c9e-5085-4103-b801-f603d04c361e.png)


Flujos:

![image](https://user-images.githubusercontent.com/71188483/141882601-e74193bf-9ab7-474a-9a43-b71c729deb02.png)


Funciones de costos por arcos:

![image](https://user-images.githubusercontent.com/71188483/141882633-22f78c61-3802-42c4-91ce-e491c1fbfbc6.png)

# ENTREGA 5

![image](https://user-images.githubusercontent.com/70209467/142665892-30122769-038a-4fce-8e92-f30283bf4472.png)

Pregunta 1: Las zonas seleccionadas se tomaron recorriendo la matriz origen destino y observando cuales viajes inluían Américo Vespucio en el trayecto, por lo que si un viaje usaba Américo Vespucio, se consideraba la zona de origen y la de destino. Cabe destacar que hay zonas muy cercanas a AVO que la lógica de recorrer la matriz origen destino no las toma en cuenta dado que zonas cercanas a Américo Vespucio podrían no necesitar ese tramo para moverse a otra zona. Cabe destacar que la funcion a costo inicial para ver que viaje usaba AVO fue una version simplificada de la funcion de costo original, ya que asumimos que el flujo era 0 y el factor que cobrarba mas incidencia era el tiempo ascociado a la longitud y velocidad del arco

Pregunta 2: Con la lógica de la pregunta 1, se formó una lista con las zonas consideradas, dando un total de 502 zonas.

Pregunta 3: Se deberán asignar la cantidad de viajes que utilicen algun tramo de Américo Vespucio, toda esta info obtenida de la matriz OD.

Pregunta 4: Los pares OD que generen mayor flujo son los viajes provenientes de las zonas limítrofes, puesto que como Américo Vespucio es un anillo que recorre los lugares alejados del centro de Santiago, los viajes que utlicen esta autopísta serán de los que necesiten trasladarse de una zona limítrofe de la ciudad a otra.



