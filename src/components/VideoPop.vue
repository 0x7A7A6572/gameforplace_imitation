<template>
  <div class="video_dialog">
    <div>
      <iframe
        frameborder="0"
        src="https://v.qq.com/txp/iframe/player.html?vid=y3023hikn7h"
        width="1046"
        height="640"
        allowfullscreen="true"
      ></iframe>
    </div>
    <a class="close_btn"><img src="../assets/images/dia-close.png" alt=""></a>
  </div>
</template>
<style scoped>
.video_dialog {
     width: 1063px;
    height: 608px;
    padding: 9px 8px;
    box-sizing: border-box;
    background: url(../assets/images/dia-bg.png) no-repeat;
    position: fixed;
    left: 0;
    right: 0;
    bottom: 0;
    top: 0;
    margin: auto;
    z-index: 20;
    display: none;
}
.video_dialog div {
  height: 588px;
  overflow: hidden;
}
.close_btn {
    position: absolute;
    right: -102px;
    top: 7px;
    width: 75px;
    height: 75px;
    cursor: pointer;
}
</style>