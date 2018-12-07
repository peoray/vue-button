<template>
  <div id="app">
    <Button :rounded="rounded" :label="label"/>
    <hr>
    <Test/>
  </div>
</template>

<script>
import Button from "./components/Button.vue";
import Test from "./components/test.vue";

export default {
  name: "app",
  components: {
    Button,
    Test
  },
  data() {
    return {
      label: "zagadat"
    };
  },
  computed: {
    rounded() {
      return {
        borderRadius: "100px"
      };
    }
  }
};
</script>

<style>
</style>
