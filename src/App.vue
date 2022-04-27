<template>
  <v-app>
    <div class="d-flex align-center">
      <CalculationsPage />
    </div>
    <v-btn color="#2fcb5a" elevation="2" x-large>
      <h2 class="mr-2" color="white">ИТОГО К ОПЛАТЕ</h2>
      <v-spacer></v-spacer>
      <h3 class="mr-2">3900 Р</h3>
    </v-btn>
  </v-app>
</template>

<script>
import CalculationsPage from "./components/CalculationsPage";

export default {
  name: "App",
  components: {
    CalculationsPage,
  },
};
</script>

<style scoped>
h2, h3 {
  font-weight: normal;
  color: white;
}

h2 {
  font-weight: 700;
}

a {
  color: #42b983;
}
</style>