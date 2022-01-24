<template>
  <!-- Content in this component, things you will export -->
  <header>
    <h1>{{ title }}</h1>
  </header>
</template>

<script>
// * JS logic about this component, define export first
export default {
  name: 'Header',
  //   props: ['title'],
  //   props: {
  //     title: String,
  //   },
  props: {
    title: {
      type: String,
      default: 'Hello World',
      //   When you don't have a value for title, the default value will take in charge.
    },
    // * These three ways of defining props are all ok.
  },
};
</script>

<style scoped>
/* scoped means anything in here will be only used for this component particular. */
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
