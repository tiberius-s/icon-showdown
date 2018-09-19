<template>
  <div class="main">
      <Header />
      <IconRow v-for="(icon, index) in icons" :key='index' :icon='icon'/>
  </div>
</template>

<script>
import IconRow from "./IconRow";
import Header from "./Header";

export default {
  name: "Container",
  components: {
    IconRow,
    Header
  },
  props: {
    icons: {
      type: Array,
      default: () => {}
    }
  }
};
</script>

<style lang="scss" scoped>
.main {
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
}
</style>
