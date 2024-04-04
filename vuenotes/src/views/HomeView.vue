<template>
  <div>
    <h1>Welcome to Our Shoe Store</h1>
    <Shoe />
  </div>
</template>

<script>
import Shoe from "@/components/shoe.vue";

export default {
  name: "Home",
  components: {
    Shoe,
  },
};
</script>

<style></style>
