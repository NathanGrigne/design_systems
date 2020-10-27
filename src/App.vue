<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
import "./assets/styles/colors.scss";
import "./assets/styles/fonts.scss";
import "./assets/styles/main.scss";

export default {};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Garamond_regular;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  height: 100%;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
}
</style>
