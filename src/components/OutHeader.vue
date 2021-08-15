<template>
  <header id="continer">
    <div id="left">
      <a href="#" class="logo"><img src="../assets/images/logo.png" alt="" /></a>
      <span>
        <img src="../assets/images/img_01.jpg" alt="" />
        <a href="#"><img src="../assets/images/img_02.jpg" alt="" /></a>
      </span>
    </div>
    <div id="right">
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
#continer {
    width: 100%;
    height: 50px;
    display: flex;
    background: #f4f4f4;
}
</style>