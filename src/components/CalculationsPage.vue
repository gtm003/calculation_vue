<template>
  <v-container>
    <v-divider inset></v-divider>
    <h3>{{ firstBlock.title }}</h3>
    <Card v-for="variant in firstBlock.variants" :variant="variant" />
  </v-container>
</template>

<script>
import data from "../assets/data.json";
import Card from "./Card.vue";

export default {
  components: {
    Card,
  },
  data: () => ({
    firstBlock: data[0],
  }),
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1,
h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
