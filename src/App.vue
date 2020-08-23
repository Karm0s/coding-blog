<template>
  <div id="app" class="antialiased">
    <AppHeader/>
    <router-view></router-view>
  </div>
</template>

<script>
import AppHeader from './components/layout/AppHeader';

export default {
  name: 'App',
  components: {
    AppHeader
  }
}
</script>

<style>
#app {
  font-family: Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
