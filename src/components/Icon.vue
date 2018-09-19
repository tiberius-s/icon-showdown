<template>
  <div class="icon-container" :class="{'glyphicon-cell' : isBS()}">
    <span><span v-if="isFA()">{{iconType}} </span>{{name}} </span><i :class='[iconType, name]'></i>
  </div>
</template>

<script>
export default {
  name: "Icon",
  props: {
    iconType: String,
    name: String
  },
  methods: {
    isFA: function() {
      return /fa/.test(this.iconType);
    },
    isBS: function() {
      return /glyphicon/.test(this.iconType);
    }
  }
};
</script>

<style lang="scss" scoped>
.icon-container {
  flex: 0 1 20%;
  border-right: 1px solid #2c3e50;
  text-align: left;
  display: flex;
  justify-content: space-between;
  padding: 0.5rem 1rem;
}
.glyphicon-cell {
  background-color: #f8f8f8;
}
</style>
