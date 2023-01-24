<template>
<h1>Bienvenido al mapa global</h1>
<div ref="mapContainer" class="map-container"></div>
   <div id='map' style='width: 600x; height: 400px;'></div>
</template>
<script setup>
import 'mapbox-gl/dist/mapbox-gl.css';
import {onMounted, ref} from 'vue';
import mapboxgl from 'mapbox-gl'; // or "const mapboxgl = require('mapbox-gl');"

mapboxgl.accessToken = 'pk.eyJ1IjoiamltZW5hbWFwOTkiLCJhIjoiY2xkOWg1MHF1MDcwcjNvczl3MWlmYWo0YSJ9.4JljQunKYrxQkJZF8XjAHA';

const mapContainer = ref<HTMLElement>(null)
onMounted(()=>{

    const map = new mapboxgl.Map({
        container: 'map', // container ID
        style: 'mapbox://styles/mapbox/streets-v12', // style URL
        center: [-74.5, 40], // starting position [lng, lat]
        zoom: 1, // starting zoom
    });
    
})


</script>
<style scoped>
.map-container{
    width: 100vw;
}
body { margin: 0; padding: 0; }
</style>
