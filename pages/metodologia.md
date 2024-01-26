---
permalink: "/metodologia/"
layout: page-fullwidth
breadcrumb: true
#sidebar: right
title: "Metodología"
meta_title: "Metodología"
subheadline: ""

teaser: "Algun text?" 

meta_teaser: ""

header: no

---

### Ciudades analizadas

Este estudio se centra en el cálculo de indicadores en las diez ciudades más pobladas de España. Para ello, en primer lugar, se identificaron los **diez municipios con mayor población según el Censo de Población y Viviendas de 2021**,
elaborado por el Instituto Nacional de Estadística. En segundo lugar, y para definir la extensión espacial y el volumen demográfico de las áreas urbanas reales de cada una de las ciudades, se identificó el perímetro urbano según
la información del Global Human Settlement Layer, concretamente la información relativa a centros urbanos en todo el mundo en su actualización de 2020, elaborado por el Joint Research Centre  de la Comisión Europea (4). 

Como resultado, en este proyecto se analizan las áreas urbanas de **Barcelona, Bilbao, Las Palmas de Gran Canaria, Madrid, Málaga, Murcia, Palma, Sevilla, Valencia y Zaragoza**, tal y como se muestra en el siguiente mapa. 

<!--mapa 1-->
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ejemplo de Inserción de Imagen HTML</title>
  <style>
    img {
      display: block;
      margin: 0 auto;
      width: 700px;
    }
  </style>
</head>
<body>

<!-- Aquí se inserta la imagen -->
<img src="/images/img_cos/situacio_def.png" alt="Descripción de la imagen">

<!-- https://gratet.github.io/ciudades-leonardo/ -->

</body>

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ejemplo de Texto Centrado HTML</title>
  <style>
    .centrado {
      text-align: center;
    }
  </style>
</head>
<body>

<p class="centrado">Mapa 1. Ciudades caso de estudio </p>

<!-- Resto del contenido -->

</body>
</html>



Los datos relativos a la extensión urbana de cada ciudad analizada y su volumen demográfico se presentan en la **Tabla 1**. En conjunto, las ciudades analizadas cubren una extensión de **1.637,4 km<sup>2</sup>**, incluyendo un total de 166 municipios,
y albergan una población de **más de 14 millones de habitantes**. Madrid y Barcelona, con 4,9 y 4,3 millones de habitantes respectivamente son las dos principales ciudades analizadas y de mayor extensión, seguidas de Valencia, con 1,3
millones, Sevilla (764 mil), Bilbao (663 mil), Málaga (651 mil), Zaragoza (407 mil), Palma (362 mil) y, finalmente, Las Palmas de Gran Canaria (358 mil). El número de municipios analizados varía substancialmente entre ciudades.
Destaca el caso de Barcelona, con información para 50 municipios, seguidos por Valencia. Madrid, pese a ser la ciudad con mayor extensión geográfica, incluye tan solo 21 municipios. Las áreas urbanas con un menor nombre de entidades
municipales analizadas son las Palmas de Gran Canaria y Zaragoza, y presentan extensiones geográficas similares, alrededor de los 60 km<sup>2</sup>.

<center>
<!-- Taula 1 -->
<iframe src="https://gratet.github.io/ciudades-leonardo/tablas/tabla_1.html" width="100%" height="280" frameborder="0"></iframe>
</center>

### Software y datos 


Este proyecto se basa en el uso del software **[Global Healthy and Sustainable City Indicators (GHSCI)](https://github.com/global-healthy-liveable-cities/global-indicators){:target="_blank"}** (3), desarrollado para el cálculo y la 
generación de informes de indicadores espaciales relacionados con la salud y la sostenibilidad a partir de las características del entorno construido, la distribución de la población y las características del transporte público 
utilizando, en este caso, datos abiertos (aunque el software admite también la incorporación de datos de otro tipo).


El análisis se ha realizado utilizando la versión 4.4.8 GHSCI con la imagen del Docker (entorno que permite empaquetar y distribuir la aplicación con todas sus dependencias) correspondiente. La imagen Docker trae consigo mismo un 
listado de plataformas, todas ellas de código abierto. Entre ellas encontramos Linux, Python, OSMnx 5, NetworkX, GeoPandas, Pandas, Shapely, Fiona, Rasterio, GDAL, Pyproj y otros. Además de esta imagen, también se utiliza una imagen 
pgRouting Docker, para ejecutar una base de datos Postgres SQL con las extensiones POstGIS y pgRouting pudiendo soportar la gestión de todos los datos y análisis necesarios.

Los datos utilizados para este análisis son de naturaleza abierta, siguiendo la filosofía del software utilizado, basado en código abierto, y por lo tanto los datos también son abiertos tal y como establece el propio programa. 
Para la utilización del software se han configurado previamente cada una de las ciudades con los datos correspondientes, mostrados en la **Tabla 2**. El primero de ellos es la definición del área de estudio, la cual se ha definido a partir 
de la selección de los municipios colindantes con el área urbana definida por la capa de áreas urbanas hecha por el Global Human Settlement Layer, Urban Centres  Database (GHS UCDB) (4). Esta capa de centros urbanos define las áreas urbanas 
a partir de celdas de 1 km de resolución con criterios de densidad, en la que se usa un umbral mínimo de 1.500 hab/km<sup>2</sup> para que un área sea considerada como parte de un centro urbano.


<center>
<!-- Taula 2 -->
<iframe src="https://gratet.github.io/ciudades-leonardo/tablas/tabla_2.htm" width="100%" height="280" frameborder="0"></iframe>
</center>


En relación a la distribución de la población, se utiliza una capa ráster de 100 m de resolución proveniente del Global Human Settlement Layer (6). Los datos del entorno construido, de la infraestructura viaria, así como las tiendas y supermercados 
y espacios públicos provienen de OpenStreetMap. Esta contiene datos globales accesibles al público y con gran cantidad de datos atribuidos por la propia comunidad, a partir de los cuáles se pueden identificar los elementos mencionados anteriormente.

### Referencias
- 3
- 4
- 5
- 6