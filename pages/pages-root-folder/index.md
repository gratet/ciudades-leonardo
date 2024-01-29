---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: headers/cl_header_index.png
background-color: "#19294d"
caption: "Barcelona (Xavier Delclòs)"

#widget1:
#  title: "Notícia en el diario digital de la URV"
#  url: 'https://diaridigital.urv.cat/es/diseno-urbano-ciudades-estilo-vida-saludable/'
#  image: widget_noticia_diari_urv.png
#  text: 'El diseño urbano de las 10 ciudades españolas tiene les condiciones necesarias para un estilo de vida saludable.'

#widget2:
#  title: "Resultados preliminares"
#  url: 'https://gratet.github.io/ciudades-leonardo/files/informe_leonardo_preliminar_enero24.pdf'
#  image: widget_informe preliminar.png
#  text: 'Disponible el primer informe con los resultados preliminares del proyecto. En este documento se presentan los principales resultados a nivel gráfico y cartográfico para cada uno de los indicadores.'


permalink: /index.html
homepage: true
breadcrumb: true
sidebar: right

#
# Gallery
#
gallery:
- image_url: DSC_0001.JPG

#
# Styling
#
image:
thumb:
#
# Metainformation & Customization
#

---


  <h1>Ciudades sostenibles y saludables</h1>
  <h2>Una aproximación open-source para el cálculo de indicadores sobre diseño urbano y de movilidad para las grandes ciudades españolas</h2> <br>
  <p>
¡Bienvenido a la página web del proyecto Ciudades Sostenibles y Saludables! Un proyecto financiado por la Fundación BBVA. En esta página, puedes consultar los principales resultados, así como 
la metodología, y descargar los informes y los datos disponibles del proyecto.
  </p>
  <p>
    Encuentra datos <a " href="https://www.movactiva.es/determinantes-de-la-movilidad-activa/caminabilidad">Densidades Urbanas</a>, <a style="color: burlywood;" 
href="https://www.movactiva.es/determinantes-de-la-movilidad" </a> y análisis detallados sobre Densidades Urbanas, Ciclabilidad, Espacios Verdes, Vitalidad Urbana y la Ciudad de los 15 Minutos. 
Somos tu fuente confiable de información para un estilo de vida más saludable y sostenible en entornos urbanos.
    <p>
  </p>


<html lang="es">
<head>
  <style>
    body {
      font-family: Arial, sans-serif;
    }

    table {
      border-collapse: collapse;
      width: 100%;
    }

    td {
      margin: 2%;
      text-align: center;
    }

    .styled-image {
      max-width: 100%;
      display: block;
      margin: 0 auto;
      border-radius: 8px; /* Agregado para bordes redondeados */
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1); /* Agregado para sombra */
      transition: transform 0.3s ease-in-out;
    }

    .styled-image:hover {
      transform: scale(1.05);
    }
  </style>
</head>



<body>

<table>
  <tr>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/caracterizacion/">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-mc.png" alt="Mapa 1">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/comercios-cotidianos/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-cc.png" alt="Mapa 2">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/transporte-publico/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-tp.png" alt="Mapa 3">
      </a>
    </td>
  </tr>
  <tr>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/espacios-publicos-abiertos/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-aos.png" alt="Mapa 3">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/caminabilidad/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-ag.png" alt="Mapa 5">
      </a>
    </td>
  </tr>
</table>

</body>






{% include gallery %}