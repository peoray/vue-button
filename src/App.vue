<template>
  <div id="app">
    <app-button disabled>Hello vue</app-button>
  </div>
</template>

<script>
import appButton from "./components/PButton";

export default {
  name: "app",
  components: {
    "app-button": appButton
  }
};
</script>
