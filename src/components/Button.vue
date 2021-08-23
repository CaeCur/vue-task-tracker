<template>
  <button @click="toggleTasks()" :style="{ background: color }" class="btn">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
    color: String,
  },
  methods: {
    toggleTasks() {
      this.$emit("btn-click");
    },
  },
};
</script>

<style scoped>
</style>