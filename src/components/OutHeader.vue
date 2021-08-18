<template>
  <header id="header">
    <div class="left">
      <!-- 腾讯游戏logo -->
      <a href="#" class="logo"
        ><img src="../assets/images/logo.png" alt=""
      /></a>
      <!-- 鼠标悬浮弹出响应图片 -->
      <span>
        <img src="../assets/images/img_01.jpg" alt="" />
        <!-- 弹出的图片 -->
        <a href="#"><img src="../assets/images/img_02.jpg" alt="" /></a>
      </span>
    </div>
    <div class="right">
      <h3 class="text1"><a href="#">成长守护平台</a></h3>
      <h3 class="text2">
        <span>腾讯游戏排行榜</span>
        <iframe
          src="https://game.gtimg.cn/images/js/title/title_game_rank.html?rd=0.5387871893477456"
          frameborder="0"
        ></iframe>
      </h3>
    </div>
  </header>
</template>

<script>
export default {
  name: "OutHeader",
};
</script>

<style scoped>
#header {
  width: 80%;
  height: 50px;
  /* max-height: 50px; */
  display: flex;
  background: #ffffff;
  position: relative;
  justify-content: space-between;
  /* justify-items: auto; */
  margin: 0 auto;
}
/* left */
.logo {
  position: relative;
  z-index: 999;
}
#header .left {
  position: relative;
}
#header .left span a {
  top: 0;
  left: 0;
  position: absolute;
  display: none;
}

#header .left span:hover a {
  display: block;
}
/* right */
.right {
  display: flex;

  /* padding-right: 10%; */
}
.text1,
.text2 {
  color: #040404;
  font-size: 14px;
  font-weight: normal;
  text-align: center;
  padding-left: 30px;
  /* padding-right: 30px; */
  position: relative;
  display: flex;
  /* justify-content: center; */
  /* text-align: center; */
}
/* .right .text1 a {
  display: flex;
} */
.right .text1::before {
  content: "";
  width: 30px;
  height: 30px;
  background: url("../assets/images/ico_01.png") -30px 0;
  /* background-position: -30px 0; */
  position: absolute;
  left: 0;
  top: -5px;
}
.text2 span {
  padding-right: 30px; /* 给伪元素空间 */
  position: relative;
}
.text2::after {
  content: "";
  width: 30px;
  height: 30px;
  background: url("../assets/images/ico_01.png");
  transform: rotate(90deg);
  position: absolute; /* 方便定位 */
  right: 0;
  top: -5px;
}
.text2 iframe {
  width: 708px;
  height: 582px;
  position: absolute;
  top: 30px;
  right: 0;
  display: none;
}
.text2:hover iframe {
  display: block;
}
.text2:hover iframe,#header .left span a{
  z-index: 13;
}

</style>