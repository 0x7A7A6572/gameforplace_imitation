<template>
  <div id="vue_body">
    <out-header></out-header>
    <nav-gp id="nva"></nav-gp>
    <section-view id="sction1">
      <sc-item></sc-item>
    </section-view>
    <video-pop></video-pop>
    <section-view id="sction2"> 
      <sc-title title="版本咨询"> </sc-title>
      <tab-section-2>
      </tab-section-2>
       </section-view>
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
import OutHeader from "./components/OutHeader.vue";
import NavGp from "./components/NavGp.vue";
import SectionView from "./components/SectionView.vue";
import ScItem from "./components/ScItem.vue";
import VideoPop from "./components/VideoPop.vue";
import ScTitle from "./components/ScTitle.vue";
import TabSection2 from './components/tab-section2.vue';

export default {
  name: "App",
  components: {
    OutHeader,
    NavGp,
    SectionView,
    ScItem,
    VideoPop,
    ScTitle,
    TabSection2
  },
};
</script>
,
    TabSction1
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
ul{ list-style: none;}

#vue_body {
  position: relative;
}
#nva {
  z-index: 10;
}

#sction1 {
  background: url(assets/images/section1_bg1.jpg) center top no-repeat;
  z-index: 9;
  /* width: 100vw; 不设置宽度 */
  height: 890px;
  position: relative;
  margin-top: -40px;
}
video-pop {
  z-index: 20;
}
#sction2 {
  background: url(assets/images/section2_bg1.jpg) center top;
  z-index: 8;
  height: 890px;
  position: relative;
  padding-top: 40px;
}
/* tab-section-2{
      width: 1200px;
} */
</style>
