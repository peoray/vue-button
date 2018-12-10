<template>
  <div>
    <button class="btn" :class="classObject">
      <slot></slot>
    </button>
  </div>
</template>

<script>
export default {
  props: {
    round: {
      type: Boolean,
      default: false
    },
    size: {
      type: String,
      default: "medium"
    }
    // disabled: {
    //   type: Boolean,
    //   default: false
    // }
  },
  computed: {
    classObject() {
      return {
        round: this.round,
        [this.size]: true
      };
    }
    // disable() {
    //   return true ? this.disabled : false;
    // }
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

.btn:disabled {
  cursor: not-allowed;
  background-color: #777;
}

.round {
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
  padding: 15px 25px;
  font-size: 20px;
}
</style>
