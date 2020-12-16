<template>
  <div class="home">
    <div class="title-box">
    <img class="logo" src="@/assets/Logo.svg" alt="Happy">
    <h1>Leve a felicidade para o mundo</h1>
    </div>
    <img class="landing" src="@/assets/landing.svg" alt="Leve a felicidade para o mundo">
    <router-link to="/Orphanages"><img src="@/assets/arrow.svg" alt="Veja os orfanatos mais proximos"></router-link>
  </div>
</template>

<script>

export default {
  name: 'Home',
}
</script>

<style scoped>

.home {
  min-height: 100vh;
  width: 100vw;
  background-color: rgb(157, 184, 235);
  display:flex;
  align-items: center;
  justify-content: space-between;
  padding: 40px;
}

.home .title-box {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  width: 40%;
  height: 50vh;
}

.home .title-box .logo {
  width: 300px;
}

.home .title-box h1 {
  color: white;
  font-size:2.5rem;
}

.home .title-box p {
  color: white;
  font-size: 1.2rem;
  text-align: center;
}

.home .landing {
  width: 40%;
  height: 80vh;
}

.home a {
  width:50px;
  height:50px;
  background-color:yellow;
  border-radius: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  position:absolute;
  bottom: 5%;
  right: 5%;
  }

  .home a:hover {
    background-color: rgb(235, 235, 19);
  }

  .home a img {
    width:30px;
    height:30px;
  }

  @media screen and (max-width:600px) {

    .home {
      flex-direction: column;
      align-items: center;
    }

    .home .title-box {
      width: 90%;
      height: 100px;
      align-items: center;
    }

    .title-box h1 {
      display: none;
    }

    .home .landing {
      width: 90%;
    }
  }

</style>
