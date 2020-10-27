<template>
  <!-- HTML CODE -->
  <div class="container--input">
    <div class="container--input-with-icon">
      <input
        type="text"
        class="default-text input input--text"
        placeholder="Placeholder"
      />
      <i class="input--icon"></i>
    </div>
    <p class="small-text js-message input--message "></p>
  </div>
</template>

<script>
// JS CODE
//const input = document.querySelector(".input");

// Export Component
export default {
  // Give name
  name: "InputText"
};
</script>

<style lang="scss" scoped>
.container--input {
  display: flex;
  flex-direction: column;
  max-width: var(--input--width);
}

.input {
  height: var(--input--height);
  width: var(--input--width);
  box-sizing: border-box;
  border-radius: var(--input--radius);
  border: 1px solid var(--gray-3-color);
  padding-left: var(--input--padding--left);
  color: var(--gray-3-color);
  background-color: transparent;
}

.input:focus {
  border: 1px solid var(--gray-4-color);
  outline: none;
  background-color: var(--white-1-color);
}

.container--input__success .input {
  border: 1px solid var(--validate-90-color);
}

.container--input__error .input {
  border: 1px solid var(--error-80-color);
  background-color: var(--error-50-color);
  color: var(--error-80-color);
}

.container--input-with-icon {
  position: relative;
}

.input--icon {
  position: absolute;
  top: calc(50% - 12px);
  right: var(--input--space--right);
  display: block;
  height: 24px;
  width: 24px;
  background-size: cover;
}

.container--input__error .input--icon {
  background-image: url("../assets/icons/alert-triangle.svg");
}

.container--input__success .input--icon {
  background-image: url("../assets/icons/validate.svg");
}

.input--message {
  max-width: var(--input--width);
  text-align: left;
  color: var(--black-color);
}

.container--input__error .input--message {
  color: var(--error-80-color);
}
</style>
