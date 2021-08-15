<template>
<div>
  <out-header></out-header>
</div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import OutHeader from './components/OutHeader.vue'
export default {
  name: 'App',
  components: {
    // HelloWorld
    OutHeader
}
}
</script>

<style>
/* 样式重置 */
body{margin: 0;}
button{
  background: none;
  border: none;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
