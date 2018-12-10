<template>
  <div>
    <p>I want to use this button test</p>
    <Button  :label='label' small/>
  </div>
</template>

<script>
import Button from "./PButton.vue";
export default {
    components: {
        Button
    },
    data() {
      return {
        label: 'zoe'
      }
    }
};
</script>

<style>
</style>
