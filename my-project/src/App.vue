<template>
  <main>
<!--    <Dummy msg="Dummy"/>-->
    <MultiBand />
<!--    <MultiBandTypescript />-->
<!--    <MultiBandDefineComponent />-->
  </main>
</template>

<script>

// import Dummy from './components/Dummy.vue'
import MultiBand from './components/MultiBand.vue'
// import MultiBandTypescript from './components/MultiBandTypescript.vue'
// import MultiBandDefineComponent from './components/MultiBandDefineComponent.ts'

export default {
  name: 'App',
  components: {
    // Dummy,
    MultiBand,
    // MultiBandTypescript,
    // MultiBandDefineComponent
  }
}
</script>

<style>
body{
  margin: 0;
  color: white;
  background-color: #000000;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
