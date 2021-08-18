<template>
  <div class="sc_item">
    <div class="sc_item_vdio">
      <img src="../assets/images/img_03.jpg" alt="" />
      <img
        class="sc_item_vdio_play"
        src="../assets/images/play-btn.png"
        alt=""
      />
    </div>
    <img class="qrcode" src="../assets/images/downqrcode.jpg" alt="" />
    <div class="bt_download">
      <a class="bt_download_ios">
        <img src="../assets/images/ios.png" alt="" />
      </a>
      <a class="bt_download_adnroid">
        <img src="../assets/images/and.png" alt="" />
      </a>
    </div>
  </div>
</template>

<style scoped>
@keyframes zoomPlay {
    0%{
		transform: scale(.9);
	}
	100%{
		transform: scale(1);
	}
  /* from {
    zoom: 100%;
  }
  to {
    zoom: 120%;
  } */
}

.sc_item {
  width: 100%;
  display: flex;
  justify-content: center;
  position: absolute;
  top: 75%;
}
.sc_item_vdio {
  position: relative;
  padding: 5px 5px 5px 5px;
  display: flex;
  justify-content: center;
  align-items: center;
  background: url("../assets/images/video-bg.png");
}
.sc_item_vdio_play {
  content: "";
  width: 61px;
  height: 61px;
  position: absolute;
  /* 居中 */
  top: 50%;
  left: 50%;
  margin: -30px 0 0 -30px;
  animation: zoomPlay 2s infinite reverse;
}
/* .sc_item_vdio_play:hover {
    不是hover 而是持续动画
  animation: zoomPlay 0.5s infinite reverse; 
} */
.qrcode {
  margin: 0px 20px 0px 20px;
  width: 156px;
  height: 156px;
}

.bt_download {
  width: 229px;
  height: 156px;
  display: flex;
  flex-wrap: wrap;
  align-content: space-between;
}

.bt_download img {
}
</style>