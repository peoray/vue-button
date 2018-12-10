<template>
  <div>
    <button :class="{btn: true, rounded: round, small: small, medium, large}">{{ label }}</button>
  </div>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      required: true
    },
    round: {
      type: Boolean,
      default: false
    },
    small: {
      type: String
    },
    medium: {
      type: String
    },
    large: {
      type: String
    }
  }
};
</script>

<style scoped>
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

.small {
  padding: 1px 1px;
  font-size: 11px;
}

.medium {
  padding: 10px 20px;
  font-size: 14px;
}

.large {
  padding: 10px 20px;
  font-size: 14px;
}
</style>
