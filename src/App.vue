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
a,a:link,a:visited,a:active,a:focus{
  color: #040404;
	text-decoration: none;
}

</style>
