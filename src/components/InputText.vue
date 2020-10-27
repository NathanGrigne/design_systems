<template>
  <!-- HTML CODE -->
  <div class="container--form--input">
    <p class="label-text input--label">{{ label }}</p>
    <div
      v-if="type == 'error'"
      class="container--input container--input__error"
    >
      <div class="container--input-with-icon">
        <input
          v-bind:placeholder="label"
          type="text"
          class="default-text input input--text"
        />
        <i class="input--icon"></i>
      </div>
      <p class="small-text js-message input--message">{{ message }}</p>
    </div>
    <div
      v-else-if="type == 'success'"
      class="container--input container--input__success"
    >
      <div class="container--input-with-icon">
        <input
          v-bind:placeholder="label"
          type="text"
          class="default-text input input--text"
        />
        <i class="input--icon"></i>
      </div>
      <p class="small-text js-message input--message "></p>
    </div>
    <div v-else class="container--input">
      <div class="container--input-with-icon">
        <input
          v-bind:placeholder="label"
          type="text"
          class="default-text input input--text"
        />
        <i class="input--icon"></i>
      </div>
      <p class="small-text js-message input--message "></p>
    </div>
  </div>
</template>

<script>
// JS CODE
//const input = document.querySelector(".input");

// Export Component
export default {
  // Give name
  name: "InputText",
  props: ["label", "type", "message"]
};
</script>

<style lang="scss" scoped>
.container--form--input {
  display: flex;
  flex-direction: column;
  align-items: baseline;
}

.container--input {
  display: flex;
  flex-direction: column;
  width: var(--input--width);
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
  margin-top: 8px;
}

.container--input__error .input--message {
  color: var(--error-80-color);
}
.input--label {
  margin-bottom: 10px;
  margin-top: 23px;
  color: var(--gray-3-color);
}
</style>
