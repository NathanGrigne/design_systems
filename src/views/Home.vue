<template>
  <div class="home">
    <!-- Call component -->
    <Test />
    <Buttons />
    <Checkbox />
  </div>
</template>

<script>

// Import Component PS : Caps is necessary on the first letter of tour component
import Test from "@/components/Test.vue";
import Buttons from "@/components/Buttons.vue";
import Checkbox from "@/components/Checkbox.vue"

export default {
  // Export Vue
  name: "Home",
  components: {
    Test,
    Buttons,
    Checkbox
  }
};
</script>
