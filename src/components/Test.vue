<template>
  <!-- HTML CODE -->
  <div class="container">
    <h2 class="title">My Input</h2>
    <input type="text" class="input" placeholder="Text">
  </div>
</template>

<script>
// JS CODE
const input = document.querySelector('.input')

// Export Component
export default {
  // Give name
  name: "Test"
};
</script>

<style lang="scss" scoped>

// CSS CODE

h1 {
  font-family: Garamond_regular;
  color: --error-100-color;
}

</style>
