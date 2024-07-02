---
permalink: /contact/
title: "Contact"
author_profile: false
---
<head>
 <link rel="stylesheet" href="https://unpkg.com/leaflet@1.9.4/dist/leaflet.css"
     integrity="sha256-p4NxAoJBhIIN+hmNHrzRCf9tD/miZyoHS5obTRR9BMY="
     crossorigin=""/>
 <script src="https://unpkg.com/leaflet@1.9.4/dist/leaflet.js"
    integrity="sha256-20nQCchB9co0qIjJZRGuk2/Z9VM+kNiyxNV1lvTlZBo="
    crossorigin=""></script>
 <style>
    #map { height: 330px; }
 </style>
</head>

<i class="fa-li fas fa-map-marker fa-2x" aria-hidden="true">
</i>
TEL Gebäude, 6. Stock
<br>
<a href="https://www.openstreetmap.org/directions?from=&to=52.51294%2C13.32005" target="_blank" rel="noopener noreferrer"> Ernst-Reuter-Platz 7, <br> 10587 Berlin</a> 

<i class="fa-li fas fa-compass fa-2x" aria-hidden="true">
</i>
<div id="map"></div>
<script>
 var map = L.map('map').setView([52.51294, 13.32005], 16);
 L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
 }).addTo(map);
 var marker = L.marker([52.51294, 13.32005]).addTo(map);
</script>