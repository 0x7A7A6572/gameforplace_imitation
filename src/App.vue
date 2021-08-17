<template>
  <div>
    <out-header></out-header>
    <nav-gp></nav-gp>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import OutHeader from "./components/OutHeader.vue";
import NavGp from "./components/NavGp.vue";

export default {
  name: "App",
  components: {
    OutHeader,
    NavGp,
  },
};
</script>

<style>
/* 样式重置 */
body {
  margin: 0;
}
button {
  background: none;
  border: none;
}
a,
a:link,
a:visited,
a:active,
a:focus {
  color: #040404;
  text-decoration: none;
}
</style>
