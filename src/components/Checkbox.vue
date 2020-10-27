<template>
  <!-- HTML CODE -->
  <div class="container-checkbox">
      <input type="checkbox" name="checkbox" class="checkbox">
  </div>
</template>

<script>
// Export Component
export default {
  // Give name
  name: "Checkbox"
};
</script>

<style lang="scss" scoped>

// CSS CODE

.container-checkbox{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 10px;
}

.checkbox{
    appearance: none;
    width: 28px;
    height: 28px;
    border: 1px solid #DDE2E5;
    border-radius: 8px;
}

.checkbox:focus{
    outline: none;
}

.checkbox:hover{
    cursor: pointer;
}

.checkbox:checked{
    appearance: none;
    background-color: var(--validate-10-color);
    border: none;
    display: flex;
    justify-content: center;
    align-items: center;
}

.checkbox:checked::before{
    content: "✔";
    color: var(--validate-90-color);
    font-size: 20px;
}

</style>
