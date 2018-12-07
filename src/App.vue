<template>
  <div id="app">
    <Button :label='label'/>
    <hr>
    <Test />
  </div>
</template>

<script>
import Button from './components/Button.vue'
import Test from './components/test.vue'

export default {
  name: 'app',
  components: {
    Button,
    Test
  },
  data() {
    return {
      label: 'zagadat'
    }
  }

}
</script>

<style>
</style>
