<template>
  <div>
    <h2>{{ name }}</h2>
    <p>{{ age }}</p>
    <h3>{{ gender }}</h3>
  </div>
</template>

<script>
export default {
  name: "ListComp",
  props: {
    name: String,
    age: Number,
    gender: String,
  },
};
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  height: 10rem;
  justify-content: space-evenly;
  align-items: center;

  padding: 2rem;
  margin: 2rem;
  border-color: white;
  border-width: 2px;
}
</style>
