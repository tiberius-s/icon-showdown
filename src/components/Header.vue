<template>
  <div class="header">
    <Note note="glyphicon used" :full-width="false" />
    <Note note="1st choice" :full-width="false" />
    <Note note="2nd choice (or alt use)" :full-width="false" />
    <Note note="3rd choice (or alt use)" :full-width="false" />
    <Note note="4th choice (or alt use)" :full-width="false" />
  </div>
</template>

<script>
import Note from "./Note";
export default {
  name: "Header",
  components: { Note }
};
</script>

<style lang="scss" scoped>
.header {
  flex: 1 1 100%;
  display: flex;
  border-bottom: 2px solid #2c3e50;
  text-align: center;
  font-size: 2rem;
  font-weight: bold;
}
</style>
