# "Análisis del Consumo de Energía Eléctrica por Entidad Federativa y su correlación con el Producto Interno Bruto (PIB)"

## Contenido:

## 1.	Selección y Justificación de la Base de Datos.
    a.	Busqueda de la base de datos.
    b.	Justificación de la selección.
## 2.	Preparación y limpieza de los datos.
    a.	Descripción de la base de datos.
    b.	Limpieza de datos.
## 3.	Análisis exploratorio de datos (EDA).
    a.	Análisis descriptivo.
## 4.	Visualización de datos.
    a.	Herramienta de visualización.
    b.	Principales visualizaciones.
## 5.	Interpretación y conclusiones.
    a.	Resultados de análisis
    b.	Conclusiones

## 1. Selección y Justificación de la Base de Datos.

He elegido realizar el análisis de este apasionante tema: El consumo de energía eléctrica y su correlación con el crecimiento económico, dicho análisis acotado a nivel entidad federativa y Nacional.

El objetivo es demostrar que en condiciones normales la correlación entre el PIB y el consumo de energía eléctrica debe ser positiva, tanto a nivel nacional como por entidad federativa. Ahora bien, en los casos que no sea así, determinar la causa raíz.

Iniciemos con lo referente al consumo de energía eléctrica. El consumo final de energía eléctrica se refiere a la energía eléctrica vendida a través de CFE suministradores y esquemas de autoabastecimiento. El consumo final se compone por seis sectores tarifarios: residencial, comercial, servicios, bombeo agrícola, empresa mediana y gran industria, estos últimos concentran el 37.4% y 23.7%, respectivamente. En tercer lugar, está el sector residencial con 26.3%, le siguen el comercial, agrícola y servicios con 5.8%, 5.4% y 1.4%, en ese orden. 

Es importante señalar que, la planeación del desarrollo del sector eléctrico parte del análisis del consumo de electricidad para el mediano y largo plazo. Ello permite diseñar de manera óptima el desarrollo y la expansión de capacidad de las actividades de generación, transmisión, distribución y comercialización de energía eléctrica.
El crecimiento del consumo de energía eléctrica está sujeto a diversos factores entre los más determinantes se encuentran: 

**Crecimiento económico.** Consiste en la tasa de crecimiento del Producto Interno Bruto (PIB). Si el crecimiento de la economía de una localidad o región aumenta, en consecuencia, también lo hace el consumo y la demanda de electricidad. Cuando la población tiene una mejora en su ingreso económico, las ventas de servicios y productos y aparatos electrodomésticos como: televisores, refrigeradores y aires acondicionados se dinamizan.

**Crecimiento poblacional.** Consiste en la tasa de crecimiento del número de habitantes dentro de un territorio. El crecimiento poblacional se encuentra estrechamente relacionado con la edificación de vivienda, servicios públicos, desarrollos comerciales, desarrollo industrial y en consecuencia más consumo de electricidad.
Estacionalidad. Los factores climáticos, temperaturas extremas, nevadas, lluvias, tienden a elevar la demanda de un Sistema Eléctrico de Potencia y con ella el consumo de energía eléctrica. En algunas situaciones, los factores climáticos, huracanes, fenómeno de El Niño, La Niña, sensación térmica, entre otros, ocasionan variaciones significativas en la demanda y consumo de energía eléctrica. 

**Electromovilidad.** La movilidad eléctrica a través de vehículos particulares y transporte público, mercancías, personas, local y foráneo, presenta una alternativa tangible para mejorar la movilidad y la reducción de emisiones al medio ambiente. En un Sistema Eléctrico aumenta el consumo de energía eléctrica y demanda por la carga del sistema de almacenamiento de energía de los vehículos eléctricos. 

En lo que respecta al PIB, el INEGI y la secretaria de economía, lo explican de forma muy elocuente.

![Captura de Pantalla 2024-09-26 a la(s) 2 42 26 p m](https://github.com/user-attachments/assets/c34da001-6fd4-4b01-865a-9acecbf77f06)
![Captura de Pantalla 2024-09-26 a la(s) 2 42 44 p m](https://github.com/user-attachments/assets/5f614a81-9f57-4157-8480-05596ac6f1a6)

Las consultas y obtención de las bases de datos se realizaron en las siguientes dependencias Gubernamentales:

![Captura de Pantalla 2024-09-26 a la(s) 2 43 27 p m](https://github.com/user-attachments/assets/e46511aa-a75e-4122-922c-e59bc51384e5)
![Captura de Pantalla 2024-09-26 a la(s) 2 43 39 p m](https://github.com/user-attachments/assets/d572d2b9-db69-4605-945d-f89b61273c5c)

## 2.	Preparación y limpieza de los datos.

La base de datos obtenida del INEGI, muestra los datos del PIB por entidad federativa durante el periodo de 2003 a 2022 a precios constantes tomando como referencia 2018, contiene 34 columnas (32 estados, total nacional y la correspondiente al periodo), incluye 21 filas (encabezado y 20 años del periodo 2003-2022). 

1. Periodos
2. PIB Nacional
3. PIB Aguascalientes
4. PIB Baja California
5. PIB Baja California Sur
6. PIB Campeche
7. PIB Coahuila
8. PIB Colima
9. PIB Chiapas
10. PIB Chihuahua
11. PIB CDMX
12. PIB Durango
13. PIB Guanajuato
14. PIB Guerrero
15. PIB Hidalgo
16. PIB Jalisco
17. PIB Estado de México
18. PIB Michoacan
19. PIB Morelos
20. PIB Nayarit
21. PIB Nuevo León
22. PIB Oaxaca
23. PIB Puebla
24. PIB Querétaro
25. PIB Qintana Roo
26. PIB San Luis Potosí
27. PIB Sinaloa
28. PIB Sonora
29. PIB Tabasco
30. PIB Tamaulipas
31. PIB Tlaxcala
32. PIB Veracruz
33. PIB Yucatan
34. PIB Zacatecas

Cabe mencionar que, los datos de 33 columnas son valores en moneda, en Millones de Pesos, la otra columna son valores numericos correspondiente al año. A continuación una muestra parcial de la base de datos.

![Captura de Pantalla 2024-09-26 a la(s) 2 56 50 p m](https://github.com/user-attachments/assets/fa11362a-1857-4a0f-8e49-af4546794479)


Referente a la base de datos obtenida de SENER, muestra los datos del consumo de energía eléctrica por entidad federativa durante el periodo de 2003 a 2016, contiene 34 columnas (32 estados, total nacional y la correspondiente al periodo), incluye 15 filas (encabezado y 14 años del periodo 2003-2016).

1. Periodos
2. Consumo E.E. Nacional
3. Consumo E.E. Aguascalientes
4. Consumo E.E. Baja California
5. Consumo E.E. Baja California Sur
6. Consumo E.E. Campeche
7. Consumo E.E. Coahuila
8. Consumo E.E. Colima
9. Consumo E.E. Chiapas
10. Consumo E.E. Chihuahua
11. Consumo E.E. CDMX
12. Consumo E.E. Durango
13. Consumo E.E. Guanajuato
14. Consumo E.E. Guerrero
15. Consumo E.E. Hidalgo
16. Consumo E.E. Jalisco
17. Consumo E.E. Estado de México
18. Consumo E.E. Michoacan
19. Consumo E.E. Morelos
20. Consumo E.E. Nayarit
21. Consumo E.E. Nuevo León
22. Consumo E.E. Oaxaca
23. Consumo E.E. Puebla
24. Consumo E.E. Querétaro
25. Consumo E.E. Qintana Roo
26. Consumo E.E. San Luis Potosí
27. Consumo E.E. Sinaloa
28. Consumo E.E. Sonora
29. Consumo E.E. Tabasco
30. Consumo E.E. Tamaulipas
31. Consumo E.E. Tlaxcala
32. Consumo E.E. Veracruz
33. Consumo E.E. Yucatan
34. Consumo E.E. Zacateca


Cabe mencionar que, los datos de 33 columnas son valores en número, Gigawatts-hora la otra columna son valores numericos correspondiente al año. Es importante señalar que, la base de datos del PIB por Estado muestra información del periodo 2003-2022, mientras que, la base de datos correspondiente al consumo de energía por Estado, solo durante el periodo 2003-2016, los consumos de energía durante el periodo 2017-2022 estan concentrados por bloques que incluyen más de un estado. Asimismo, con el objetivo de hacer coincidir bases de datos fue necesario trasponer datos correspondientes al consumo de energía eléctrica y convertir tablas xls a csv.  A continuación muestra parcial de BD.

![Captura de Pantalla 2024-09-26 a la(s) 2 58 51 p m](https://github.com/user-attachments/assets/63b569dd-7b31-4d00-954f-ef7dba193dec)


## 3.	Análisis exploratorio de datos (EDA).

Utilizando excel, se integraron las bases de datos para realizar cálculos estadísticos (media, mediana, desviación estandar y factor de correlación) y gráficas que reflejan la correlación entre PIB y consumo de energía. 

![Captura de Pantalla 2024-09-26 a la(s) 3 01 45 p m](https://github.com/user-attachments/assets/b9738e6a-7050-470d-ab8a-dc7b4a8b18fd)
![Captura de Pantalla 2024-09-26 a la(s) 3 02 10 p m](https://github.com/user-attachments/assets/944090df-95d3-4774-9783-e45e3566f201)
![Captura de Pantalla 2024-09-26 a la(s) 3 04 34 p m](https://github.com/user-attachments/assets/c0f97686-e8ac-4f11-945d-722f62081686)
![Captura de Pantalla 2024-09-26 a la(s) 3 04 54 p m](https://github.com/user-attachments/assets/d25660c2-75dc-468f-a757-f538b031aa41)
![Captura de Pantalla 2024-09-26 a la(s) 3 05 18 p m](https://github.com/user-attachments/assets/ab0091f5-1d9a-46a4-974a-d5e9f308202d)
![Captura de Pantalla 2024-09-26 a la(s) 3 05 44 p m](https://github.com/user-attachments/assets/379e557b-520d-4f44-add4-38dd25e29211)
![Captura de Pantalla 2024-09-26 a la(s) 3 06 09 p m](https://github.com/user-attachments/assets/5bf66059-a142-42f5-bc9a-3007de583aef)
![Captura de Pantalla 2024-09-26 a la(s) 3 06 30 p m](https://github.com/user-attachments/assets/a0a7dbc9-c993-4d0e-96be-d6bda8602627)
![Captura de Pantalla 2024-09-26 a la(s) 3 06 58 p m](https://github.com/user-attachments/assets/40267985-0745-4fd1-8e7c-acd3f3f349c3)
![Captura de Pantalla 2024-09-26 a la(s) 3 07 23 p m](https://github.com/user-attachments/assets/3e93e6cd-ed29-4d15-9870-9f8581f1fc78)
![Captura de Pantalla 2024-09-26 a la(s) 3 07 46 p m](https://github.com/user-attachments/assets/46554c1d-c51b-4cf9-bab2-1d6cde627aa1)
![Captura de Pantalla 2024-09-26 a la(s) 3 08 02 p m](https://github.com/user-attachments/assets/43fdf05c-2af0-4893-aa20-d3cfb10902ad)
![Captura de Pantalla 2024-09-26 a la(s) 3 08 16 p m](https://github.com/user-attachments/assets/9a2b1b4d-f22c-48a9-a9f1-35e92510253e)
![Captura de Pantalla 2024-09-26 a la(s) 3 08 37 p m](https://github.com/user-attachments/assets/3b9949ff-8988-47ce-bf78-4c76da618134)
![Captura de Pantalla 2024-09-26 a la(s) 3 09 06 p m](https://github.com/user-attachments/assets/21b713b0-8b3d-4d92-8285-e3e96fcc4bd7)
![Captura de Pantalla 2024-09-26 a la(s) 3 09 19 p m](https://github.com/user-attachments/assets/6a8e76f3-c63a-44d3-89ed-cf4f6a1910e4)
![Captura de Pantalla 2024-09-26 a la(s) 3 09 42 p m](https://github.com/user-attachments/assets/c1503b2d-d1c6-4c5d-bca0-944a0dff0260)


Ahora bien, aplicando lo visto en la 3ª sesión de python, prepare el archivo excel a csv, eliminando la columna de periodos y dejando para análisis el periodo 2003-2016. A continuación se muestran imágenes del código, análisis estádistico y mapa de calor para correlación entre PIB y consumo de energía eléctrica.

![Captura de Pantalla 2024-09-26 a la(s) 3 15 10 p m](https://github.com/user-attachments/assets/cc832ba7-2c66-4359-8f85-b0c7f6d5b801)
![Captura de Pantalla 2024-09-26 a la(s) 3 15 31 p m](https://github.com/user-attachments/assets/e01873a9-2fd1-4c0b-b41e-aba1d47542b1)
![Captura de Pantalla 2024-09-26 a la(s) 3 15 45 p m](https://github.com/user-attachments/assets/f60f8de7-9283-4bbf-86eb-0ad285f86af7)
![Captura de Pantalla 2024-09-26 a la(s) 3 16 21 p m](https://github.com/user-attachments/assets/2bde9971-aaa6-4b92-8d1e-97ee38a52d65)
![Captura de Pantalla 2024-09-26 a la(s) 3 16 35 p m](https://github.com/user-attachments/assets/549a690e-2a4c-4225-8905-402a06b8bb9d)


## 4.	Visualización de datos.

Si bien en los análisis estádisticos realizados en excel y la parte de python, se obtienen algunas gráficas, la vizualización completa la realice en tableau. A continuación se muestran imágenes de los dashboards elaborados. Cabe mencionar que, para incluir gráficas de los 32 estados y a nivel nacional, los agrupe de cuatro en cada dashboard. Utilice gráficas combinadas, barras para representar el consumo de energía eléctrica y líneas para indicar el PIB.

![Captura de Pantalla 2024-09-26 a la(s) 3 19 20 p m](https://github.com/user-attachments/assets/70cf306f-9af9-47e1-aa9b-bc77df9ddb41)
![Captura de Pantalla 2024-09-26 a la(s) 3 19 35 p m](https://github.com/user-attachments/assets/2c58d68a-8fa6-4b94-8397-30c0a0bd1785)
![Captura de Pantalla 2024-09-26 a la(s) 3 35 32 p m](https://github.com/user-attachments/assets/b73097eb-ba6e-4010-b745-e78f0a9a986d)
![Captura de Pantalla 2024-09-26 a la(s) 3 40 33 p m](https://github.com/user-attachments/assets/63448c4d-39db-4c7b-b1b2-0404b13f7a55)
![Captura de Pantalla 2024-09-26 a la(s) 3 40 46 p m](https://github.com/user-attachments/assets/e8752afd-40f8-4a22-84e8-1112d6256d30)
![Captura de Pantalla 2024-09-26 a la(s) 3 40 58 p m](https://github.com/user-attachments/assets/25292d96-df82-45f4-a4f1-513956d779a5)
![Captura de Pantalla 2024-09-26 a la(s) 3 41 20 p m](https://github.com/user-attachments/assets/9908fb3b-6d1a-47fc-a4bf-bed4d4aa98d5)
![Captura de Pantalla 2024-09-26 a la(s) 3 41 40 p m](https://github.com/user-attachments/assets/6e0e7a71-619f-4818-b649-223c6189a55c)
![Captura de Pantalla 2024-09-26 a la(s) 3 41 54 p m](https://github.com/user-attachments/assets/ca8e2453-e7e0-4778-90e1-4db8c278f45e)


## 5.	Interpretación y conclusiones

En las figuras de la 1.1 a la 1.3 se muestra la definición del PIB, como se obtiene y su segmentación. Asimismo, en las figuras 1.4 y 1.5 se indican las fuentes de la bases de datos. Se explica adicionalmente el porque se elegierón estas bases de datos.
La figuras 2.1 y 2.2, son muestra parcial de las fuentes de datos obtenidas. Asimismo, se comenta el tratamiento que se dío a las mismas.
En referencia a las figuras de la 3.1 a la 3.33, se muestran la base de datos parcial a nivel nacional y por cada entidad federativa, en donde se muestran datos estádisticos como son media, mediana, desviación estandar y factor de correlación entre el PIB y consumo de energía.

En particular las figuras 3.1 y 4.1, muestran el consumo de energía y el PIB a nivel nacional utilizando líneas y gráfica combinada. Cabe reiterar que, se dispone de datos del PIB para el periodo 2003-2022 y de consumo de energía del 2003 al 2016. En las gráficas se observa, una depresión en  2009-2010 a consecuencia de la pandemia de influenza y que provocó una contracción de la economía y en 2020 una mayor contracción a causa de la pandemia del COVID 19. Resalta la correlación positiva entre ambas curvas.

El PIB a nivel nacional al cierre de 2022 fue de $24,268,261.335 MDP, es decir $24.26 Billones de pesos, derivado del análisis se observa la mayor aportación al PIB fue de:

![Captura de Pantalla 2024-09-26 a la(s) 3 46 58 p m](https://github.com/user-attachments/assets/2c1f118c-6420-4033-9d2a-388f19721be1)

Referente al consumo nacional de energía de 2016 (último dato certero) fue de 218,072.29 GWH, derivado del análisis se observa la mayor aportación al consumo fue de:

![Captura de Pantalla 2024-09-26 a la(s) 3 48 00 p m](https://github.com/user-attachments/assets/75f0dc5f-f46e-4732-a6b8-e2dba5eeb118)

Ahora bien, en las gráficas 3.1 a 3.33 y 4.1 a 4.9 se presenta entre otras cosas la correlación entre el PIB y el consumo de energía eléctrica a nivel nacional y los 32 estados (incluyendo la CDMX), merecen atención especial dos casos donde la correlación es negativa y casi cero.

**Estado de Campeche:** En las figuras 3.5 y 4.8 muestran una correlación negativa y se observa que a partir de 2003 el PIB tiene una tendencia a la baja, caso contrario al consumo de energía que tiende a incrementarse desde 2003. La causa de la caida en el PIB de manera constante durante los últimos años, es por la baja producción petrolera, el PIB dependía en un 80% de la actividad petrolera, por ello la economía del estado ha colapsado y se adapta al nuevo entorno económico. 

**Estado de Michoacan:** Las figuras 3.17 y 4.4 muestran una correlación minima y un comportamiento del PIB incrementandose de manera natural desde 2003, con las caidas en 2009 y 2020 causadas por las pandemias de influenza y COVID-19 respectivamente. Ahora bien, el consumo de energía presenta una caida muy pronunciada. 
Al ser un estado poco industrializado, prácticamente solo la industria siderúrgica del puerto Lázaro Cárdenas es el principal impulsor. La caida en el consumo en 2009 interrumpió la tendencia al alza que se venía presentando y la recuperación aún no ha llegado, esto por diversos factores, la inseguridad y las huelgas que aquejan a esa industria. 

A continuación se muestra un mapa que refleja el porcentaje de participación en el PIB nacional de cada entidad federativa al cierre de 2022.

![Captura de Pantalla 2024-09-26 a la(s) 3 50 57 p m](https://github.com/user-attachments/assets/f7846e96-293b-4468-a080-cf9c5c3f60a9)


A continuación se muestra un mapa que refleja el consumo de energía eléctrica en GWH en el ámbito regional al cierre de 2022.

![Captura de Pantalla 2024-09-26 a la(s) 3 51 35 p m](https://github.com/user-attachments/assets/2d512b92-a2c7-4c40-91f8-00776aa36b4f)

## CONCLUSIONES

**LECCIONES APRENDIDAS**

1. Como resultado del análisis podemos concluir que el Comportamiento del producto interno bruto (PIB) y el consumo de energía eléctrica en una región y durante un periodo, presentan una correlación positiva, hay contadas excepciones que no se cumple y donde la causa raíz es un evento atipico que influya en el comportamiento de las variables mencionadas. La figura 5.3 muestra un histograma formado con los factores de correlación obtenidos en el análisis estádistic.

2. Con base a lo anterior, podemos afirmar que sin energía eléctrica para actividades primaias, secundarias o terciarias no hay crecimiento económico, no hay generación de empleos y en si, generación de riqueza en una región.

3. La relocalización de empresas que actualmente estan o estaban en China y han optado por instalarse en nuestro país (NEOSHORING), buscan instalarse en sitios donde se disponga de entre otras cosas, de red eléctrica para formar parques industriales que satisfagan la demanda de energía eléctrica. Asimismo, buscan condiciones de servicios básicos como agua, seguridad, certidumbre jurídica y acceso a medios de transporte con rutas a Estados Unidos de America principalmente.

4. México dispone de un potencial para generar energías limpias (Sol y viento), la figura 5.4 muestra los mapas por separado. Asimismo, el mapa final de la figura 5.4, muestra el pronostico de crecimiento por región del consumo de energía eléctrica. 
 


![Captura de Pantalla 2024-09-26 a la(s) 3 52 37 p m](https://github.com/user-attachments/assets/ec85e54c-3994-4bb4-886e-d10a22e5a90b)


**PASOS A SEGUIR**

1. Con la entrada de la nueva administración, se espera que esten disponibles nuevamente las bases de datos del consumo de energía eléctrica por estados y municipios.

2. Con base a lo anterior, realizar un nuevo análisis y contrastarlo con los mapas actuales donde se indique el potencial de energías limpias (Solar y eólica).

3. El país requiere de energía para estar en movimiento, si el próximo Gobierno decide hacer inversiones públicas, privadas o mixtas, bienvenidas.










