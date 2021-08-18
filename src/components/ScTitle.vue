<template>
  <h2>{{ mTitle }}</h2>
</template>
<script>

export default {
  props: { title: { type: String, defualt: "" } },
  data: function () {
    return {
      mTitle: this.title,
    };
  },
};
</script>

<style scoped>
h2 {
  height: 76px;
  background: url(../assets/images/section2_head.png) no-repeat center;
  text-indent: -9999px;
  overflow: hidden;
}
</style>