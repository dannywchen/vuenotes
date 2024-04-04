<template>
  <div>
    <h1>peepeepoopoo</h1>
    <div class="list">
      <ListComp
        class="comp"
        v-for="obj in list"
        :name="obj.name"
        :age="obj.age"
        :gender="obj.gender"
      />
    </div>
  </div>
</template>

<script>
import ListComp from "../components/ListComp.vue";
import { list } from "../../list.js";

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
  width: 50rem;
  justify-content: space-evenly;
}
</style>
