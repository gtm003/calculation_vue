<template>
  <v-container>
    <v-card>
      <v-card-title>
        <h3>{{ variant.title }}</h3>
        <v-spacer></v-spacer>
        <h4>400</h4>
      </v-card-title>
      <div class="d-flex flex-no-wrap justify-space-between">
        <v-card-text class="text-block">{{ variant.description }}</v-card-text>
        <v-divider inset vertical></v-divider>
        <v-card-actions class="action-block">
          <v-checkbox
            v-model="checkbox"
            :label="`Checkbox 1: ${checkbox.toString()}`"
          ></v-checkbox>
          <v-btn color="#2fcb5a" elevation="2"> Выбрано </v-btn></v-card-actions
        >
      </div>
    </v-card>
  </v-container>
</template>

<script>
export default {
  props: {
    variant: {
      type: Object,
      reqired: true,
    },
  },
    data: () => ({
    checkbox: true,
  }),
};
</script>

<style scoped>
.text-block {
  white-space: pre-line;
  font-size: 1rem;
  width: 600px;
}

.action-block {
  flex-direction: column;
}
</style>
