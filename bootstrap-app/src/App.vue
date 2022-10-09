<template>
  <div id="app">
    <TopHeader />
    <HomeComponent />
  </div>
</template>

<script>
import HomeComponent from './components/HomeComponent.vue'
import TopHeader from './components/TopHeader.vue'

export default {
  name: 'App',
  components: {
    HomeComponent,
    TopHeader
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 20px;
  margin-left: 20px;
  margin-right: 20px;
}
</style>
