<template>
  <div class="home">
    <!-- Call component -->
    <Test />
  </div>
</template>

<script>

// Import Component PS : Caps is necessary on the first letter of tour component
import Test from "@/components/Test.vue";

export default {
  // Export Vue
  name: "Home",
  components: {
    Test
  }
};
</script>
