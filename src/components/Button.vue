<template>
  <button class="btn" :style="{ background: color }" @click="onClick()">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'Button',
  props: {
    text: String,
    color: String,
  },
  methods: {
    onClick() {
      this.$emit('toggle-add-task');
      // * this button shows in the Header component, so the 'toggle-add-task' function is emitted to Header
    },
  },
};
</script>
