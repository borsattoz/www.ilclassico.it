---
layout: default
title: "Contatti"
permalink: ':path/'
custom_css:
- 'https://unpkg.com/leaflet@1.9.4/dist/leaflet.css'
custom_js:
- 'https://unpkg.com/leaflet@1.9.4/dist/leaflet.js'
---

# Contatti e orari
Associazione *Il*Classico Musica e Arte APS

via Giuseppe Meda 45, Milano, 20141

**Tel**: [02 8438027](tel:+39028438027)

**Mail**: [{{ site.email }}](mailto:{{ site.email }})

## Orari scuola
I corsi individuali di strumento si svolgono dal **lunedì** al **sabato** dalle **9:00** alle **21:00**. I corsi collettivi si svolgono al **pomeriggio** in giorni prestabiliti.

## Orari segreteria
**lunedì** - **giovedì** dalle **15:00** alle **19:00**

## Come raggiungerci
**Metro**: M2 Romolo / Famagosta

**Autobus**: Linee 90/91, 95

**Tram**: Linee 3, 15

<style scoped>
#map { height: 350px; }
</style>
<div id="map"></div>

<script>
const geocoord = [45.440109505103635, 9.178731722793597];
let map = L.map('map').setView(geocoord, 13);

L.tileLayer('https://tile.openstreetmap.org/{z}/{x}/{y}.png', {
    maxZoom: 19,
    attribution: '&copy; <a href="http://www.openstreetmap.org/copyright">OpenStreetMap</a>'
}).addTo(map);

let marker = L.marker(geocoord).addTo(map);
</script>
