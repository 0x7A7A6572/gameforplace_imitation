<template>
  <nav class="gpnav">
    <div>
      <a><img src="../assets/images/logo2.png" alt="" class="applogo" /></a>
      <!-- h1包住两个text 下文block换行 -->
      <h1>
        和平精英
        <span>全球玩家的竞技冒险世界</span>
      </h1>
    </div>

    <ul class="nav-list">
      <li v-for="(item, i) in navList" :key="i">
        <a href="">{{ item }}</a>
      </li>
    </ul>
    <!-- 进入官网 -->
    <button class="to-official"></button>
  </nav>
</template>
<script>
export default {
  name: "NavGp",
  data: function () {
    return {
      navList: [
        "版本资讯",
        "新增玩法",
        "新增场景",
        "新增道具",
        "新增内容",
        "系统优化",
        "游戏特色",
      ],
    };
  },
};
</script>
<style scoped>
.gpnav {
  /* padding: 5px; */
  /* width: 100vw;不设置宽度  */
  background: url("../assets/images/nav_bg.png") center no-repeat;
  position: relative;
  display: flex;
  justify-content: space-between;
}
.gpnav div {
  position: relative;
  display: flex;

  margin: 0 auto;
}
.gpnav .applogo {
  margin: 5px;
  /* left: 200px; */
  /* margin-left: 200px; */
}
.gpnav h1 {
  margin-left: 20px;
  color: orange;
  white-space: normal;
  flex-shrink: 0;
}
.gpnav span {
  font-size: 14px;
  color: white;
  font-weight: normal;
  display: block; /*换行 */
}
.nav-list {
  /* position: relative; */

  display: flex;
  /* justify-content: center; */
  align-items: center;
  list-style: none;
  margin: 0 auto;
}
.nav-list li {
  width: 120px;
  height: 100px;
  text-align: center;
  /* align-items: center; */
}
.nav-list li:hover {
  background: url("../assets/images/navHover_bg.png") 0 -70px;
}
.nav-list li a {
  line-height: 80px; /**ul中a居中靠ta */
  color: white;
  text-align: center;
}
.to-official {
  width: 232px;
  height: 78px;
  position: absolute;
  top:100%;
  right: 10%;
  background: url("../assets/images/join_btn.png");
}
</style>

