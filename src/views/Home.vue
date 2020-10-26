<template>
  <div class="home">
    <!-- Call component -->
    <PrimaryButton />
    <SecondaryButton />
    <Checkbox />
  </div>
</template>

<script>

// Import Component PS : Caps is necessary on the first letter of tour component
import PrimaryButton from "@/components/PrimaryButton.vue";
import SecondaryButton from "@/components/SecondaryButton.vue";
import Checkbox from "@/components/Checkbox.vue"

export default {
  // Export Vue
  name: "Home",
  components: {
    PrimaryButton,
    SecondaryButton,
    Checkbox
  }
};
</script>
