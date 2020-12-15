<template>
  <div class="wrapper">
    <section class="side-bar">
      <router-link to="/">
      <img class="logo" src="@/assets/Logo.svg" alt="Happy">
      </router-link>
      <p>Ajude a transformar o mundo em um lugar melhor.</p>
    </section>
    <iframe class="map" src="https://www.google.com/maps/embed?pb=!1m16!1m12!1m3!1d887820.4050671754!2d-51.58234180067377!3d-29.631335827372475!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!2m1!1sorfanatos!5e0!3m2!1spt-BR!2sbr!4v1608058474340!5m2!1spt-BR!2sbr" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
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
  flex-direction: column;
  justify-content: space-between;
  padding: 50px 0;
}

.side-bar a {
  display: flex;
  justify-content: center;
}

.side-bar p {
  color: white;
  text-align: center;
  font-size: 1.3rem;
}

.map {
  width: 70%;
  height: 100vh;
}

</style>