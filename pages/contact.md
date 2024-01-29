---
layout              : page-fullwidth
title               : "Contacta con el equipo"
meta_title          : ""
subheadline         : ""
teaser              : ""
permalink           : "/contact/"
breadcrumb: true

header:
    image_fullwidth: headers/cl_header_index.png
    background-color: "#262930"
    caption: "Barcelona (Xavier Delclòs)"
---
<div class="row">

<div class="small-12 large-4 columns">

<h4>Investigador principal</h4>
<a href="mailto: xavier.delclos@urv.cat?subject=[Ciudades Sostenibles] " title="xavier.delclos@urv.cat">Dr. Xavier Delclòs Alió</a><br>xavier.delclos@urv.cat <br> Investigador Postdoctoral Ramón y Cajal<br>Grup de Recerca en Anàlisi Territorial i Estudis Turístics (GRATET)<br>








<h4>Dirección postal:</h4>
<a href="https://www.geografia.urv.cat/ca/">Departament de Geografia, Facultat de Turisme i Geografia</a><br>
<a href="https://www.urv.cat/">Universitat Rovira i Virgili</a><br>
C/ Joanot Martorell, 15 <br>
43480 - Vila-seca (Tarragona) <br>
España

</div>

<div class="small-12 large-8 columns">


<html>
<head>
<link rel="stylesheet" href="https://unpkg.com/leaflet@1.7.1/dist/leaflet.css" integrity="sha512-xodZBNTC5n17Xt2atTPuE1HxjVMSvLVW9ocqUKLsCC5CXdbqCmblAshOMAS6/keqq/sMZMZ19scR4PsZChSR7A==" crossorigin=""/>
<script src="https://unpkg.com/leaflet@1.7.1/dist/leaflet.js" integrity="sha512-XQoYMqMTK8LvdxXYG3nZ448hOEQiglfqkJs1NOQV44cWnUrBc8PkAOcXy20w0vlaXaVUearIOBhiXZ5V3ynxwA==" crossorigin=""></script>


	
</head>
<body>
<div id="mapid" style="width: 100%; height: 400px;"></div>
<script>

       var mymap = L.map('mapid', {
            zoomControl:true, maxZoom:18, minZoom:2
        }).fitBounds([[41.10188530474122,1.146026661908157],[41.103289521850144,1.149400214972932]]);


	L.tileLayer('http://{s}.google.com/vt/lyrs=s,h&x={x}&y={y}&z={z}', {
	attribution: 'Google Maps',
        maxZoom: 18,
        minZoom: 2,
        subdomains: ['mt0', 'mt1', 'mt2', 'mt3'],
    }).addTo(mymap);

	L.marker([41.10248, 1.14790]).addTo(mymap)
		.bindPopup("<b>Facultat de Turismo y Geografía</b><br />Universitat Rovira i Virgili").openPopup();

	var popup = L.popup();

</script>

</body>
</html>

