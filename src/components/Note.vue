<template>
  <div class="note-container" :class="{'full-width': fullWidth}">
    <span>{{note}}</span>
  </div>
</template>

<script>
export default {
  name: "Note",
  props: {
    note: String,
    fullWidth: Boolean
  }
};
</script>

<style lang="scss" scoped>
.note-container {
  padding: 0.5rem 1rem;
  flex: 0 1 20%;
  text-transform: uppercase;
}
.full-width {
  flex: 0 1 80%;
  text-align: left;
  color: crimson;
}
</style>
