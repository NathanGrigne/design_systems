<template>
  <div class="home">
    <!-- Call component -->
    <div class="container">
      <h1>Planty</h1>
      <p class="third-title">How much are you a plant lover?</p>
      <InputText />
      <SocialButton type="google" />
      <div class="confirm-form">
        <div class="accept-term">
          <Checkbox />
          <p>Creating an account means you're ready with our <span class="term">Terms of Service</span> and our <span class="term">Privacy Policy</span></p>
        </div>
        <PrimaryButton />
        <p class="log-in">Already an account? <span class="term">Sign in</span></p>
      </div>
    </div>
  </div>
</template>

<script>
// Import Component PS : Caps is necessary on the first letter of tour component
import PrimaryButton from "@/components/PrimaryButton.vue";
import SecondaryButton from "@/components/SecondaryButton.vue";
import Checkbox from "@/components/Checkbox.vue";
import InputText from "@/components/InputText.vue";
import SocialButton from "@/components/BtnSocialConnexion.vue";

export default {
  // Export Vue
  name: "Home",
  components: {
    PrimaryButton,
    SecondaryButton,
    Checkbox,
    InputText,
    SocialButton
  }
};
</script>

<style lang="scss" scoped>
  .container{
    width: 614px;
    height: 818px;
    background-color: #060904A6;
    margin-left: 15vw;
    margin-top: 6vh;
    border-radius: 18px;
  }

  h1{
    font-family: Garamond-Regular;
    font-size: 48px;
    color: var(--secondary-100-color);
  }

  p.third-title{
    color: var(--gray-1-color);
    font-family: Garamond-Regular;
  }

  .accept-term{
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: left;
    font-family: Typold-Regular;
    font-size: 12px;
    line-height: 16.36px;
  }

  .accept-term p{
    width: 372px;
  }

  .term{
    color: var(--secondary-100-color);
  }

  .log-in{
    font-family: Typold-Regular;
    font-size: 12px;
    line-height: 16.36px;;
  }
</style>