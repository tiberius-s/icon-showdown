<template>
  <div id="app">
    <Container :icons="icons" />
  </div>
</template>

<script>
import Container from "./components/Container";
import icons from "./assets/icons.json";

export default {
  name: "app",
  components: {
    Container
  },
  data() {
    return {
      icons: icons
    };
  }
};
</script>

<style lang="scss">
body {
  width: 100%;
  text-align: center;
}
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  font-size: 18px;
  color: #2c3e50;
  margin: 0 auto;
  width: 85%;
  margin-top: 4rem;
  margin-bottom: 3rem;
}
</style>
