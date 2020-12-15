<template>
  <div class="wrapper">
    <section class="side-bar">
      <img class="logo" src="@/assets/Logo.svg" alt="Happy">
    </section>
    <GmapMap
  :center="{lat:-29.9234021, lng:-51.4119127}"
  :zoom="8"
  map-type-id="terrain"
  style="width: 70%; height: 100vh"
>
  <GmapMarker
    :key="index"
    v-for="(m, index) in markers"
    :position="m.position"
    :clickable="true"
    :draggable="true"
    @click="center=m.position"
  />
</GmapMap>
  </div>
</template>

<script>
export default {
  name: 'Orphanages'
}
</script>

<style scoped>

.wrapper {
  width:100vw;
  min-height: 100vh;
  display:flex;
}

.side-bar {
  width: 30%;
  height: 100vh;
  background-color: rgb(157, 184, 235);
  display: flex;
  justify-content: center;
  align-items: flex-start;
}

</style>