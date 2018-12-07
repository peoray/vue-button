<template>
  <div>
    <button class="btn">{{ label }}</button>
  </div>
</template>

<script>
export default {
    props: ['label']
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
</style>
