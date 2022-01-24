<template>
  <!-- Content in this component, things you will export -->
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
    <Button text="Update Task" color="blue" />
    <Button text="Delete Task" color="red" />
    <!-- By this way, the button component is reusable -->
  </header>
</template>

<script>
import Button from './Button.vue';
export default {
  name: 'Header',
  components: {
    Button,
  },
  props: {
    title: String,
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
