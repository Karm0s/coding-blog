<template>

  <div class="hero flex flex-col justify-start">
    <AppHeader/>
    <slot class="flex-grow"/>
  </div>

</template>

<script>
import AppHeader from './AppHeader';

export default {
  name: 'AppHero',
  components: {
    AppHeader,
  }
}
</script>

<style scoped>
.hero {
  background-image: linear-gradient(
      rgba(18, 16, 13, 0.9),
      rgba(18, 16, 13, 0.5)
    ),
    url(https://upload.wikimedia.org/wikipedia/commons/0/0a/The_Great_Wave_off_Kanagawa.jpg);
  background-size: cover;
  background-attachment: fixed;
  height: 90vh;
}
.hero-content{
  height: 100%;
}
.logo-font{
  font-family: 'GoatskinBrush';
  font-size: 35px;
  font-weight: normal;
}

</style>