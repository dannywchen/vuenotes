<template>
  <div>
    <h1>Characters</h1>
    <div class="list">
      <ListComp
        v-for="(obj, index) in list"
        :key="index"
        :name="obj.name"
        :age="obj.age"
        :gender="obj.gender"
      />
    </div>
  </div>
</template>

<script>
import ListComp from "../components/ListComp.vue"; // Adjust the import path as necessary
import { list } from "/list.js"; // Adjust the path to where your list.js is located

export default {
  name: "HomeView",
  components: {
    ListComp,
  },
  data() {
    return {
      list,
    };
  },
};
</script>

<style scoped>
.list {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: space-evenly;
  align-items: start; /* Align items at the start */
  width: 100%; /* Adjusted for responsiveness */
  padding: 1rem; /* Padding around the entire list for spacing */
}
</style>
