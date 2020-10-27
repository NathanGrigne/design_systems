<template>
  <div id="app">
    <div id="nav">
      <router-link to="/" class="default-text">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
import "./assets/styles/main.scss";

export default {};
</script>

<style lang="scss">
#app {
  font-family: Garamond_regular;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: var(--error-100-color);
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
