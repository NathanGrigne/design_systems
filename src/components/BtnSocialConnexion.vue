<template>
  <!-- HTML CODE -->
  <div class="container-buttons">
    <div class="small-text btn-bis">
      <i v-if="type == 'google'"></i>
      <i v-if="type == 'facebook'"></i>
      <a v-if="type == 'google'" class="btn--text btn--icon btn--icon__google">
        Sign-in with Google
      </a>
      <a
        v-if="type == 'facebook'"
        class="btn--text btn--icon btn--icon__facebook"
      >
        Sign-in with Facebook
      </a>
    </div>
  </div>
</template>

<script>
// JS CODE
//const input = document.querySelector(".input");

// Export Component
export default {
  // Give name
  name: "SocialButton",
  props: ["type"]
};
</script>

<style lang="scss" scoped>
.btn-bis {
  position: relative;
  display: inline-block;
  border-radius: var(--input--radius);
  padding: var(--btn--space);
  color: var(--secondary-100-color);
  box-sizing: border-box;
  border: 1px solid var(--white-1-color);
  cursor: pointer;
  background-color: var(--white-1-color);
}

.btn-bis:hover {
  border: 1px solid var(--secondary-100-color);
}

.btn--text {
  display: flex;
  justify-content: center;
  align-items: center;
}

.btn--icon::before {
  content: " ";
  margin-right: var(--btn--space);
  height: 24px;
  width: 24px;
  background-size: contain;
  background-repeat: no-repeat;
  background-position: center;
}

.btn--icon__google::before {
  background-image: url("../assets/icons/google.svg");
}

.btn--icon__facebook::before {
  background-image: url("../assets/icons/facebook.svg");
}
</style>
