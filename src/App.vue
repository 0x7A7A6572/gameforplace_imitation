<template>
  <div id="vue_body">
    <out-header></out-header>
    <nav-gp id="nva"></nav-gp>
    <section-view id="sction1">
      <sc-item></sc-item>
    </section-view>
    <video-pop></video-pop>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import OutHeader from "./components/OutHeader.vue";
import NavGp from "./components/NavGp.vue";
import SectionView from "./components/SectionView.vue";
import ScItem from "./components/ScItem.vue";
import VideoPop from "./components/VideoPop.vue";

export default {
  name: "App",
  components: {
    OutHeader,
    NavGp,
    SectionView,
    ScItem,
    VideoPop,
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
#vue_body {
  position: relative;
}
#nva {
  z-index: 10;
}

#sction1 {
  background: url(assets/images/section1_bg1.jpg) center top no-repeat;
  z-index: 9;
}
video-pop{
  z-index: 20;
}
</style>
