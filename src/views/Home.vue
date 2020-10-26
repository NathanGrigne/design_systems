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
import Buttons from "@/components/Buttons.vue";
import Checkbox from "@/components/Checkbox.vue"

export default {
  // Export Vue
  name: "Home",
  components: {
    Buttons,
    Checkbox
  }
};
</script>
