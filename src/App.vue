<template>
  <div id="app" class="antialiased">
    <router-view></router-view>
  </div>
</template>

<script>
export default {
  name: 'App',
  components: {
  }
}
</script>

<style>
#app {
  font-family: 'Merriweather', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
@font-face {
  font-family: "GoatskinBrush";
  src: local("GoatskinBrush"),
    url("./fonts/GoatskinBrushPersonalUse-RG5E.ttf") format("truetype");
}
@font-face{
  font-family: 'Merriweather';
  src: url('./fonts/Merriweather-Regular.ttf') format('truetype');
  font-weight: normal;
  font-style: normal;
}
@font-face{
  font-family: 'Merriweather';
  src: url('./fonts/Merriweather-Black.ttf') format('truetype');
  font-weight: bold;
  font-style: normal;
}
</style>
