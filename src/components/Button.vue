<template>
  <div>
    <button :class="{'btn': true, 'rounded': round}">{{ label }}</button>
  </div>
</template>

<script>
export default {
  props: {
    label: String,
    round: {
      type: Boolean
    }
  }
};
</script>

<style>
.btn {
  padding: 10px 20px;
  font-size: 14px;
  color: #fff;
  background-color: #7744ee;
  border: 0;
  outline: none;
}

.rounded {
  border-radius: 100px;
}
</style>
