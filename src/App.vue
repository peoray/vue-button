<template>
  <div id="app">
    <app-button>Hello vue</app-button>
  </div>
</template>

<script>
import Button from "./components/PButton";

export default {
  name: "app",
  components: {
    "app-button": Button
  }
};
</script>
