<template>
  <div class="home">
    <!-- Call component -->
    <div class="container">
      <h1>Planty</h1>
      <p class="third-title">How much are you a plant lover?</p>
      <div class="container--connexion">
        <div class="container--connexion__social">
          <SocialButton type="google" />
          <SocialButton type="facebook" />
        </div>
        <InputText label="Name"></InputText>
        <InputText label="Email" type="success"></InputText>
        <InputText
          label="Password"
          type="error"
          message="Error: Error message"
        ></InputText>
        <div class="confirm-form">
          <div class="accept-term">
            <Checkbox />
            <p class="label-text">
              Creating an account means you're ready with our
              <span class="term action-text">Terms of Service</span> and our
              <span class="term action-text">Privacy Policy</span>
            </p>
          </div>
          <PrimaryButton text="Create my account" />
          <p class="log-in label-text">
            Already an account? <span class="term action-text">Sign in</span>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// Import Component PS : Caps is necessary on the first letter of tour component
import PrimaryButton from "@/components/PrimaryButton.vue";
import Checkbox from "@/components/Checkbox.vue";
import InputText from "@/components/InputText.vue";
import SocialButton from "@/components/BtnSocialConnexion.vue";

export default {
  // Export Vue
  name: "Home",
  components: {
    PrimaryButton,
    Checkbox,
    InputText,
    SocialButton
  }
};
</script>

<style lang="scss" scoped>
.home {
  display: flex;
  align-items: center;
  width: 100vw;
  height: 100vh;
}
.container {
  width: 614px;
  min-height: 818px;
  background-color: #060904a6;
  margin-left: 15vw;
  border-radius: 18px;
}
.container .third-title {
  text-align: left;
}
h1 {
  font-family: Garamond-Regular;
  font-size: 48px;
  color: var(--secondary-100-color);
}

p.third-title {
  color: var(--gray-1-color);
  font-family: Garamond-Regular;
}

.accept-term {
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: left;
}

.accept-term p {
  width: 372px;
}

.term {
  color: var(--secondary-100-color);
  cursor: pointer;
}

.container {
  padding: 5%;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
  align-items: baseline;
  backdrop-filter: blur(3px);
}
.container--connexion {
  width: 100%;
}
.container--connexion__social {
  display: flex;
  justify-content: space-around;
  margin-top: 10%;
}
</style>
