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
Iniciemos con lo referente al consumo de energía eléctrica. El consumo final de energía eléctrica se refiere a la energía eléctrica vendida a través de CFE suministradores y esquemas de autoabastecimiento. El consumo final se compone por seis sectores tarifarios: residencial, comercial, servicios, bombeo agrícola, empresa mediana y gran industria, estos últimos concentran el 37.4% y 23.7%, respectivamente. En tercer lugar, está el sector residencial con 26.3%, le siguen el comercial, agrícola y servicios con 5.8%, 5.4% y 1.4%, en ese orden. 

Es importante señalar que, la planeación del desarrollo del sector eléctrico parte del análisis del consumo de electricidad para el mediano y largo plazo. Ello permite diseñar de manera óptima el desarrollo y la expansión de capacidad de las actividades de generación, transmisión, distribución y comercialización de energía eléctrica.
El crecimiento del consumo de energía eléctrica está sujeto a diversos factores entre los más determinantes se encuentran: 

**Crecimiento económico.** Consiste en la tasa de crecimiento del Producto Interno Bruto (PIB). Si el crecimiento de la economía de una localidad o región aumenta, en consecuencia, también lo hace el consumo y la demanda de electricidad. Cuando la población tiene una mejora en su ingreso económico, las ventas de servicios y productos y aparatos electrodomésticos como: televisores, refrigeradores y aires acondicionados se dinamizan.

**Crecimiento poblacional.** Consiste en la tasa de crecimiento del número de habitantes dentro de un territorio. El crecimiento poblacional se encuentra estrechamente relacionado con la edificación de vivienda, servicios públicos, desarrollos comerciales, desarrollo industrial y en consecuencia más consumo de electricidad.
Estacionalidad. Los factores climáticos, temperaturas extremas, nevadas, lluvias, tienden a elevar la demanda de un Sistema Eléctrico de Potencia y con ella el consumo de energía eléctrica. En algunas situaciones, los factores climáticos, huracanes, fenómeno de El Niño, La Niña, sensación térmica, entre otros, ocasionan variaciones significativas en la demanda y consumo de energía eléctrica. 

**Electromovilidad.** La movilidad eléctrica a través de vehículos particulares y transporte público, mercancías, personas, local y foráneo, presenta una alternativa tangible para mejorar la movilidad y la reducción de emisiones al medio ambiente. En un Sistema Eléctrico aumenta el consumo de energía eléctrica y demanda por la carga del sistema de almacenamiento de energía de los vehículos eléctricos. 

![Captura de Pantalla 2024-09-26 a la(s) 2 42 26 p m](https://github.com/user-attachments/assets/c34da001-6fd4-4b01-865a-9acecbf77f06)
![Captura de Pantalla 2024-09-26 a la(s) 2 42 44 p m](https://github.com/user-attachments/assets/5f614a81-9f57-4157-8480-05596ac6f1a6)

## Las consultas y obtención de las bases de datos se realizaron en las siguientes dependencias Gubernamentales:

![Captura de Pantalla 2024-09-26 a la(s) 2 43 27 p m](https://github.com/user-attachments/assets/e46511aa-a75e-4122-922c-e59bc51384e5)
![Captura de Pantalla 2024-09-26 a la(s) 2 43 39 p m](https://github.com/user-attachments/assets/d572d2b9-db69-4605-945d-f89b61273c5c)

## 2.	Preparación y limpieza de los datos.

La base de datos obtenida del INEGI, muestra los datos del PIB por entidad federativa durante el periodo de 2003 a 2022 a precios constantes tomando como refrencia 2018, contiene 34 columnas (32 estados, total nacional y la correspondiente al periodo), incluye 21 filas (encabezado y 20 años del periodo      2003-2022). 

Cabe mencionar que, los datos de 33 columnas son valores en moneda, en Millones de Pesos, la otra columna son valores numericos correspondiente al año. A continuación una muestra parcial de la base de datos.

![Captura de Pantalla 2024-09-26 a la(s) 2 56 50 p m](https://github.com/user-attachments/assets/fa11362a-1857-4a0f-8e49-af4546794479)


Referente a la base de datos obtenida de SENER, muestra los datos del consumo de energía eléctrica por entidad federativa durante el periodo de 2003 a 2016, contiene 34 columnas (32 estados, total nacional y la correspondiente al periodo), incluye 15 filas (encabezado y 14 años del periodo 2003-2016).

Cabe mencionar que, los datos de 33 columnas son valores en número, Gigawatts-hora la otra columna son valores numericos correspondiente al año. Es importante señalar que, la base de datos del PIB por Estado muestra información del periodo 2003-2022, mientras que, la base de datos correspondiente al consumo de energía por Estado, solo durante el periodo 2003-2016, los consumos de energía durante el periodo 2017-2022 estan concentrados por bloques que incluyen más de un estado. Asimismo, con el objetivo de hacer coincidir bases de datos fue necesario trasponer datos correspondientes al consumo de energía eléctrica y convertir tablas xls a csv.  A continuación muestra parcial de BD.

![Captura de Pantalla 2024-09-26 a la(s) 2 58 51 p m](https://github.com/user-attachments/assets/63b569dd-7b31-4d00-954f-ef7dba193dec)


## 3.	Análisis exploratorio de datos (EDA).

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

