<template>
  <div>
    <button class="btn" :class="{round, classObject}">{{ label }}</button>
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
    size: {
      type: String,
      default: "medium"
    }
  },
  computed: {
    classObject() {
      let desiredSize = this.size;
      return {
        [desiredSize]: true // cannot remember off top of head
      };
    }
    // classObject() {
    //   return {
    //     small: this.size === "small",
    //     medium: this.size === "medium",
    //     large: this.size === "large"
    //   };
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
