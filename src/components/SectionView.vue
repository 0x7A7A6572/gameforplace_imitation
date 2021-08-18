<template>
  <section>
    <!-- 插槽 -->
    <slot></slot>
  </section>
</template>
<script>
export default {
  name: "SectionView",
  props: {
    bg_path: {
      type: String,
    },
  },
  data: function () {
    return {
      bgPath: this.bg_path,
    };
  },
};
</script>

<style scoped>
section {
  /* width: 100vw; 不设置宽度 */
  height: 890px;
  position: relative;
  margin-top: -40px;
}
</style>