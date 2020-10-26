<template>
  <!-- HTML CODE -->
  <div class="container-buttons">
      <div class="primary-button">
          <p>Primary</p>
      </div>
  </div>
</template>

<script>
// Export Component
export default {
  // Give name
  name: "PrimaryButton"
};
</script>

<style lang="scss" scoped>

// CSS CODE

.container-buttons{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px;
}

.primary-button{
    width: 182px;
    height: 48px;
    border-radius: 8px;
    background-color: var(--primary-70-color);
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px;
}

.primary-button:hover{
    background-color: var(--primary-90-color)
}

.primary-button:active{
    background-color: var(--primary-100-color)
}

p{
  font-family: Typold-medium;
  font-size: 16px;
  color: #FFFFFF;
  margin: 0;
  letter-spacing: 1px;
}

</style>
