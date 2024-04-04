<template>
  <div>
    <section v-for="(sizes, category) in shoeSizesByCategory" :key="category">
      <h2>{{ category }}</h2>
      <ul>
        <li v-for="size in sizes" :key="size">{{ size }}</li>
      </ul>
    </section>
  </div>
</template>

<script>
export default {
  name: "Shoe",
  data() {
    return {
      shoeSizesByCategory: {
        Men: [39, 40, 41, 42, 43, 44, 45],
        Women: [36, 37, 38, 39, 40, 41],
        Children: [28, 29, 30, 31, 32, 33, 34],
      },
    };
  },
};
</script>

<style>
section {
  margin-bottom: 20px;
}
</style>
