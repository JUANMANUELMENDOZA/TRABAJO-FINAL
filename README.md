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
