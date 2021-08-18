<template>
  <div class="select">
    <ul class="select_ul">
      <li v-for="(item, i) in select_title" :key="i">{{ item }}</li>
    </ul>
<div class="select_content">
    <ul class="select_content_active">
        <li v-for="(item,i) in select_title_active" :key="i">{{item}}</li>
    </ul>
</div>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      select_title: ["最新活动", "商城新品"],
      select_title_active: ["抢占据点", "烤鸡大师"],
      select_title_shop: [
        "未来战士-套装",
        "M24未来战士",
        "S686未来战士",
        "Scar-L未来战士",
      ],
    };
  },
};
</script>
<style scoped>
.select {
  width: 1200px;
  margin: 60px auto 0;
}

.select_ul {
  display: flex;
}
.select_ul li {
  width: 600px;
  height: 100px;
  line-height: 100px;
  font-size: 38px;
  color: #ffbf05;
  text-align: center;
  cursor: pointer;
  background: url(../assets/images/css-sprites.png) no-repeat -20px -17px;
}
.select_content{
    height: 440px;
    background: url(../assets/images/sec2-cont-bg.png) no-repeat;
}
</style>
