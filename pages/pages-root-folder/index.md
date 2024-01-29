---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: page
header:
  image_fullwidth: headers/cl_header_index.png
background-color: "#19294d"
caption: "Barcelona (Xavier Delclòs)"

widget1:
  title: "Notícia en el diario digital de la URV"
  url: 'https://diaridigital.urv.cat/es/diseno-urbano-ciudades-estilo-vida-saludable/'
  image: widget_noticia_diari_urv.png
  text: 'El diseño urbano de las 10 ciudades españolas tiene les condiciones necesarias para un estilo de vida saludable.'

widget2:
  title: "Resultados preliminares"
  url: 'https://gratet.github.io/ciudades-leonardo/files/informe_leonardo_preliminar_enero24.pdf'
  image: widget_informe preliminar.png
  text: 'Disponible el primer informe con los resultados preliminares del proyecto. En este documento se presentan los principales resultados a nivel gráfico y cartográfico para cada uno de los indicadores.'


permalink: /index.html
homepage: true
breadcrumb: true
sidebar: right

#
# Gallery
#
gallery:
- image_url: https://gratet.github.io/ciudades-leonardo/images/img_cos/situacio_def.png
  caption: Great images by Unsplash.com
- image_url: gallery-example-2.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-3.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-1.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-2.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-3.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-2.jpg
  caption: Great images by Unsplash.com
- image_url: gallery-example-3.jpg
  caption: Great images by Unsplash.com

#
# Styling
#
image:
thumb:
#
# Metainformation & Customization
#

---

# Styling


{% include gallery %}

