<template>
  <div class="home">
    <!-- Call component -->
    <InputText />
    <SocialButton type="google" />
  </div>
</template>

<script>
// Import Component PS : Caps is necessary on the first letter of tour component
import InputText from "@/components/inputText.vue";
import SocialButton from "@/components/btnSocialConnexion.vue";

export default {
  // Export Vue
  name: "Home",
  components: {
    InputText,
    SocialButton
  }
};
</script>
