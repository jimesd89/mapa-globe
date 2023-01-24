<script>
import MapaGlobe from "./components/MapaGlobe.vue"

export default {
  components:{
    MapaGlobe
  }
}
</script>

<template>
<MapaGlobe/>
</template>

<style scoped>
html, body {
  padding: 0;
  margin: 0;
}
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
}
.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}
.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}
</style>
