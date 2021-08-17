<template>
  <nav class="gpnav">
    <div>
      <a><img src="../assets/images/logo2.png" alt="" class="applogo" /></a>
        <!-- h1包住两个text 下文block换行 -->
        <h1>和平精英
          <span>全球玩家的竞技冒险世界</span>
        </h1>
    </div>

    <ul class="nav-list">
      <li v-for="(item, i) in navList" :key="i">
       <a href="">{{ item }}</a> 
      </li>
    </ul>
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
  padding: 5px;
  width: 100vw;
  background: url("../assets/images/nav_bg.png") center no-repeat;
  position: relative;
  display: flex;
}
.gpnav div{
  /* position: relative; */
   display: flex;
   
   /* margin: 0 auto; */
}
.gpnav .applogo {
  /* left: 200px; */
  /* margin-left: 200px; */
}
.gpnav h1 {
  margin-left: 20px;
  color: orange;
  white-space: normal;
  flex-shrink: 0;
}
.gpnav span{
  font-size: 14px;
  color: white;
  font-weight: normal;
  display: block; /*换行 */
}
.nav-list {
  /* position: relative; */
  display: flex;
  justify-content: center;
  
  list-style: none;
  /* margin: 0 auto; */
}
.nav-list li{
text-align: center;
width: 120px;
}
</style>

