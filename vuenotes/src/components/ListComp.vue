<template>
  <div class="card">
    <h2>{{ name }}</h2>
    <p>Age: {{ age }}</p>
    <h3>Gender: {{ gender }}</h3>
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
.card {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  align-items: center;
  height: 10rem;
  padding: 2rem;
  margin: 2rem;
  border: 2px solid #cc7e7e; /* Light grey border */
  border-radius: 8px; /* Rounded corners for a card-like appearance */
  background-color: #811515; /* White background for better readability */
}
h2,
h3,
p {
  width: 100%;
  text-align: center;
  border-bottom: 1px solid #050303; /* Light borders under text for separation */
}
h3,
p {
  padding-bottom: 0.5rem; /* Padding for visual space */
}
</style>
