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

---

Bienvenido a la página web del proyecto **Ciudades Sostenibles y Saludables**

Este proyecto tiene como objetivo cuantificar y evaluar en qué medida las grandes ciudades españolas cuentan con diseños urbanos y sistemas de movilidad sostenibles y saludables.

En esta página web encontraréis información relativa al planteamiento general del [**proyecto**](https://gratet.github.io/ciudades-leonardo/project/), 
su [**metodología**](https://gratet.github.io/ciudades-leonardo/metodologia/), los [**principales resultados**](https://gratet.github.io/ciudades-leonardo/resultados/), 
así como una página desde la que os podréis [**descargar material derivado del proyecto**](https://gratet.github.io/ciudades-leonardo/descargas/).



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
  text-align: center;
  }
  
  .styled-image {
  max-width: 100%;
  display: block;
  margin: 0 auto;
  border-radius: 8px; /* Agregado para bordes redondeados */
  box-shadow: 0 0px 0px rgba(0, 0, 0, 0); /* Agregado para sombra */
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
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-mc.svg" alt="Mapa 1">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/comercios-cotidianos/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-cc.svg" alt="Mapa 2">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/transporte-publico/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-tp.svg" alt="Mapa 3">
      </a>
    </td>
  </tr>
</table>
<div style="max-width: 66%; margin: auto;">
<table>
  <tr>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/espacios-publicos-abiertos/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-aos.svg" alt="Mapa 3">
      </a>
    </td>
    <td>
      <a href="https://gratet.github.io/ciudades-leonardo/caminabilidad/" target="_blank">
        <img class="styled-image" src="https://gratet.github.io/ciudades-leonardo/images/img_cos/index-ag.svg" alt="Mapa 5">
      </a>
    </td>
  </tr>
</table>
</div>
</body>