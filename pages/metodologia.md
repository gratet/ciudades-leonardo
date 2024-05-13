---
permalink: "/metodologia/"
layout: page-fullwidth
breadcrumb: true
#sidebar: right
title: "Metodología"
meta_title: "Metodología"
subheadline: ""

teaser: "" 

meta_teaser: ""

header:
    image_fullwidth: headers/cl_header_index.png
    background-color: "#19294d"
    caption: "Barcelona (Xavier Delclòs)"

---

### Ciudades analizadas 


Este estudio se centra en el cálculo de indicadores en las diez ciudades más pobladas de España. Para ello, en primer lugar, se identificaron los **diez municipios con mayor población según el Censo de Población y Viviendas de 2021**,
elaborado por el Instituto Nacional de Estadística. En segundo lugar, y para definir la extensión espacial y el volumen demográfico de las áreas urbanas reales de cada una de las ciudades, se identificó el perímetro urbano según
la información del Global Human Settlement Layer, concretamente la información relativa a centros urbanos en todo el mundo en su actualización de 2020, elaborado por el **[Joint Research Centre  de la Comisión Europea](https://joint-research-centre.ec.europa.eu/index_en){:target="_blank"}**.

Como resultado, en este proyecto se analizan las áreas urbanas de **Barcelona, Bilbao, Las Palmas de Gran Canaria, Madrid, Málaga, Murcia, Palma, Sevilla, Valencia y Zaragoza**, tal y como se muestra en el siguiente mapa. 

<figure>
  <img src="https://gratet.github.io/ciudades-leonardo/images/img_cos/situacio_def.png" alt="Mapa 1" style="max-width: 100%; display: block; margin: 0 auto;">
    <figcaption style="text-align: center"><strong>Mapa 1.</strong>  Ciudades caso de estudio.</figcaption>
</figure>

Los datos relativos a la extensión urbana de cada ciudad analizada y su volumen demográfico se presentan en la **Tabla 1**. En conjunto, las ciudades analizadas cubren una extensión de **1.637,4 km<sup>2</sup>**, incluyendo un total de 166 municipios,
y albergan una población de **más de 14 millones de habitantes**. Madrid y Barcelona, con 4,9 y 4,3 millones de habitantes respectivamente son las dos principales ciudades analizadas y de mayor extensión, seguidas de Valencia, con 1,3
millones, Sevilla (764 mil), Bilbao (663 mil), Málaga (651 mil), Zaragoza (407 mil), Palma (362 mil) y, finalmente, Las Palmas de Gran Canaria (358 mil). El número de municipios analizados varía substancialmente entre ciudades.
Destaca el caso de Barcelona, con información para 50 municipios, seguidos por Valencia. Madrid, pese a ser la ciudad con mayor extensión geográfica, incluye tan solo 21 municipios. Las áreas urbanas con un menor nombre de entidades
municipales analizadas son las Palmas de Gran Canaria y Zaragoza, y presentan extensiones geográficas similares, alrededor de los 60 km<sup>2</sup>.

<center>
<!-- Taula 1 -->
<iframe src="https://gratet.github.io/ciudades-leonardo/tablas/tabla_1.htm" width="100%" height="260" frameborder="0"></iframe>
    <figcaption style="text-align: center"><strong>Tabla 1.</strong>  Descripción de las ciudades analizadas.</figcaption>
</center>

### Software y datos 


Este proyecto se basa en el uso del software **[Global Healthy and Sustainable City Indicators (GHSCI)](https://github.com/global-healthy-liveable-cities/global-indicators){:target="_blank"}**, desarrollado para el cálculo y la 
generación de informes de indicadores espaciales relacionados con la salud y la sostenibilidad a partir de las características del entorno construido, la distribución de la población y las características del transporte público 
utilizando, en este caso, datos abiertos (aunque el software admite también la incorporación de datos de otro tipo).


El análisis se ha realizado utilizando la versión 4.4.8 GHSCI con la imagen del Docker (entorno que permite empaquetar y distribuir la aplicación con todas sus dependencias) correspondiente. La imagen Docker trae consigo mismo un 
listado de plataformas, todas ellas de código abierto. Entre ellas encontramos Linux, Python, OSMnx, NetworkX, GeoPandas, Pandas, Shapely, Fiona, Rasterio, GDAL, Pyproj y otros. Además de esta imagen, también se utiliza una imagen 
pgRouting Docker, para ejecutar una base de datos Postgres SQL con las extensiones POstGIS y pgRouting pudiendo soportar la gestión de todos los datos y análisis necesarios.

Los datos utilizados para este análisis son de naturaleza abierta, siguiendo la filosofía del software utilizado, basado en código abierto, y por lo tanto los datos también son abiertos tal y como establece el propio programa. 
Para la utilización del software se han configurado previamente cada una de las ciudades con los datos correspondientes, mostrados en la **Tabla 2**. El primero de ellos es la definición del área de estudio, la cual se ha definido a partir 
de la selección de los municipios colindantes con el área urbana definida por la capa de áreas urbanas hecha por el  **[Global Human Settlement Layer, Urban Centres  Database (GHS UCDB)](https://data.jrc.ec.europa.eu/dataset/53473144-b88c-44bc-b4a3-4583ed1f547e){:target="_blank"}**. 
Esta capa de centros urbanos define las áreas urbanas a partir de celdas de 1 km de resolución con criterios de densidad, en la que se usa un umbral mínimo de 1.500 hab/km<sup>2</sup> para que un área sea considerada como parte de un centro urbano.


<center>
<!-- Taula 2 -->
<iframe src="https://gratet.github.io/ciudades-leonardo/tablas/tabla_2.htm" width="100%" height="200" frameborder="0"></iframe>
    <figcaption style="text-align: center"><strong>Tabla 2.</strong>  Datos y fuentes originales.</figcaption> <br>
</center>


En relación a la distribución de la población, se utiliza una capa ráster de 100 m de resolución proveniente del  **[Global Human Settlement Layer](https://data.jrc.ec.europa.eu/dataset/53473144-b88c-44bc-b4a3-4583ed1f547e){:target="_blank"}**. 
Los datos del entorno construido, de la infraestructura viaria, así como las tiendas y supermercados y espacios públicos provienen de OpenStreetMap. Esta contiene datos globales accesibles al público y con gran cantidad de datos atribuidos por 
la propia comunidad, a partir de los cuáles se pueden identificar los elementos mencionados anteriormente.

Finalmente, los datos GTFS (General Transit Feed Specification) se corresponden con un estándar de formato de datos que define la estructura y la semántica para describir información de transporte colectivo, como horarios, rutas y paradas, facilitando 
la interoperabilidad entre sistemas de información y operadores de transporte público. Este tipo de datos se han utilizado para el cálculo de los indicadores relativos al acceso a transporte público. No obstante, en esta versión preliminar del informe 
se recomienda precaución al interpretar los resultados, puesto éstos están pendientes de revisión pormenorizada, especialmente considerando que la disponibilidad y compleción de los datos GTFS puede variar según el operador.


### Indicadores y cálculos

Este proyecto se ha basado en el cálculo de una batería de indicadores relativos al diseño urbano y a los niveles de accesibilidad a pie en las ciudades analizadas. Concretamente, se han construido indicadores en los siguientes temas:

1. indicadores **demográficos** y de **forma urbana**. Es el caso del cálculo de la superficie de cada ciudad, la estimación de población, la densidad de población, así como la densidad de intersecciones.
2. Indicadores de **acceso a servicios básicos** como tiendas de alimentación y otros tipos de comercio cotidiano. Tanto en estos indicadores como en los siguientes relativos a la accesibilidad, se ha usado un radio de 500 metros a pie por la red peatonal de cada ciudad. 
3. Indicadores de **acceso a transporte colectivo** según su nivel de frecuencia.
4. Indicadores de **acceso a espacios públicos abiertos** según la dimensión de su superficie. 
5. Un indicador de **accesibilidad general** calculado a partir de los indicadores de acceso mencionados anteriormente. 
6. Un índice de **caminabilidad**, que indica el grado en el que el entorno construido favorece o limita la movilidad a pie. Este índice se construye a partir de la densidad de población, la densidad de intersecciones, y el indicador de accesibilidad general anteriormente descrito.

La **Figura 1** ilustra el flujo simplificado de procesos utilizado para calcular los indicadores, que consta de las siguientes cuatro etapas:

1. **Recolección de datos**: Adquisición y recopilación de los datos relevantes y necesarios para el análisis, provenientes de las fuentes mencionadas, asegurando la calidad y precisión de los datos. 
2. **Configuración de parámetros y definición de la región de estudio**: Establecimiento de los criterios, variables y límites geográficos que guiarán el análisis, permitiendo delimitar la extensión, características específicas y datos de la zona a estudiar. 
3. **Procesamiento de los datos de entrada**: Transformación y preparación de los datos recolectados para su análisis. 
4. **Procesamiento de las estimaciones del muestreo y agregación de indicadores**: Aplicación de métodos estadísticos y algoritmos para calcular estimaciones a partir de una muestra de datos y la configuración de cada ciudad, para la generación de los indicadores.

<figure>
<!-- Figura 1 -->
<img src="https://gratet.github.io/ciudades-leonardo/images/svg_files/figura_1-01.png" height="230" alt="Figura 1" /><br>
    <figcaption style="text-align: center"><strong><br>Figura 1.</strong>  Malla ráster de resolución de 100m.</figcaption>
</figure>

Los indicadores se calculan a nivel de área urbana y a una resolución de 100 metros, utilizando una malla ráster que incorpora la estimación de la población ya mencionada. La **Figura 2** muestra una imagen de satélite de la ciudad de Barcelona, en la que se muestra
un ejemplo de la malla de 100 metros de resolución utilizada para el cálculo de los indicadores. Finalmente, en la **Tabla 3** se muestra el detalle de los indicadores concretos calculados.


<figure>
   <img src="https://gratet.github.io/ciudades-leonardo/images/img_cos/figura_2.png" alt="Figura 2" style="max-width: 300px; display: block; margin: 0 auto;">
    <figcaption style="text-align: center"><strong><br> Figura 2. </strong>  Malla ráster de resolución de 100m.</figcaption>
</figure>

<center>
<!-- Taula 3 -->
<iframe src="https://gratet.github.io/ciudades-leonardo/tablas/tabla_3.htm" width="100%" height="400" frameborder="0"></iframe>
    <figcaption style="text-align: center"><strong> Tabla 3. </strong>  Datos e indicadores calculados por el software. </figcaption>
</center>
<br>
En la obtención de resultados el software genera diferentes ficheros de salida, tanto en formato gpkg como en formato csv, ambos con los indicadores calculados. Para más detalle tanto del cálculo de cada uno de los 
indicadores como del proceso seguido por el software se puede consultar la documentación disponible en el repositorio correspondiente.

