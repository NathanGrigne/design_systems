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
*{
  margin: 0;
  padding: 0;
}

#app {
  font-family: Garamond_regular;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #FFFFFF;
  background-image: url("assets/image/background.png");
  background-position: center;
  background-size: cover;
  height: 100%;
  width: 100%;
  position: absolute;
  top: 0;
  left: 0;
  overflow: hidden;
}
</style>
