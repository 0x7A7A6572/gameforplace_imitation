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
