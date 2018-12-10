<template>
  <div id="app">
    <app-button round small :label='label'></app-button>
    <hr>
    <app-test/>
  </div>
</template>

<script>
import Button from "./components/PButton.vue";
import Test from "./components/test.vue";

export default {
  name: "app",
  components: {
    'app-button': Button,
    'app-test': Test
  },
  data() {
    return {
      label: "zagadat"
    };
  }
};
</script>

<style>
</style>
