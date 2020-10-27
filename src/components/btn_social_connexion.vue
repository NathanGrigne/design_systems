<template>
  <!-- HTML CODE -->
  <div class="container-buttons">
    <div class="btn-bis">
      <i v-if="type == 'google'"></i>
      <i v-if="type == 'facebook'"></i>
      <p v-if="type == 'google'" class="btn--text btn--icon btn--icon__google">
        Sign-in with Google
      </p>
      <p
        v-if="type == 'facebook'"
        class="btn--text btn--icon btn--icon__facebook"
      >
        Sign-in with Facebook
      </p>
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
