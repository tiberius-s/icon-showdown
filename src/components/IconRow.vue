<template>
  <div class="icon-row">
    <Icon icon-type="glyphicon" :name=icon.bootstrap />
    <Note v-if="icon.note !== ''" :note=icon.note :full-width="true" />
    <Icon v-else v-for="(item, index) in icon.fontawesome" :key="index" :icon-type="item.type" :name=item.name />
  </div>
</template>

<script>
import Icon from "./Icon";
import Note from "./Note";
export default {
  name: "IconRow",
  components: { Icon, Note },
  props: {
    icon: Object
  }
};
</script>

<style lang="scss" scoped>
.icon-row {
  flex: 1 1 100%;
  display: flex;
  border-bottom: 1px solid #2c3e50;
}
</style>
