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
      this.$emit('btn-click');
      // * change this emit as 'btn-click' can make the button emit event reusable.
      // * In the upper level, Header, it can change the name to make this event more reasonable.
      // * But the whole process is still the same.
      // * If we have another component needs to use the button and emit sth, we need to define the function the name in upper level components.
    },
  },
};
</script>
